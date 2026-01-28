# Changelog

All notable changes to the AI Research Navigator will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2026-01-27

### Initial Release

**Core Features:**
- Complete decision tree implementation based on Eto 3-Stage Framework
- 9-step interactive assessment process
- Real-time progress tracking with percentage completion
- Warm, educational tone throughout
- Mobile-responsive design

**Regulatory Framework:**
- Integration of FDA 2026 Clinical Decision Support Software guidance
- 45 CFR 46 (Common Rule) compliance guidance
- 21 CFR Parts 56, 812, 820, 11 references
- Medical device determination based on 4-criteria test
- Research vs. Quality Improvement distinction
- Synthetic data privacy considerations

**Key Decision Points:**
- FDA Clinical Investigation determination
- Clinical association (Stage 1) assessment
- Medical device validation (Stage 2) pathways
- Stage-appropriate review level assignment
- Human subjects research determination
- Re-identification risk evaluation

**User Experience:**
- Progressive disclosure of complexity
- Contextual tips and encouragement banners
- Detailed explanation sections with expandable content
- "Go Back" button for navigation
- Confirmation dialog on restart
- Helper tips throughout

**Results & Documentation:**
- Personalized results with regulatory citations
- Celebration messaging and positive reinforcement
- Comprehensive "What This Means For You" explanations
- Actionable "Next Steps" guidance
- Complete decision journey documentation table
- SR/NSR determination explanation
- PDF export functionality with proper formatting

**Technical Implementation:**
- Pure HTML/CSS/JavaScript (no build required)
- External fonts: Crimson Pro (serif) and DM Sans (sans-serif)
- html2pdf.js integration for PDF generation
- Event-driven architecture with proper listener management
- Responsive design with mobile-first approach

**Notable Design Decisions:**
- Removed "Phase" terminology in favor of "Stage" per Eto Framework
- Separated Stage 2 into device vs. non-device pathways
- Added explicit synthetic data guidance to prevent misconceptions
- Emphasized intended design and function over research project use
- Integrated medical device considerations into QI assessment

### Regulatory Accuracy Updates
- Based on FDA Clinical Decision Support Software Guidance (January 6, 2026)
- Reflects enforcement discretion for single clinically-appropriate recommendations
- Addresses patient-facing tools as automatic device classification
- Incorporates time-critical decision considerations
- Includes formal privacy verification requirements for synthetic data

### Known Limitations
- PDF generation requires external library load time
- Complex regulatory scenarios may require IRB consultation
- Tool provides guidance, not official determinations

---

## Future Considerations

**Potential Enhancements:**
- Additional language translations
- Integration with institutional IRB systems
- Enhanced accessibility features (WCAG AAA compliance)
- Interactive tutorial or walkthrough mode
- Save/resume functionality for long sessions
- Email summary option
- Print-friendly version without PDF library dependency

**Content Updates to Monitor:**
- FDA guidance revisions
- Changes to Common Rule (45 CFR 46)
- New device regulations (21 CFR parts)
- Emerging AI-specific regulations
- Case law affecting research oversight

**Technical Improvements:**
- Offline functionality (Progressive Web App)
- Enhanced analytics for institutional use
- API for integration with IRB management systems
- Customization interface for institutional branding

---

## Contact

For updates, questions, or to report issues:
- **Website**: [TechInHSR.com](https://www.TechInHSR.com)
- **Email**: info@TechInHSR.com

## Citation

```
Eto, T. (2026). AI Research Navigator: Interactive IRB Decision Tree Tool (Version 1.0.0). 
TechInHSR LLC. https://github.com/TechInHSR/ai-research-navigator
```
