# Session 2C: Hands-On Guide - Building Your Paper Extraction Prompt

[LINKED TO SHARED DOC](https://docs.google.com/document/d/15vb-eCd08p466UT5ifweicVNK1B1C-tu1zfC_TTwHSI/edit?usp=sharing)

## Overview
This guide accompanies the Day 2B presentation. You'll build a paper extraction prompt iteratively, adding one building block at a time.

**What you need:**
- A scientific paper from your domain (PDF or text)
- Access to your AI tool of choice
- A document to track your prompt versions and observations
- The `prompt_fundamentals.md` reference guide

**Goal:** By the end, you'll have a working paper extraction prompt tailored to your needs.

---

## Cycle 1: Basic Instruction (15 minutes)

### Your Task
Create a simple, instruction-only prompt for paper extraction.

### Instructions
1. Write a basic prompt that tells the AI what to do
2. Keep it simple - just the core instruction
3. Test it on your paper
4. Note what you get

### Example Starting Points
- "Summarize this scientific paper."
- "Extract key information from this research paper."
- "Provide an overview of the main findings in this paper."

### What to Observe
- What format did the output take?
- What information was included/excluded?
- Was it consistent if you ran it twice?
- What's missing that you need?

**Write down your observations** - we'll discuss as a group.

---

## Cycle 2: Add Role & Objective (15 minutes)

### Your Task
Enhance your Cycle 1 prompt by adding a role and objective.

### Building Blocks to Add

**Role:** Who is the AI?
- Examples: "You are a scientific literature specialist..."
- "You are an expert in [your domain] research..."
- "You are a research assistant helping with literature review..."

**Objective:** What's the overall goal?
- Examples: "...to create structured summaries for literature review"
- "...to extract key information for research synthesis"
- "...to support systematic literature analysis"

### Template Structure
```
**Role:** [Define who the AI is]

**Objective:** [State the overall goal]

**Task:** [Your instruction from Cycle 1]

[Your paper text]
```

### What to Observe
- Did the tone or style change?
- Is the output more focused?
- Does it better match your needs?
- What still needs improvement?

---

## Cycle 3: Add Output Formatting (20 minutes)

### Your Task
Add explicit formatting requirements to specify the structure you want.

### Think About
- What sections do you need?
- Bullet points or paragraphs?
- How much detail in each section?
- Any length constraints?
- What must be included vs. optional?

### Example Format Requirements
```
**Format required:**
- Title and full citation
- Abstract (original, verbatim)
- Research question/objective
- Methodology summary (3-5 bullet points)
- Main results with statistics
- Key conclusions
- Figures and tables mentioned (with brief descriptions)

**Constraints:**
- Use bullet points for summaries
- Include all quantitative results
- Maximum 2000 words
```

### Template Structure
```
**Role:** [From Cycle 2]

**Objective:** [From Cycle 2]

**Output Format:**
[List your required sections and structure]

**Task:** [Your instruction]

[Your paper text]
```

### What to Observe
- Is the structure now consistent?
- Does it include everything you need?
- Is anything still missing or unclear?
- Could you use this format for multiple papers?

---

## Cycle 4: Add Context (20 minutes)

### Your Task
Add context about how the output will be used and what to prioritize.

### Think About
- What will you do with these summaries?
- What information is most important for your work?
- What should be emphasized vs. de-emphasized?
- What should be excluded?
- Any domain-specific requirements?

### Example Context
```
**Context:** 
These summaries will be used for:
- Comparing methodologies across multiple studies
- Identifying research gaps in [specific area]
- Synthesizing findings for a literature review

**Priorities:**
- Quantitative results with statistical measures
- Sample sizes and study populations
- Methodological approaches that enable comparison
- Limitations acknowledged by authors

**Exclude:**
- Author affiliations and biographical information
- Acknowledgments and funding details
- Complete reference lists
```

### Optional: Add Examples
If you want to show exactly what you're looking for, include 1-2 example extractions.

### Template Structure
```
**Role:** [From previous cycles]

**Objective:** [From previous cycles]

**Context:**
[What will this be used for?]
[What should be prioritized?]
[What should be excluded?]

**Output Format:**
[From Cycle 3]

**Task:** [Your instruction]

[Your paper text]
```

### What to Observe
- Is the output more focused on what matters to you?
- Does it exclude irrelevant information?
- Is it now useful for your actual research needs?

---

## Cycle 5: Advanced Features (Optional, 15-20 minutes)

### Your Task
If needed, add reasoning steps or better organization with delimiters.

### Reasoning Steps
Add if you want the AI to:
- Analyze or evaluate (not just extract)
- Show its thinking process
- Make comparisons or judgments

**Example:**
```
Before generating the summary:
1. Identify the main research question
2. Determine the study design and methodology
3. Extract key quantitative results
4. Note any limitations mentioned
Then provide the structured summary.
```

### Delimiters
Use markers to organize complex prompts:

**Example:**
```
### ROLE AND OBJECTIVE ###
[Your role and objective]

### CONTEXT AND PRIORITIES ###
[Your context]

### OUTPUT FORMAT ###
[Your format requirements]

### PAPER TO ANALYZE ###
[Your paper text]
```

### What to Observe
- Does adding reasoning improve quality?
- Do delimiters make the prompt clearer?
- Is this level of complexity necessary for your task?

---

## Final Refinement (10 minutes)

### Your Task
Review your complete prompt and refine.

### Questions to Ask
- Does it produce what you need?
- Is anything unclear or ambiguous?
- Would it work on different types of papers in your domain?
- What would you change based on testing?

### Save Your Work
Keep your final prompt version - you'll use it tomorrow for evaluation exercises.

---

## Reflection Questions

**For the shared doc:**
- Which building blocks made the biggest difference?
- What surprised you during this process?
- What challenges remain with your prompt?
- How would you describe "good enough" for your needs?

---

## Reference

**Building blocks covered:**
1. ✅ Instructions - What to do
2. ✅ Role & Objective - Who and why
3. ✅ Output Formatting - Structure and constraints
4. ✅ Context - Priorities and usage
5. ⚡ Examples - Sample outputs (optional)
6. ⚡ Reasoning Steps - Chain-of-thought (optional)
7. ⚡ Delimiters - Organization (optional)

**Full reference:** See [resources/prompt_fundamentals.md](resources/prompt_fundamentals.md) for detailed explanations of each building block.