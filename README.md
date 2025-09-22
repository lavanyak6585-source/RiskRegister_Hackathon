# RiskRegister_Hackathon

Welcome to the Open Source Risk Scoring Template

This workbook helps you calculate and prioritize risk scores for open source components based on multiple factors.

Instructions:
1. Go to the 'Risk Scoring' sheet.
2. For each component, fill in the following columns:
   - CVSS_Base: Base score from CVSS (0.0 to 10.0).
   - Exposure_Factor: 1.0 (internal) to 2.0 (public-facing).
   - Criticality_Factor: 1.0 (non-critical) to 2.0 (premium/SOC-audited).
   - Maintainer_Factor: 0.5 (maintained) to 1.5 (unmaintained).
   - Version_Gap_Factor: 1.0 (up-to-date) to 2.0 (major version behind).
   - Microsoft_Usage_Factor: 0.5 (MS-authored) to 1.5 (third-party only).
3. The Risk Score is automatically calculated using the formula:
   Risk Score = CVSS_Base × Exposure × Criticality × Maintainer × Version Gap × MS Usage

Risk Score Interpretation:
- >80: Critical (Red)
- 60–80: High (Orange)
- 40–60: Medium (Yellow)
- <40: Low (Green)

Use this template to prioritize remediation efforts and track risk across components.

Factor Descriptions:
CVSS_Base: Severity of the vulnerability (from NVD, GitHub, etc.).
Exposure_Factor: How exposed the component is (public-facing = higher risk).
Criticality_Factor: Importance of the service using the component.
Maintainer_Factor: How actively the component is maintained.
Version_Gap_Factor: How outdated the component is.
Microsoft_Usage_Factor: Lower risk if widely used or authored internally.
<img width="991" height="32766" alt="image" src="https://github.com/user-attachments/assets/c6479908-9b7d-4e99-9999-d3f972a6df15" />
