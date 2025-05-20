# Using `prompt.md` with Cursor: Direct Prompting (Simplest Method)

This document outlines the simplest way to use the full `prompt.md` AI minion persona with Cursor by directly pasting its content into the chat or using the `@` mention feature.

## Method: Direct Pasting or `@` Mention of `prompt.md`

This approach is straightforward and ensures Cursor receives the complete set of instructions for a specific, complex task when you need it to adopt the full "AI Minion" persona.

1.  **Open `prompt.md`:**
    *   Locate and open the `prompt.md` file from this repository.

2.  **Copy Content (for pasting method):**
    *   Select and copy the **entire content** of the `prompt.md` file.

3.  **Provide to Cursor Chat:**
    *   **Option A: Pasting:**
        1.  Open a new chat session with Cursor.
        2.  Paste the copied content directly into the chat input.
        3.  Immediately follow the pasted prompt with your specific task request.
    *   **Option B: `@` Mention:**
        1.  In the Cursor chat input, type `@prompt.md`. This will include the content of `prompt.md` as context for the current interaction.
        2.  Follow this with your specific task request.

**Example Interaction (Pasting):**

> **User:** (Pastes entire content of `prompt.md`)
>
> **User:** Now, acting as the AI Minion defined above, I need you to analyze the `PaymentGateway` interface and propose a plan to integrate a new payment provider.

**Example Interaction (`@` Mention):**

> **User:** @prompt.md
> Please act as the AI Minion defined in the referenced prompt. I need you to design the database schema for a new inventory management system.

## When to Use This Method

*   **Simplicity:** This is the most direct way to provide the full persona to Cursor.
*   **Specific Complex Tasks:** Ideal when you have a substantial task that would benefit from the detailed workflow and principles outlined in `prompt.md`.
*   **Full Control:** Ensures that for the current interaction, Cursor is operating under the complete set of instructions from `prompt.md`.

This direct prompting method can be used independently or in conjunction with general guidance provided via a `.cursorrules` file (see `cursor_setup_rules.md`) or a more integrated Custom Mode (see `cursor_setup_custom_mode.md`). 