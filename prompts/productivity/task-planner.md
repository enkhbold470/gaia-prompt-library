# GAIA Task Planning & Productivity Prompts

> A collection of prompts optimized for AMD GAIA models to enhance productivity and organization.

These prompts are designed to work efficiently with GAIA's resource constraints while maximizing practical utility for planning, organization, and productivity tasks.

## Prompts

### Project Breakdown Planner

**Template:**
```
Break down this project into manageable tasks:
Project: [PROJECT_NAME]
Description: [BRIEF_DESCRIPTION]
Deadline: [DEADLINE]
Available time: [HOURS_AVAILABLE] hours

Format your response as:
1. Brief project overview (2 sentences)
2. List of 4-7 main tasks with estimated time for each
3. Dependencies between tasks (which must be completed first)
4. Top 3 potential challenges and simple solutions
5. A proposed schedule given the deadline

Keep your response concise and actionable.
```

**Example:**
```
Break down this project into manageable tasks:
Project: Home Office Renovation
Description: Converting spare bedroom into functional home office
Deadline: 2 weeks from now
Available time: 20 hours

Format your response as:
1. Brief project overview (2 sentences)
2. List of 4-7 main tasks with estimated time for each
3. Dependencies between tasks (which must be completed first)
4. Top 3 potential challenges and simple solutions
5. A proposed schedule given the deadline

Keep your response concise and actionable.
```

**Tips for Best Results:**
- Provide realistic timeframes and deadlines
- Works well with all GAIA models, including smaller parameter models
- More detailed project descriptions will yield more specific task breakdowns

### Daily Priority Optimizer

**Template:**
```
Help me optimize my day with these tasks:
[TASK_1]
[TASK_2]
[TASK_3]
...
[TASK_N]

My working hours are [START_TIME] to [END_TIME].
My energy level is typically highest in the [MORNING/AFTERNOON/EVENING].
Each task should take approximately [X] minutes/hours.

Provide:
1. Optimal task sequence with specific time blocks
2. Which 2-3 tasks are most important and why
3. Which task(s) could be delegated or postponed if needed
4. One 15-minute break and when to take it

Keep your response under 200 words.
```

**Example:**
```
Help me optimize my day with these tasks:
Write quarterly report
Prepare presentation for team meeting
Respond to client emails
Update project documentation
Review team's code submissions
One-on-one meeting with direct report

My working hours are 9:00 AM to 5:00 PM.
My energy level is typically highest in the morning.
Each task should take approximately 1 hour.

Provide:
1. Optimal task sequence with specific time blocks
2. Which 2-3 tasks are most important and why
3. Which task(s) could be delegated or postponed if needed
4. One 15-minute break and when to take it

Keep your response under 200 words.
```

**Tips for Best Results:**
- This works well with Phi-3.5 Mini and other small models
- Being specific about your energy patterns improves the schedule quality
- List tasks in no particular order for unbiased optimization

### Decision Matrix Generator

**Template:**
```
Create a decision matrix for choosing between these options:
Options: [OPTION_1], [OPTION_2], [OPTION_3]
Goal: [DECISION_GOAL]

Please use these criteria to evaluate (scale 1-5, where 5 is best):
- [CRITERIA_1]
- [CRITERIA_2]
- [CRITERIA_3]
- [CRITERIA_4]

Format as a simple markdown table with:
- Options as rows
- Criteria as columns
- A final "Total" column
- Brief 1-2 sentence recommendation based on highest score
```

**Example:**
```
Create a decision matrix for choosing between these options:
Options: Hire full-time employee, Contract with freelancer, Outsource to agency
Goal: Develop new company website

Please use these criteria to evaluate (scale 1-5, where 5 is best):
- Cost efficiency
- Quality control
- Timeline reliability
- Long-term maintenance

Format as a simple markdown table with:
- Options as rows
- Criteria as columns
- A final "Total" column
- Brief 1-2 sentence recommendation based on highest score
```

**Tips for Best Results:**
- Works best with 3B+ parameter models in GAIA
- Using 3-5 criteria yields the most balanced analysis
- Equal weighting is applied by default; specify if certain criteria should be weighted differently

## Performance Notes

These prompts have been optimized for GAIA by:
1. Limiting response length to reduce computational load
2. Using structured formats that are easier for models to generate
3. Focusing on practical outcomes rather than lengthy explanations

For best results:
- Llama-3.2 3B and Phi-3.5 Mini perform particularly well with these structured productivity prompts
- Adding specific constraints (word counts, formats) helps keep responses concise
- These prompts work in both Hybrid NPU+iGPU mode and Generic mode