# Using `prompt.md` with GitHub Copilot: `.github/copilot-instructions.md` for General Guidance

This document explains how to use the `.github/copilot-instructions.md` file to provide general, repository-level guidance to GitHub Copilot. This method is suitable for concise instructions and can complement the direct pasting of the full `prompt.md` for complex tasks.

## Method: Using `.github/copilot-instructions.md`

GitHub Copilot's custom instructions file (`.github/copilot-instructions.md`) is designed for short, high-level directives that apply to most interactions within the repository.

1.  **Create/Update `.github/copilot-instructions.md`**:
    *   If it doesn't exist, create a file named `copilot-instructions.md` inside a `.github` directory in the root of your repository.
    *   Add concise instructions to this file. Instead of pasting the entire `prompt.md` (which is too long for this file), include high-level principles or a reference to it.

    **Example `.github/copilot-instructions.md` content:**

    ```markdown
    When I assign a complex task that requires a systematic approach, I may provide a detailed persona and workflow guide (like `prompt.md` in this repository) directly in the chat. Please adhere to that detailed guide for such tasks.

    For all interactions, consider these key principles:
    - Analyze requirements thoroughly.
    - Ask clarifying questions before making assumptions.
    - Propose a clear plan for complex changes.
    - Focus on security, testability, and verifiability.
    - If working with code, assume an "extend by default" approach for existing systems.

    For general coding assistance, prioritize clarity, efficiency, and adherence to best practices.
    ```

## Purpose of this Method

*   **General Context:** Provides Copilot with persistent, high-level context about your project or preferred ways of working for everyday, simpler tasks.
*   **Conciseness:** Aligns with Copilot's design for brief custom instructions. The full `prompt.md` is too extensive for this file.
*   **Complementary:** This method is best used in conjunction with directly pasting the full `prompt.md` (see `copilot_setup_direct_prompting.md`) when the comprehensive "AI Minion" persona is required for a specific complex task. The `.copilot-instructions.md` can remind Copilot to be receptive to such detailed, task-specific prompts.

By using `.github/copilot-instructions.md` for general hints and direct pasting for the full persona, you can effectively tailor GitHub Copilot's behavior. 