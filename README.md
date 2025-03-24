# GAIA Prompt Library

A collection of optimized prompts for AMD GAIA LLM models, designed to get the best performance from models running on Ryzen AI NPU hardware.

## About This Project

The GAIA Prompt Library aims to be a comprehensive resource for users of AMD's GAIA framework. It provides carefully crafted prompts that are optimized for the various models supported by GAIA, taking into account the unique capabilities and limitations of the NPU+iGPU hybrid execution environment.

## Contents

- [Prompt Categories](#prompt-categories)
- [Optimization Techniques](#optimization-techniques)
- [Models](#models)
- [Contributing](#contributing)
- [License](#license)

## Prompt Categories

### Creative Writing
- [Story Generation](prompts/creative/story-generation.md)
- [Poetry and Lyrics](prompts/creative/poetry-lyrics.md)
- [Character Development](prompts/creative/character-development.md)

### Productivity
- [Email Composition](prompts/productivity/email-composition.md)
- [Note Taking](prompts/productivity/note-taking.md)
- [Task Planning](prompts/productivity/task-planning.md)

### Educational
- [Study Guides](prompts/educational/study-guides.md)
- [Concept Explanation](prompts/educational/concept-explanation.md)
- [Problem Solving](prompts/educational/problem-solving.md)

### Technical
- [Code Explanation](prompts/technical/code-explanation.md)
- [Bug Fixing](prompts/technical/bug-fixing.md)
- [Code Generation](prompts/technical/code-generation.md)

### Conversational
- [Interview Simulation](prompts/conversational/interview-simulation.md)
- [Debate Partner](prompts/conversational/debate-partner.md)
- [Language Practice](prompts/conversational/language-practice.md)

## Optimization Techniques

This library employs several techniques to optimize prompts for GAIA models running on NPU+iGPU hardware:

### Token Efficiency
Prompts are designed to be concise while providing sufficient context, maximizing the available context window and reducing inference time.

### Instruction Clarity
Clear and explicit instructions help models running on more constrained hardware provide better responses without multiple clarification rounds.

### Context Management
Techniques for managing context when working with the limited context windows of quantized models on NPU hardware.

### Model-Specific Adjustments
Tailored prompts for different models (Phi-3, Llama-3.2, Mistral, etc.) to leverage their unique strengths when running on GAIA.

## Models

This library includes prompts optimized for all models officially supported by GAIA:

### NPU+iGPU Hybrid Mode
- Phi-3.5 Mini Instruct
- Phi-3 Mini Instruct
- Llama-2 7B Chat
- Llama-3.2 1B Instruct
- Llama-3.2 3B Instruct
- Qwen 1.5 7B Chat
- Mistral 7B Instruct

### Generic Mode
- Llama 3.2 1B
- Llama 3.2 3B
- Llama 3.1 8B

## Getting Started

To use these prompts:

1. Ensure you have [GAIA installed](https://github.com/amd/gaia) on your Ryzen AI PC
2. Browse to the prompt category you're interested in
3. Copy the prompt template and fill in the required information
4. Paste the completed prompt into GAIA's web interface or CLI

## Contributing

We welcome contributions from the community! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details on how to submit new prompts or improve existing ones.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.