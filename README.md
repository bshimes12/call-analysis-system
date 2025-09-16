# Call Analysis System

Automated system for processing business call transcripts into structured analysis and email communications using Claude Code.

## Quick Start

### Two Main Commands

1. **Generate Call Analysis**
   ```bash
   ./scripts/generate-call-analysis.sh <transcript-file>
   ```

2. **Generate Emails**
   ```bash
   ./scripts/generate-emails.sh <call-directory>
   ```

## Project Structure

```
call-analysis-system/
├── templates/
│   ├── call-analysis-template.md       # Template for call analysis
│   ├── email-templates/
│   │   ├── stakeholder-update.md       # Stakeholder email template
│   │   ├── action-items.md             # Action items email template
│   │   └── next-meeting-goals.md       # Next meeting email template
│   └── email-tone-guide.md             # Communication tone guide
├── scripts/
│   ├── generate-call-analysis.sh       # Command 1: Generate analysis
│   └── generate-emails.sh              # Command 2: Generate emails
├── output/                             # Generated call directories
└── README.md
```

## Workflow

### Step 1: Analyze Call Transcript
```bash
./scripts/generate-call-analysis.sh my-transcript.txt
```
- Prompts for call details (title, date, duration, participants)
- Creates organized directory: `output/{call-title-and-date}/`
- Prepares analysis prompt for Claude Code
- Copies transcript to call directory

### Step 2: Use Claude Code to Generate Analysis
1. Run `claude code`
2. Navigate to the created call directory
3. Read `analysis_prompt.txt`
4. Generate `call-analysis.md` based on the prompt

### Step 3: Generate Email Communications
```bash
./scripts/generate-emails.sh output/{call-title-and-date}
```
- Creates `emails/` subdirectory
- Generates prompts for three email types
- Copies tone guide to call directory

### Step 4: Use Claude Code to Generate Emails
1. Navigate to the `emails/` directory
2. Process each prompt file to generate:
   - `stakeholder-update-email.md`
   - `action-items-email.md`
   - `next-meeting-goals-email.md`

## Output Structure

After running both commands and Claude Code generation:

```
output/{call-title-and-date}/
├── transcript.txt                      # Original transcript
├── call-analysis.md                    # Generated analysis
├── email-tone-guide.md                 # Communication guidelines
└── emails/
    ├── stakeholder-update-email.md     # Generated stakeholder email
    ├── action-items-email.md           # Generated action items email
    └── next-meeting-goals-email.md     # Generated next meeting email
```

## Features

- **Automated Directory Structure**: Organized by call title and date
- **Comprehensive Analysis**: Extracts key decisions, action items, next steps
- **Multiple Email Types**: Stakeholder updates, action items, meeting goals
- **Consistent Tone**: Professional communication guidelines
- **Claude Code Integration**: Leverages AI for intelligent content generation
- **Template-Based**: Customizable templates for consistent output

## Usage Tips

- Keep transcript files in a consistent format
- Use descriptive call titles for better organization
- Review generated content before sending emails
- Customize templates as needed for your organization
- Use consistent naming conventions for better tracking