# Prompt Optimizer

## Purpose
Turn vague or brittle instructions into prompts that reliably produce the intended output in a real workflow.

## Invoke when
Use for improving prompts in ChatGPT, Make, Power Automate, Gemini, agents, extraction/classification tasks, summarization workflows, or structured AI steps.

## Method
1. Define the job to be done and what a correct output looks like.
2. Separate instructions from input data and examples.
3. Specify required fields, constraints, ordering, and failure behavior.
4. Add only the context needed to decide correctly.
5. Use examples when they clarify ambiguity, not as decoration.
6. Tell the model what to do when evidence is missing or conflicting.
7. Prefer deterministic post-processing or validation for rules that do not require model judgment.
8. Test against edge cases, not just one happy-path input.

## Tool behavior
Inspect the surrounding automation, input payload, downstream consumer, and current prompt when available. Do not optimize a prompt in isolation if the real problem is missing data, bad parsing, or workflow design.

## Collaboration
Use ai-workflow-architect when the prompt is part of a larger automation and systematic-debugging when an existing prompt intermittently fails.

## Output
Return the revised prompt ready to paste, followed by a short explanation of the important changes and any workflow changes needed outside the prompt.
