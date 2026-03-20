# The LLM Council for Roam Research

Accelerate the evolution of an idea in RoamResearch by employing Andrej Karpathy's LLM Council concept.

## Features
- **Multi-Model Support:** The council currently allows you to compare up to 4 AI models simultaneously per run.
- **Customizable Council:** You can substitute the default models in the SmartBlock code with any models you prefer (e.g., from OpenRouter, OpenAI, Anthropic, Gemini, etc.).
- **Graph Context Integration:** The SmartBlock allows you to select and append existing Roam pages as direct context for the AI council to consider.

## How to Install
1. Open your Roam graph.
2. Copy the complete block structure from `llm-council.md` into your graph.
3. Ensure RoamDepot extensions **SmartBlocks** and **Live AI** are installed and active.

## Customizing your Models
In the `llm-council.md` code (or within your Roam graph after pasting), locate the lines containing `%INPUT:Model #1...%` through `%INPUT:Model #4...%`. 
You can replace the model tags (e.g., `openRouter/anthropic/claude-sonnet-4.6`) with your preferred model string IDs. 

## How to Use
1. In your DNP or project page, write out your conjecture, idea, or problem. This can be an outline with 'as many' child blocks.
2. On the parent block, type `;;` and call the template: **👥 The Council**.
3. This creates a nested button structure. Click the button to trigger the workflow.

### The Breakdown
- **Phase 1: The Council Responds (Conjecture)**
  Fires your prompt at up to 4 models in parallel. Each model provides an independent answer without seeing the others' responses.
- **Phase 2: The Peer Review Board (Criticism)**
  Models are assigned to critique a different model's response. They evaluate logical consistency, unexamined assumptions, and argument robustness. 
- **Phase 3: The Verdict**
  The chair model reviews the conjectures and criticisms, attempting to synthesize the correct path forward.

> **Note:**__You are the average of the LLMs you hang out with!__