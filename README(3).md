# AI Research Navigator - IRB Decision Tree Tool

**Interactive regulatory guidance tool for AI human subjects research**

A comprehensive, user-friendly web application that guides researchers and IRB professionals through the complex regulatory landscape of AI research oversight. Built on the Eto 3-Stage Framework, adopted by 23+ institutions.

## Overview

The AI Research Navigator helps determine:
- Whether a project requires IRB review
- What type of review pathway is appropriate (Expedited vs. Full Board)
- Medical device classification under FDA regulations
- Quality Improvement vs. Research distinctions
- Human subjects research determinations
- Stage-appropriate oversight for AI development

## Features

- **Warm, Educational Tone**: Reduces anxiety and builds confidence through supportive guidance
- **Progressive Disclosure**: Reveals complexity gradually with contextual tips and explanations
- **Regulatory Precision**: Based on 45 CFR 46, 21 CFR 56/812/820, FDA 2026 CDS guidance
- **Visual Progress Tracking**: Shows users where they are in the decision process
- **Comprehensive Results**: Provides regulatory citations, next steps, and decision journey documentation
- **PDF Export**: Downloadable summary for IRB submissions and records
- **Mobile Responsive**: Works seamlessly on phones, tablets, and desktops

## Technical Implementation

- **Pure HTML/CSS/JavaScript**: No build process required
- **External Dependencies**: 
  - Google Fonts (Crimson Pro, DM Sans)
  - html2pdf.js (for PDF generation)
- **Browser Compatibility**: Modern browsers (Chrome, Firefox, Safari, Edge)

## Usage

### For End Users

1. Open `AIHSR_DecisionTree_Final.html` in any modern web browser
2. Click "I'm ready - let's start" to begin the assessment
3. Answer questions honestly based on your project's actual characteristics
4. Use the "Go Back" button to revise answers if needed
5. Review your personalized results with regulatory citations
6. Download the PDF summary for your records

### For Developers/Customizers

The decision tree logic is contained in the `decisionTree` JavaScript object (starting around line 425). Each node contains:

```javascript
node_name: {
    question: "The question text",
    info: "Plain language explanation",
    encouragement: "Supportive message (optional)",
    tip: "Helpful hint (optional)",
    details: [{ title: "Section", content: "Detailed info" }], // optional
    options: [
        { 
            label: "Button text", 
            next: "next_node_name", 
            summary: "Log entry", 
            why: "Regulatory citation" 
        }
    ]
}
```

Result nodes use:
```javascript
node_name: {
    conclusion: true,
    result: {
        title: "Result Title",
        badge: "Badge Text",
        celebration: "Celebration Message",
        why_final: "Full explanation with regulatory framework",
        next_steps: "Actionable next steps"
    }
}
```

## The Eto 3-Stage Framework

This tool is built on the Eto 3-Stage Framework for AI Human Subjects Research:

- **Stage 1**: Algorithm Development & Clinical Association (existing data)
- **Stage 2**: Validation & Performance Testing (new data, "off-line")
- **Stage 3**: Clinical Investigation & Real-World Integration (live deployment)

Each stage has appropriate risk-based oversight requirements, with special considerations for medical device development.

## Key Regulatory Distinctions

### Medical Device Determination
Based on FDA 2026 Clinical Decision Support Software guidance, evaluates:
1. Does it process medical images/signals? (Criterion 1)
2. Does it display commonly-discussed medical information? (Criterion 2)
3. Does it provide patient-specific recommendations? (Criterion 3)
4. Can HCPs independently review the basis? (Criterion 4)

### Research vs. Quality Improvement
Distinguishes generalizable knowledge (research) from local improvement (QI), with special emphasis on:
- Intent to publish or share findings
- Medical device development (triggers research oversight regardless of QI label)
- Multi-site collaboration
- Hypothesis testing vs. implementing known best practices

### Synthetic Data Considerations
Addresses the common misconception that synthetic data is automatically anonymous:
- Requires formal privacy verification (e.g., differential privacy)
- Re-identification risk assessment needed
- Source data privacy implications

## About TechInHSR LLC

TechInHSR LLC provides AI research ethics consulting, IRB training, and regulatory strategy for digital health. Founded by Tamiko Eto, MA, CIP, with over 20 years of IRB leadership experience across major institutions including Mayo Clinic.

**Services:**
- AI research ethics consulting
- IRB training and workshops
- Regulatory strategy for digital health
- Expert testimony and advisory services

**Learn more:** [TechInHSR.com](https://www.TechInHSR.com)

## License

Copyright © 2026 TechInHSR LLC. All rights reserved.

This software is proprietary and confidential. See LICENSE file for full terms.

## Citation

If you use this tool in your research or institutional processes, please cite:

```
Eto, T. (2026). AI Research Navigator: Interactive IRB Decision Tree Tool. 
TechInHSR LLC. https://github.com/TechInHSR/ai-research-navigator
```

## Version History

- **v1.0.0** (January 2026): Initial release
  - Complete decision tree based on Eto 3-Stage Framework
  - FDA 2026 CDS guidance integration
  - Synthetic data considerations
  - PDF export functionality
  - Mobile-responsive design

## Support

For questions, training requests, or consulting inquiries:
- **Website**: [TechInHSR.com](https://www.TechInHSR.com)
- **Email**: info@TechInHSR.com

## Acknowledgments

This tool incorporates regulatory guidance from:
- FDA Clinical Decision Support Software Guidance (2026)
- 45 CFR 46 (Common Rule)
- 21 CFR Parts 56, 812, 820, 11
- 21 USC 321(h) (Medical Device Definition)

Developed with insights from 23+ institutions that have adopted the Eto 3-Stage Framework for AI human subjects research oversight.

---

**Disclaimer**: This tool provides educational guidance and does not constitute legal or regulatory advice. Always consult with your institution's IRB and legal counsel for specific determinations.
