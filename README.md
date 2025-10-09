# Use of AI for Literature Review

**A 5-Day Intensive Course on AI-Assisted Research**

*IAEA Laboratories, Seibersdorf, Austria | October 2025*

## Course Overview

This hands-on course explores how to effectively integrate AI and Large Language Models (LLMs) into literature review workflows. Rather than treating AI as a magic solution, we focus on developing a methodical, ethical approach that keeps researchers in control while enhancing their capabilities.

### Philosophy: AI as a Learning Companion

- AI as a partner for better and faster learning, not a replacement for critical thinking
- Focus on methodology over specific tools
- Emphasis on evaluation, reliability, and maintaining research quality

## What You'll Learn

### Core Topics
- **LLM Fundamentals**: Understanding how these systems work and why they sometimes fail
- **Advanced Prompt Engineering**: Building effective prompts through systematic iteration
- **Evaluation & Quality Control**: Systematic approaches to assess AI outputs using open/axial coding and LLM-as-judge methodology
- **Research Workflows**: Organizing AI-assisted literature reviews and multi-paper synthesis
- **IP-Aware Approaches**: Respecting copyright while leveraging AI capabilities
- **Tools & Platforms**: Understanding different AI tools and their appropriate use cases
- **Ethics & Detection**: Navigating journal policies and AI detection challenges

## 5-Day Schedule

### Day 1: Foundations & Initial Experience
**Morning:**
- Course philosophy and what makes AI effective for research
- Tools exploration: "Who's using what?" (collaborative session)

**Afternoon:**
- First hands-on: Try paper extraction yourself (authentic struggle)
- Debrief and introduction to the Three Gulfs Model
- Collaborative discussion: expectations, concerns, and ethical considerations

### Day 2: Prompt Engineering Fundamentals
**Morning:**
- How LLMs are trained: understanding capabilities and limitations
- The seven building blocks of effective prompts

**Afternoon:**
- Iterative hands-on: Build a paper extraction prompt step-by-step
- Group comparison and discussion of different approaches

### Day 3: Evaluation Methodology
**Morning:**
- Evaluation methodology: open coding, axial coding, and LLM-as-judge concepts
- Hands-on: Systematically evaluate your Day 2 prompts

**Afternoon:**
- Live axial coding session: analyzing patterns from shared observations
- Key insights and preparing for synthesis work

### Day 4: Synthesis & Hands-On Practice
**Morning:**
- Multi-paper synthesis prompt building with IP constraints
- Hands-on: Apply and refine synthesis prompts with real papers

**Afternoon:**
- Demo: 20-paper literature review workflow in SolveIt
- Discussion: "What would you need from your tools to do this?"

### Day 5: Real-World Applications, Ethics & Future
**Morning:**
- Real-world case studies:
  - MARIS RAG system (Monaco): IP-aware synthesis at scale
  - IOM report evaluation: Multi-step prompts in action
- Journal policies on AI use

**Afternoon:**
- Hands-on: AI detection challenge (build your own detector)
- Collaborative framework synthesis
- Individual consultation planning

## Course Approach

- **Experience First**: Start with authentic challenges before introducing frameworks
- **Iterative Learning**: Build complexity gradually through hands-on cycles
- **Collaborative**: Shared documentation and group learning throughout
- **Methodological**: Develop systematic approaches, not ad-hoc tool use
- **Honest**: Acknowledge limitations and share real development processes

## Key Frameworks

### The Three Gulfs Model
Understanding AI system challenges through three fundamental gaps:
- **Gulf of Comprehension**: You ↔ Your Data
- **Gulf of Specification**: You ↔ AI Pipeline
- **Gulf of Generalization**: Your Data ↔ AI Pipeline

### The Seven Building Blocks of Prompting
1. Role and Objective
2. Instructions / Response Rules
3. Context
4. Examples (Few-shot)
5. Reasoning Steps (Chain-of-thought)
6. Output Formatting
7. Delimiters

## About the Instructor

**Franck Albinet**  
Independent Data Science & AI Consultant  
Email: franckalbinet@gmail.com

## Prerequisites

- Basic familiarity with research and literature review processes
- No prior AI or programming experience required
- Bring your own research questions and papers to work with
- Access to at least one AI tool (ChatGPT, Claude, Copilot, etc.)

## What You'll Take Away

- A systematic methodology for AI-assisted literature review
- Practical experience building and evaluating prompts
- Understanding of evaluation approaches (open/axial coding, LLM-as-judge)
- Knowledge of IP-aware synthesis techniques
- Ethical framework for AI use in research
- Your own refined prompts for paper extraction and synthesis
- Individual consultation opportunities (6 additional days available)

## Materials Provided

- Prompt engineering fundamentals guide
- Hands-on session instructions
- Shared documentation templates
- Example prompts and case studies
- Reference materials on journal policies and ethics

## Target Audience

Researchers, graduate students, and professionals who want to:
- Enhance their literature review capabilities with AI
- Understand AI tools beyond the hype
- Develop reliable, ethical approaches to AI-assisted research
- Stay in control while leveraging AI capabilities
- Learn systematic evaluation methodologies

## Collaborative Learning

Throughout the course, participants contribute to shared documentation:
- Open coding observations from hands-on exercises
- Pain points and solutions
- Ethical concerns and guidelines
- Best practices and recommendations

This collective knowledge will be synthesized into a collaborative framework and may contribute to future publications on AI-assisted research methodologies.

## Presentations

Available in the `presentations/` directory [wip]:
- Course scope and philosophy
- LLM training fundamentals
- Prompt engineering principles
- The Three Gulfs Model
- Evaluation methodologies

## Getting Started with Quarto/Reveal.js

This course uses Quarto with Reveal.js for interactive presentations.

### Setup
To use the same template as the course materials:
```bash
quarto use template grantmcdermott/quarto-revealjs-clean-demo
```

### Viewing Presentations
To render and view a presentation file:
```bash
quarto preview my-presentation.qmd
```
This will open the presentation in your local browser with live reload.

### Converting to PDF
Built-in print stylesheet (recommended): Quarto reveal.js presentations can be exported to PDF via a special print stylesheet. Simply add `?print-pdf` to your presentation URL, open the browser print dialog (Ctrl+P), change destination to "Save as PDF", set layout to landscape, margins to none, and enable background graphics.

---

*Course materials updated October 2025. For questions or early access inquiries, contact the instructor.*