---
description: "Analyze a call transcript and generate structured analysis using templates"
---

# Analyze Call Transcript

Please analyze the call transcript provided and generate a comprehensive call analysis.

I will:
1. Read the transcript file: `@$1`
2. Use the call analysis template: `@templates/call-analysis-template.md`
3. Create a directory structure: `output/$(date +%Y-%m-%d)/analysis/`
4. Generate a complete call analysis following the template structure

## Instructions:
- Extract key information from the transcript
- Populate all sections of the template with relevant analysis
- Save the result as `call-analysis.md` in the analysis directory
- Use today's date for the generation timestamp

Please ensure the analysis is thorough and captures:
- Executive summary of the call
- Key discussion points and decisions
- Action items and next steps
- Technical notes and stakeholder impact

Begin the analysis now.