# Task Instructions

## Tactic 1: Use delimiters to clearly indicate distinct parts of the input
Delimiters can be anything like: ```, """, < >, `<tag> </tag>`, `:`

## Tactic 2: Ask for a structured output
Output formats: JSON, HTML

Prompt:
You will be provided with text delimited by triple quotes. 
If it contains a sequence of instructions, rewrite those instructions in the following format:

Step 1 - ...
Step 2 - …
…
Step N - …

If the text does not contain a sequence of instructions, then simply write "No steps provided."

## Tactic 3: Ask the model to check whether conditions are satisfied

## Tactic 4: "Few-shot" prompting
Prompt:
Your task is to answer in a consistent style.

<child>: Teach me about patience.

<grandparent>: The river that carves the deepest valley flows from a modest spring; the grandest symphony originates from a single note; the most intricate tapestry begins with a solitary thread.

<child>: Teach me about resilience.

# Principle 2: Give the model time to “think”

## Tactic 1: Specify the steps required to complete a task
Prompt:
Perform the following actions: 
1 - Summarize the following text delimited by triple backticks with 1 sentence.
2 - Translate the summary into French.
3 - List each name in the French summary.
4 - Output a JSON object that contains the following keys: french_summary, num_names.

Separate your answers with line breaks.

## Tactic 2: Instruct the model to work out its own solution before rushing to a conclusion
Prompt:
Your task is to determine if the student's solution is correct or not.
To solve the problem, do the following:
- First, work out your own solution to the problem including the final total. 
- Then compare your solution to the student's solution and evaluate if the student's solution is correct or not. 
- Don't decide if the student's solution is correct until you have done the problem yourself.

Use the following format:
Question:
## Model Limitations: Hallucinations
Reducing hallucinations can be done by 
First find relevant information 
Then answer the questions 
Based on the relevant information 

