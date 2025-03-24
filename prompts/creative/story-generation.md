# Story Generation Prompts

This collection contains prompts specifically designed for generating stories with GAIA models. These prompts are optimized for the NPU+iGPU architecture to provide the best possible creative writing experience while maintaining efficient performance.

## Short Story Generator

### Prompt Template
```
Create a short story based on the following elements:
- Setting: [SETTING]
- Main character: [CHARACTER]
- Theme: [THEME]
- Conflict: [CONFLICT]
- Time period: [TIME_PERIOD]

The story should be between 200-300 words and follow a clear beginning, middle, and end structure.
```

### Example

```
Create a short story based on the following elements:
- Setting: A remote research station in Antarctica
- Main character: A botanist who discovers an unusual plant growing in the ice
- Theme: Discovery and isolation
- Conflict: The plant begins exhibiting strange properties that affect the station's equipment
- Time period: Near future

The story should be between 200-300 words and follow a clear beginning, middle, and end structure.
```

### Tips for Best Results
- Be specific about the setting and character details
- Limit the word count to avoid overwhelming the model
- Provide a clear conflict to give the story direction
- Works best with Phi-3.5 Mini Instruct and Llama-3.2 3B Instruct models

## Character-Driven Scene

### Prompt Template
```
Write a scene where [CHARACTER 1] and [CHARACTER 2] are [SITUATION]. Their personalities are:

[CHARACTER 1]:
- Trait 1: [TRAIT]
- Trait 2: [TRAIT]
- Goal: [GOAL]

[CHARACTER 2]:
- Trait 1: [TRAIT]
- Trait 2: [TRAIT]
- Goal: [GOAL]

Include meaningful dialogue that reveals their personalities. The scene should be 250-350 words.
```

### Example

```
Write a scene where a seasoned detective and a new partner are investigating a crime scene. Their personalities are:

Detective Rivera:
- Trait 1: Cynical and bitter after 20 years on the force
- Trait 2: Highly observant of small details
- Goal: Solve the case quickly to move on to retirement

Officer Chen:
- Trait 1: Enthusiastic and idealistic rookie
- Trait 2: Technology-savvy with modern investigation techniques
- Goal: Prove herself worthy of being a detective

Include meaningful dialogue that reveals their personalities. The scene should be 250-350 words.
```

### Tips for Best Results
- Clearly define contrasting character traits to create tension
- Give each character a specific goal that may conflict with the other
- Specify the scene's location and context
- Works well with Mistral 7B Instruct and Qwen 1.5 7B Chat models

## Plot Twist Generator

### Prompt Template
```
Create a surprising but logical plot twist for a story with these elements:
- Genre: [GENRE]
- Setup: [SETUP]
- Main character: [CHARACTER]
- What readers are led to believe: [EXPECTATION]

The twist should subvert expectations while remaining consistent with the established elements. Keep it under 150 words.
```

### Example

```
Create a surprising but logical plot twist for a story with these elements:
- Genre: Mystery thriller
- Setup: A valuable painting has been stolen from a museum, with security footage showing the curator entering the secure room just before the theft
- Main character: A detective who has been friends with the curator for years
- What readers are led to believe: The curator is the prime suspect due to the evidence and financial problems

The twist should subvert expectations while remaining consistent with the established elements. Keep it under 150 words.
```

### Performance Notes
This prompt works effectively on NPU+iGPU hardware because it:
- Keeps the output relatively short (under 150 words)
- Provides specific constraints that help the model focus
- Includes enough context without overloading the context window

Optimal models: Phi-3 Mini Instruct, Llama-3.2 1B Instruct