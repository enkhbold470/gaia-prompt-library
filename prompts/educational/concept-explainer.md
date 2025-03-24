# GAIA Educational Concept Explainer Prompts

> A collection of prompts optimized for AMD GAIA models to explain complex concepts clearly and concisely.

These prompts are specially designed to work efficiently with GAIA's NPU+iGPU architecture or Generic mode. They focus on clear explanations while minimizing computational overhead.

## Prompts

### Basic Concept Explainer

**Template:**
```
Explain the concept of [CONCEPT] in simple terms.
Follow these guidelines:
- Start with a one-sentence definition
- Break down into 3-4 key components
- Use a concrete, everyday example
- Mention one practical application
- Keep your explanation under 200 words
```

**Example:**
```
Explain the concept of quantum computing in simple terms.
Follow these guidelines:
- Start with a one-sentence definition
- Break down into 3-4 key components
- Use a concrete, everyday example  
- Mention one practical application
- Keep your explanation under 200 words
```

**Tips for Best Results:**
- Replace [CONCEPT] with a specific, well-defined concept
- For technical topics, specify the desired level (beginner, intermediate, etc.)
- Works well with both Hybrid and Generic mode models

### Comparative Concept Analysis

**Template:**
```
Compare and contrast [CONCEPT_A] and [CONCEPT_B] with the following structure:
1. One-sentence definition of each
2. Three key similarities
3. Three important differences
4. When to use each one
5. A simple example of each in practice
Use simple language and limit your response to 250 words.
```

**Example:**
```
Compare and contrast machine learning and rule-based systems with the following structure:
1. One-sentence definition of each
2. Three key similarities
3. Three important differences
4. When to use each one
5. A simple example of each in practice
Use simple language and limit your response to 250 words.
```

**Tips for Best Results:**
- Choose concepts that have meaningful comparisons
- Works well with 3B+ parameter models in GAIA
- Consider specifying a domain or context for more relevant comparisons

### ELI5 (Explain Like I'm 5)

**Template:**
```
Explain [COMPLEX_CONCEPT] like I'm 5 years old.
Your explanation should:
- Use extremely simple vocabulary
- Include a fun analogy with [FAMILIAR_OBJECT/SCENARIO]
- Be engaging and conversational
- Avoid any technical jargon
- Be 100-150 words long
```

**Example:**
```
Explain black holes like I'm 5 years old.
Your explanation should:
- Use extremely simple vocabulary
- Include a fun analogy with a bathtub drain
- Be engaging and conversational
- Avoid any technical jargon
- Be 100-150 words long
```

**Tips for Best Results:**
- This prompt works particularly well with Phi-3.5 Mini and Llama-3.2 3B models
- Replace [FAMILIAR_OBJECT/SCENARIO] with something children would understand
- For very complex topics, you may need to greatly simplify certain aspects

## Performance Notes

These prompts have been optimized to:
1. Minimize token usage while maximizing educational value
2. Structure responses to reduce computational demands
3. Work efficiently with GAIA's NPU+iGPU architecture

For best performance:
- Smaller models (<3B parameters) perform well with the Basic Concept Explainer
- Larger models (3B+) excel with the Comparative Concept Analysis 
- All models perform well with the ELI5 format, which keeps responses concise