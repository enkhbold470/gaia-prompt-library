# Contributing to GAIA Prompt Library

We're thrilled that you're interested in contributing to the GAIA Prompt Library! This document provides guidelines and instructions for contributing.

## How to Contribute

There are several ways you can contribute to this project:

1. **Add new prompts** - Create new prompt templates for different use cases
2. **Improve existing prompts** - Enhance performance or clarity of existing prompts
3. **Add model-specific optimizations** - Document how certain prompts perform better with specific GAIA models
4. **Report issues** - Let us know if you find prompts that don't work well with GAIA

## Submitting Contributions

### Adding New Prompts

1. Fork the repository
2. Create a new branch for your contribution
3. Add your prompt file in the appropriate category folder
   - If your prompt doesn't fit existing categories, propose a new one
4. Follow the standard format (see below)
5. Submit a pull request with a clear description of your contribution

### Standard Prompt Format

Please use the following format for all prompt submissions:

```markdown
# [Prompt Title]

[Brief description of what this prompt does and what it's good for]

## Prompt Template
```
[The actual template with placeholders in ALL_CAPS]
```

## Example
```
[A complete example with the placeholders filled in]
```

## Tips for Best Results
- [Tip 1]
- [Tip 2]
- [Tip 3]

## Performance Notes
[Notes about which GAIA models this works best with and why]
[Any specific optimization tips for NPU+iGPU execution]
```

## Testing Guidelines

Before submitting a prompt, please test it with at least two different GAIA models, preferably:
1. One model in NPU+iGPU hybrid mode
2. One model in generic mode

Document any differences in performance or output quality.

## Optimization Principles

When designing prompts for GAIA, consider these optimization principles:

1. **Token Efficiency** - Keep prompts concise but thorough
2. **Context Management** - Be mindful of limited context windows in quantized models 
3. **Explicit Instructions** - Be clear and specific to reduce the need for clarifications
4. **Model-Specific Adjustments** - Note which models perform best with your prompt

## Code of Conduct

- Be respectful and constructive in all interactions
- Welcome contributions from everyone regardless of experience level
- Focus on the quality and usefulness of prompts for GAIA users
- Provide constructive feedback on pull requests

## Licensing

By contributing to this repository, you agree that your contributions will be licensed under the same [MIT License](LICENSE) that covers the project.

Thank you for helping make GAIA more useful for everyone!