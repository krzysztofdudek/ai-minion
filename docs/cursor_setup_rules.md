# Using `prompt.md` with Cursor: `.cursorrules` for General Guidance

This document explains how to use a `.cursorrules` file in your project to provide Cursor with general, repository-level AI instructions. This method is suitable for concise, high-level directives and can complement other methods of using the more detailed `prompt.md`.

## Method: Using `.cursorrules` for High-Level Instructions

Cursor's `.cursorrules` file allows you to set persistent guidelines for its AI features (Chat, Edit, Agent mode) across your project.

1.  **Create/Update `.cursorrules` File:**
    *   In the root of your project, create a file named `.cursorrules` if it doesn't already exist.
    *   Add concise, high-level instructions to this file. The full `prompt.md` is generally too extensive for `.cursorrules`; instead, focus on core principles or references.

    **Example `.cursorrules` content:**

    ```
    # General AI Guidelines for this Project

    When a complex task is initiated that requires a systematic, multi-step approach, I may provide a detailed operational prompt (like `prompt.md` from this repository) directly in the chat or via a Custom Mode. Please prioritize such detailed instructions when given.

    Core principles for all general tasks:
    - Prioritize understanding requirements fully. Ask clarifying questions proactively.
    - For significant code changes, consider outlining a plan or approach first.
    - Emphasize security, code quality, and testability.
    - When modifying existing code, adopt an "extend by default" philosophy.

    For general assistance, focus on providing clear, accurate, and efficient solutions.
    ```

## Purpose of this Method

*   **General Context:** Provides Cursor with persistent, high-level context about your project or preferred ways of working for everyday, simpler tasks.
*   **Conciseness:** `.cursorrules` is best for brief instructions that don't overly constrain the AI for all interactions.
*   **Complementary Guidance:** This method is most effective when used to set a general tone or highlight key considerations. It can inform the AI's behavior during routine tasks and make it more receptive when you invoke the full `prompt.md` persona via:
    *   Direct pasting or `@` mention (see `cursor_setup_direct_prompting.md`).
    *   A dedicated Custom Mode (see `cursor_setup_custom_mode.md`).

Using `.cursorrules` for general guidance helps create a baseline for AI interactions, which can then be augmented with more specific and detailed instructions from `prompt.md` as needed. 