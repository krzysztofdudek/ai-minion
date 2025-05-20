# Using `prompt.md` with Cursor: Custom Mode Setup

This document outlines a method to integrate the `prompt.md` AI worker persona with Cursor by creating a dedicated "Custom Mode". This provides a more integrated experience, making it easy to switch to the detailed operational mode without repeatedly pasting the prompt.

## Method: Creating a "Minion" Custom Mode

For a seamless experience, you can create a dedicated Custom Mode in Cursor to embody the "AI Worker" persona defined in `prompt.md`.

As per the [Cursor Custom Modes documentation](https://docs.cursor.com/chat/custom-modes), you can create a new mode with specific tools and instructions.

**Steps to Create a "Minion" Custom Mode:**

1.  **Enable Custom Modes:** If you haven't already, enable Custom Modes in Cursor settings: `Settings` → `Features` → `Chat` → `Custom modes`.
2.  **Open the Mode Menu:** In the Cursor chat interface, click on the current mode (e.g., "Agent") to open the mode selection menu.
3.  **Add Custom Mode:** Select the option to "Add custom mode" (often a `+` icon or similar, as shown in the UI for creating new modes).
    
    *(Refer to the visual layout for creating a new mode, where you can configure its name, icon, tools, and instructions.)*

4.  **Configure the Mode:**
    *   **Enter a name:** Call it "Minion", "AI Worker", or a name of your choice.
    *   **Icon (Optional):** Choose an icon if you like.
    *   **Model:** Select your preferred model (e.g., Claude 3.5 Sonnet, GPT-4o, etc.).
    *   **Tools:** Enable the tools you want this mode to have access to. For the full `prompt.md` experience, you'd likely want most, if not all, tools enabled (Search, Edit, Run Commands, etc.). The `prompt.md` itself guides the AI on *how* and *when* to consider using tools.
    *   **Auto-apply edits / Auto-run / Auto-fix errors:** Configure these to your preference. The `prompt.md` emphasizes explicit approval steps, so you might want to keep auto-apply and auto-run off initially, or configure them cautiously.
    *   **Add custom instructions:** This is the crucial step. 
        1.  Open the `prompt.md` file in this repository.
        2.  Copy its **entire content**.
        3.  Paste the entire content of `prompt.md` into the "Add custom instructions" field for your new "Minion" mode.

5.  **Save the Mode:** Click "Done" or the equivalent save button.

**Using Your New "Minion" Custom Mode:**

*   Once created, you can select your "Minion" mode from the mode selection dropdown in the chat interface.
*   When this mode is active, Cursor will automatically use the full `prompt.md` content as its guiding instructions for all interactions within that chat session.

## Benefits of this Method

*   **Convenience:** Easily switch to the detailed AI persona without manual copy-pasting for each complex task.
*   **Consistency:** Ensures the AI always operates under the full `prompt.md` guidelines when this mode is active.
*   **Tailored Toolset:** You can pre-configure the exact set of tools available to the "Minion" persona.

This method provides a powerful and convenient way to integrate the comprehensive `prompt.md` directly into your Cursor workflow for specialized tasks, allowing for quick activation of the full AI Worker persona. 