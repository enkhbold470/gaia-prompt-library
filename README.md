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
- [Story Generation](prompts/creative/story-generation.md) - Prompts for generating engaging short stories with GAIA models

### Productivity
- [Task Planner](prompts/productivity/task-planner.md) - Prompts for project planning and task management optimized for GAIA

### Educational
- [Concept Explainer](prompts/educational/concept-explainer.md) - Prompts for explaining complex concepts clearly and concisely

### Technical
- [Code Generation](prompts/technical/code-generation.md) - Prompts for efficient code generation with GAIA models

### Conversational
- [Character Chat](prompts/conversational/character-chat.md) - Prompts for engaging character-based conversations

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

## Performance Tips

For best results with GAIA's hardware:

1. **Model Selection**: 
   - For quick responses: Use Phi-3.5 Mini or Llama-3.2 1B
   - For more complex tasks: Use Llama-3.2 3B or Mistral 7B

2. **Response Length**:
   - Set explicit word/token limits in your prompts
   - For NPU-optimized performance, aim for responses under 200 words

3. **Context Management**:
   - Be specific about what information is most important
   - Structure prompts to focus the model on key details

4. **Batching Considerations**:
   - When using the same model for multiple prompts, batch them when possible
   - This is more efficient than loading/unloading models between prompts

## Contributing

We welcome contributions from the community! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details on how to submit new prompts or improve existing ones.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.