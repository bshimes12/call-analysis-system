---
description: "Generate follow-up emails based on call analysis using email templates"
---

# Generate Follow-up Emails

Please generate follow-up emails based on the most recent call analysis.

I will:
1. Find the most recent call analysis in: `@output/*/analysis/call-analysis.md`
2. Use the email templates: `@templates/email-templates/`
3. Reference the email tone guide: `@templates/email-tone-guide.md`
4. Create directory: `output/$(date +%Y-%m-%d)/emails/`
5. Generate emails for different stakeholders and purposes

## Email Types to Generate:
- **stakeholder-update.md** - General update for stakeholders
- **action-items.md** - Focused on action items and deadlines
- **next-meeting-goals.md** - Preparation for next meeting

## Instructions:
- Use the call analysis data to populate email templates
- Follow the tone and style guidelines
- Customize content for each email type's specific purpose
- Save each email as a separate .md file in the emails directory
- Include proper placeholders that can be easily customized

Generate all three email types now based on the latest call analysis.