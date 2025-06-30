# Agent Guidelines for Prompt Creation

This document outlines the conventions and best practices for creating new prompts within this project. Adhering to these guidelines ensures consistency, clarity, and ease of use for all agents.

## 1. Input Requirements (Verbosity)

When designing a prompt, ensure that it is **verbose and comprehensive**. The goal is to elicit as much relevant information as possible from the user to enable a thorough and accurate response.

*   **Be Explicit:** Clearly state what information is required for each section.
*   **Provide Examples:** Include examples for data types, formats, or expected values where appropriate (e.g., `VARCHAR(255)`, `INT`, `YYYY-MM-DD`).
*   **Ask Open-Ended Questions:** Encourage detailed responses rather than simple yes/no answers.
*   **Cover All Angles:** Think about all potential aspects or considerations related to the task the prompt is addressing and include sections for them.
*   **Optional Sections:** Clearly mark sections as "(Optional)" if the information is not strictly necessary but would be beneficial.

## 2. Output Formatting

The output of the prompt should be structured and easy to parse. Use Markdown for clear readability.

*   **Headings:** Use Markdown headings (`#`, `##`, `###`) to organize the prompt into logical sections.
*   **Lists:** Use bullet points (`*` or `-`) or numbered lists (`1.`, `2.`) for enumerating items or options.
*   **Code Blocks:** Use fenced code blocks (``````) for any examples of code, data structures, or specific formats. Always specify the language if applicable.
*   **Bold/Italics:** Use bold (`**text**`) or italics (`*text*`) sparingly for emphasis.

## 3. File Naming Conventions

All prompt files should follow a consistent naming convention to ensure they are easily discoverable and understandable.

*   **Format:** `snake_case`
*   **Extension:** `.md`
*   **Content Description:** The name should clearly and concisely describe the purpose of the prompt.
*   **Examples:**
    *   `code_review_prompt.md`
    *   `dependency_audit_prompt.md`
    *   `generate_unit_tests_prompt.md`
    *   `database_schema_design_prompt.md`
    *   `code_explanation_prompt.md`
