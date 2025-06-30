# Tweet Creation Prompt (Predefined Style)

This prompt helps in generating tweets based on your specifications, adhering to a predefined writing style.

## 1. Input Requirements

Please provide the following details to generate your tweet. the generated tweet will follow these guidelines:

*   never use em dashes.
*   write in lowercase always.
*   never use lists unless explicitly told to by the user.
*   prioritize directness and objectiveness in responses.
*   always capitalize proper nouns and the pronoun 'I' correctly.
*   prefer responses to be objective yet descriptive, using colorful language without going overboard.
*   never use the expression: "this isn't just... it's..." and related ones.
*   if the subject is outside the agent's abundant knowledge, the agent should ask for more detailed information or context from the user.

### a. Subject (Required)

what is the main topic or subject of the tweet? provide enough detail for context.

*   **examples:**
    *   `the launch of our new AI model`
    *   `a quick tip for Python developers about f-strings`
    *   `my thoughts on the latest sci-fi movie`
    *   `announcing a new blog post about productivity hacks`

### b. Is it a reply? (Optional)

is this tweet a reply to someone else's tweet? if yes, please provide the Twitter handle of the person you are replying to.

*   **examples:**
    *   `no`
    *   `yes, @username`

### c. Technical Details (Optional)

should this tweet include technical details or specifications? if yes, please provide the specific technical information you want to include (e.g., performance metrics, key features, technical specifications).

*   **examples:**
    *   `no`
    *   `yes, include performance benchmarks and key features.`
    *   `yes, focus on its technical specifications and unique functionalities.`

## 2. Output Formatting

the output will be the generated tweet text, ready to be posted.

``````
[generated tweet text here]
``````