# Code Generation Prompts

These prompts are designed to help GAIA models generate high-quality code. They're optimized for the processing constraints of NPU+iGPU execution while still producing useful technical output.

## Simple Function Generator

### Prompt Template
```
Create a [LANGUAGE] function that accomplishes the following task:

Task: [DESCRIPTION_OF_TASK]

Requirements:
- The function should be named: [FUNCTION_NAME]
- Input parameters: [PARAMETERS]
- Expected output: [OUTPUT]
- Include basic error handling
- Add brief comments explaining the logic

Please provide only the code with minimal explanation.
```

### Example

```
Create a Python function that accomplishes the following task:

Task: Convert a temperature between Celsius and Fahrenheit

Requirements:
- The function should be named: convert_temperature
- Input parameters: temperature (float), unit (string: 'C' or 'F')
- Expected output: The converted temperature as a float
- Include basic error handling
- Add brief comments explaining the logic

Please provide only the code with minimal explanation.
```

### Tips for Best Results
- Be very specific about the expected inputs and outputs
- Limit the scope to a single function for better results
- Specify which language you want the code in
- Works best with Phi-3.5 Mini Instruct and Phi-3 Mini Instruct models

## Algorithm Implementation

### Prompt Template
```
Implement the [ALGORITHM_NAME] algorithm in [LANGUAGE]. The implementation should:

1. Handle inputs: [INPUT_DESCRIPTION]
2. Follow these constraints: [CONSTRAINTS]
3. Be optimized for [OPTIMIZATION_GOAL]
4. Include comments explaining key steps

Please provide only the code implementation.
```

### Example

```
Implement the binary search algorithm in JavaScript. The implementation should:

1. Handle inputs: A sorted array of numbers and a target value to find
2. Follow these constraints: O(log n) time complexity, iterative approach (no recursion)
3. Be optimized for readability
4. Include comments explaining key steps

Please provide only the code implementation.
```

### Performance Notes
This prompt works well on NPU+iGPU hardware because:
- It constrains the problem to a specific algorithm
- It provides clear expectations about the implementation approach
- It reduces token usage by focusing on code only

Optimal models: Phi-3.5 Mini Instruct, Llama-3.2 3B Instruct

## Code Refactoring

### Prompt Template
```
Refactor the following [LANGUAGE] code to improve [ASPECT_TO_IMPROVE]:

```
[ORIGINAL_CODE]
```

Focus specifically on:
- [FOCUS_POINT_1]
- [FOCUS_POINT_2]
- [FOCUS_POINT_3]

Provide only the refactored code without explanations.
```

### Example

```
Refactor the following Python code to improve performance:

```python
def find_duplicates(numbers):
    duplicates = []
    for i in range(len(numbers)):
        for j in range(i+1, len(numbers)):
            if numbers[i] == numbers[j] and numbers[i] not in duplicates:
                duplicates.append(numbers[i])
    return duplicates
```

Focus specifically on:
- Reducing the time complexity
- Avoiding nested loops
- Using appropriate data structures

Provide only the refactored code without explanations.
```

### Performance Notes
This prompt template works effectively on GAIA models because:
- It provides a complete, contained problem
- It has specific focus points for the refactoring
- It constrains the output to just code, reducing token usage

For larger code blocks, consider breaking them down into smaller segments if the model struggles with context management.

Optimal models: Llama-2 7B Chat, Mistral 7B Instruct