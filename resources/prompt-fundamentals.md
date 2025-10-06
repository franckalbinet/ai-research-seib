# Prompting Fundamentals 

Prompting is the act of crafting the input text given to the LLM to elicit the desired output. 

A well-structured prompt typically includes several key pieces: 

## 1. Role and Objective 

Clearly define the persona or role the LLM should adopt and its overall goal. This helps set the stage for the desired behavior. 

Example: `"You are an expert technical writer tasked with explaining complex AI concepts to a non-technical audience."`

## 2. Instructions / Response Rules 

This is a core component, providing clear, specific, and unambiguous directives for the task. For newer models that interpret instructions literally, it's vital to be explicit about what to do and what not to do. 

Use bullet points or numbered lists for clarity, especially for multiple instructions. 

Example: 

```
- "Summarize the following research paper abstract." 

- "The summary must be exactly three sentences long." 

- "Avoid using technical jargon above a high-school reading level." 

- "Do not include any personal opinions or interpretations." 
```

For complex instruction sets, consider breaking them into sub-categories (e.g., ### Tone and Style, ### Information to Exclude). 

## 3. Context 

The relevant background information, data, or text the LLM needs to perform the task. This could be a customer email, a document to summarize, a code snippet to debug, or user dialogue history. 

Example: `"[Insert the full text of the customer email here]"`

When providing multiple documents or long context, clear delimiters are crucial (see point 7). 

## 4. Examples (Few-Shot Prompting) 

Provide one or more examples of desired input-output pairs. This is highly effective for guiding the model towards the correct format, style, and level of detail. Examples can also clarify nuanced instructions or demonstrate complex tool usage. 

Example: `Showing one or two sample emails and their ideal bullet-point action items, or a sample input and the correctly formatted JSON output.`

Ensure that any important behavior demonstrated in your examples is also explicitly stated in your rules/instructions. 

## 5. Reasoning Steps (Inducing Chain-of-Thought) 

For more complex problems, you can instruct the model to "think step by step" or outline a specific reasoning process. This technique, often called Chain-of-Thought (CoT) prompting, encourages the model to break down the problem and can lead to more accurate and well-reasoned outputs, even for models not explicitly trained for internal reasoning. 

Example: `"Before generating the summary, first identify the main hypothesis, then list the key supporting evidence, and finally explain the primary conclusion. Then, write the summary."`

## 6. Output Formatting Constraints 

Explicitly define the desired structure, format, or constraints for the LLM's response. This is critical for programmatic use of the output. 

Example: 

```
"Respond using only JSON format with the following keys: sender_name (string), main_issue (string), and suggested_action_items (array of strings)." 

or

"Ensure your response is a single paragraph and ends with a question to the user." 
```

## 7. Delimiters and Structure 

Use clear delimiters (e.g., Markdown section headers like ### Instructions ###, triple backticks for code/text blocks, XML tags) to separate different parts of your prompt, such as instructions, context, and examples. This helps the model understand the distinct components of your input, especially in long or complex prompts. 

A general recommended prompt organization, especially for complex prompts or long contexts, is to place overarching instructions or role definitions at the beginning, followed by context and examples, and potentially reiterating key instructions or output format requirements at the end. 

The goal of effective prompting is to make our intent as explicit and unambiguous as possible for the model. What seems obvious to us might be unclear to the LLM. E.g., is "summarize" meant to be extractive or abstractive? Should the tone be formal or informal? Precision in our prompt is key. 

However, finding the perfect prompt is rarely immediate. It's an iterative process. We'll write a prompt, test it on various inputs, analyze the outputs (using evaluation techniques we'll discuss in future sections), identify failure modes, and refine the prompt accordingly. 

*Note: There are many tools that will write prompts for you and optimize them. It's important that you avoid these in the beginning stages of development, as writing the prompt forces you to externalize your specification and clarify your thinking. People who delegate prompt writing to a black box too aggressively struggle to fully understand their failure modes. After you have some reps with looking at your data, you can introduce these tools (but do so carefully).*

An iterative refinement process hinges on having clear ways to judge whether the output is good or bad. This brings us to the concept of evaluation metrics. 

 