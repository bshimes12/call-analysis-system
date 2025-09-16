# Call Analysis System

## Overview

The Call Analysis System is an automated workflow tool designed to transform business call transcripts into structured, actionable insights. Leveraging Claude Code's AI capabilities, this system generates comprehensive call analyses and targeted email communications.

## Key Features

- 🔍 Intelligent Call Analysis
- 📧 Automated Email Generation
- 📂 Structured Output Management
- 🤖 AI-Powered Content Creation

## Prerequisites

- Bash shell
- Claude Code CLI
- Text transcript of business calls

## Installation

1. Clone the repository:
```bash
git clone https://github.com/your-org/call-analysis-system.git
cd call-analysis-system
```

2. Ensure scripts are executable:
```bash
chmod +x scripts/*.sh
```

## Quick Start

### 1. Generate Call Analysis

Process a call transcript:
```bash
./scripts/generate-call-analysis.sh <path-to-transcript>
```

#### Example
```bash
./scripts/generate-call-analysis.sh transcripts/client-meeting.txt
```

### 2. Generate Email Communications

Create email drafts from call analysis:
```bash
./scripts/generate-emails.sh <output-directory>
```

#### Example
```bash
./scripts/generate-emails.sh output/client-meeting-2025-09-15
```

## Workflow Details

1. **Transcript Processing**
   - Extracts key call details
   - Creates organized output directory
   - Prepares analysis prompts

2. **AI-Powered Analysis**
   - Generates comprehensive call summary
   - Identifies key decisions and action items
   - Creates structured markdown report

3. **Email Generation**
   - Produces multiple email types:
     - Stakeholder update
     - Action items
     - Next meeting goals

## Output Structure

```
output/{call-title-and-date}/
├── transcript.txt
├── call-analysis.md
├── email-tone-guide.md
└── emails/
    ├── stakeholder-update-email.md
    ├── action-items-email.md
    └── next-meeting-goals-email.md
```

## Best Practices

- Use consistent transcript formatting
- Choose descriptive call titles
- Review AI-generated content before sending
- Customize templates to match organizational style

## Customization

Modify templates in the `templates/` directory to:
- Adjust analysis structure
- Refine email communication style
- Add organization-specific sections

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

[Include your license information here]

## Support

For issues or questions, please [add your support contact or method]