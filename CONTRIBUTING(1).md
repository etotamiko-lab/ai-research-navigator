# Contributing to AI Research Navigator

Thank you for your interest in improving the AI Research Navigator! This document provides guidelines for making content updates and customizations.

## Making Content Changes

The decision tree content is contained entirely within the `decisionTree` JavaScript object in the HTML file (starting around line 425). You can edit questions, explanations, and guidance text directly.

### Structure Overview

Each decision node follows this structure:

```javascript
node_name: {
    question: "Main question text displayed as heading",
    info: "Plain language explanation of what the question means",
    encouragement: "Supportive message to reduce anxiety (optional)",
    tip: "Helpful hint or example (optional)",
    details: [  // Optional array for detailed sections
        { 
            title: "Section Title", 
            content: "Detailed explanation text" 
        }
    ],
    options: [  // Array of choice buttons
        { 
            label: "Button text user sees",
            next: "name_of_next_node",
            summary: "Short description for decision log",
            why: "Regulatory citation and reasoning"
        }
    ]
}
```

### Content Guidelines

**Tone:**
- Warm, encouraging, non-judgmental
- Assumes good faith and intelligence
- Acknowledges complexity and uncertainty
- Empowers users to make informed decisions

**Structure:**
- Lead with plain language, follow with regulatory specifics
- Use concrete examples over abstract principles
- Break complex concepts into digestible sections
- Provide "red flags" and "green lights" for clarity

**Regulatory Accuracy:**
- Always cite specific CFR sections when relevant
- Use current FDA guidance (as of 2026)
- Distinguish between requirements and best practices
- Note when legal counsel should be consulted

### Common Content Updates

**Updating a Question:**
```javascript
question: "Your new question text here",
```

**Adding Encouragement:**
```javascript
encouragement: "You're doing great! This is a tricky distinction...",
```

**Adding a Tip:**
```javascript
tip: "Quick hint: If you plan to publish, it's research.",
```

**Adding Detail Sections:**
```javascript
details: [
    { 
        title: "Key Distinction", 
        content: "Detailed explanation with examples..." 
    },
    { 
        title: "Common Pitfalls", 
        content: "What to watch out for..." 
    }
],
```

**Updating Button Text:**
```javascript
options: [
    { 
        label: "Your updated button text",
        next: "next_node_name",
        summary: "Updated summary",
        why: "Updated regulatory reasoning"
    }
]
```

### Updating Results

Result nodes have a different structure:

```javascript
node_name: {
    conclusion: true,
    result: {
        title: "Result Title",
        badge: "Badge Text (e.g., 'Full Board Review Required')",
        celebration: "Positive reinforcement message",
        why_final: "Comprehensive explanation with regulatory framework",
        next_steps: "Specific actionable steps"
    }
}
```

### Testing Your Changes

1. Save your modified HTML file
2. Open it in a web browser
3. Walk through the entire decision tree
4. Test all pathways to ensure logic flows correctly
5. Test the PDF export functionality
6. Test the back button navigation
7. Check mobile responsiveness

### Regulatory Updates

When regulatory guidance changes (e.g., new FDA guidance, CFR amendments):

1. Identify affected nodes
2. Update regulatory citations
3. Revise examples if necessary
4. Update the "why" explanations
5. Test to ensure logic remains sound
6. Document changes in version history

## Style Consistency

### Writing Style
- Use second person ("you", "your") not third person
- Active voice over passive voice
- Short paragraphs (2-4 sentences)
- Bullet points for lists of criteria
- Bold for emphasis, not ALL CAPS

### Regulatory Citations
- Format: `45 CFR 46.102(l)` or `21 CFR Part 56`
- Full names on first use: "Institutional Review Board (IRB)"
- Abbreviations after: "IRB"

### Examples Format
```
CLEAR EXAMPLES:
• Algorithm DESIGNED to... → Device
• Tool DESIGNED to... → Not a device
```

## Institutional Customizations

You may customize content for your institution while maintaining attribution:

**Allowed:**
- Adding institution-specific examples
- Referencing local policies or procedures
- Adjusting tone slightly for your audience
- Adding local contact information in results

**Required:**
- Keep all TechInHSR attributions intact
- Maintain copyright notices
- Note that customizations have been made
- Retain link to TechInHSR.com

**Not Allowed:**
- Removing or obscuring TechInHSR branding
- Claiming the tool as your own creation
- Redistributing modified versions publicly

## Questions or Suggestions?

For questions about:
- **Content accuracy**: Contact TechInHSR LLC at info@TechInHSR.com
- **Technical issues**: Check browser console for error messages
- **Licensing**: See LICENSE file or contact TechInHSR LLC
- **Training**: Visit TechInHSR.com for workshop information

## Version Control Best Practices

- Make incremental changes and test frequently
- Keep notes on what you've customized
- Maintain a changelog for institutional versions
- Consider version numbering (v1.0-YourInstitution)

---

**Remember**: This tool provides educational guidance. Always consult your IRB and legal counsel for official determinations.
