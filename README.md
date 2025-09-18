# Call Analysis System

## Overview

The Call Analysis System is an AI-powered workflow for transforming business call transcripts into structured insights and targeted communications. It leverages Claude Code's capabilities to generate comprehensive call analyses and follow-up emails.

## Key Features

- 🔍 Intelligent Call Transcript Analysis
- 📧 Automated Email Generation
- 📂 Structured Output Management
- 🤖 AI-Powered Content Creation

## Quick Start

In Claude Code, simply run:
```
/analyze_call <transcript-file>
/write_emails
```

## Project Structure

```
call-analysis-system/
├── .claude/
│   └── commands/
│       ├── analyze_call.md      # Command for analyzing call transcripts
│       └── write_emails.md      # Command for generating follow-up emails
├── templates/
│   ├── call-analysis-template.md
│   ├── email-templates/
│   │   ├── stakeholder-update.md
│   │   ├── action-items.md
│   │   └── next-meeting-goals.md
│   └── email-tone-guide.md
├── output/                       # Generated call analysis and email outputs
└── sample-transcript.md          # Example transcript for testing
```

## Workflow

### 1. Analyze Call Transcript

Run `/analyze_call` with your transcript:
- Reads the transcript
- Uses the call analysis template
- Creates an organized output directory
- Generates a comprehensive call analysis

### 2. Generate Follow-up Emails

Run `/write_emails`:
- Finds the most recent call analysis
- Uses predefined email templates
- Generates multiple email types:
  - Stakeholder update
  - Action items
  - Next meeting goals

## Prerequisites

- Claude Code CLI
- Text transcript of business calls

## Customization

Modify templates in the `templates/` directory to:
- Adjust analysis structure
- Refine email communication style
- Add organization-specific sections

## Best Practices

- Use consistent transcript formatting
- Choose descriptive call titles
- Review AI-generated content before sending
- Customize templates to match organizational style

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

[Include your license information here]

