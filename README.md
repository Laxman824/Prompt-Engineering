# ChatGPT Prompting Guide

## Principles for Effective Prompting

### Principle 1: Clarity and Specificity
- Write clear and specific instructions.
- Use delimiters to clearly indicate distinct parts of the input.

### Principle 2: Allow Time to "Think"
- Give the model time to process and generate responses.
- Specify the steps required to complete a task.

## Tactics for Structured Output

### Tactic 1: Delimiters
- Use delimiters like triple backticks or tags to separate different parts of the prompt.

### Tactic 2: Structured Responses
- Request outputs in structured formats like JSON or HTML.

### Tactic 3: Condition Checking
- Ask the model to verify if certain conditions are met before proceeding.

### Tactic 4: Few-Shot Prompting
- Provide examples of the desired output style or structure.

## Steps to Craft Your Prompt

1. **Define the Task Clearly**: Start by clearly stating what you need from the model.

2. **Use Delimiters**: Separate instructions, inputs, and expected outputs with clear delimiters.

3. **Request Structured Output**: If you need a specific format, instruct the model accordingly.

4. **Check Conditions**: Include a step where the model checks if certain conditions are satisfied.

5. **Provide Examples**: Use few-shot prompting to give the model examples of the desired output.

6. **Allow for "Thinking"**: Structure your prompt to let the model "think" through the problem.

7. **Avoid Rushing**: Instruct the model to work out its own solution before providing an answer.

8. **Handle Hallucinations**: Instruct the model to base its responses on relevant information.

## Example Prompt

```plaintext
Your task is to summarize the provided text and translate it into French. Check if any names are mentioned and list them. Finally, output a JSON object with the summary and the number of names.

Text to Summarize:
<Your text here>

Instructions:
1. Summarize the text in one sentence.
2. Translate the summary into French.
3. List any names mentioned in the summary.
4. Output a JSON object with keys: 'french_summary' and 'num_names'.

Format your response as follows:
Summary: <Your summary here>
Translation: <Your translation here>
Names: <List of names here>
Output JSON: <Your JSON object here>
