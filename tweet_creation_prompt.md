# Tweet Creation Prompt

This prompt helps in generating tweets based on your specifications.

## 1. Input Requirements

Please provide the following details to generate your tweet:

### a. Writing Style (Required)

Describe the desired writing style for the tweet. Be as specific as possible.

*   **Examples:**
    *   `Formal and informative`
    *   `Casual and humorous`
    *   `Enthusiastic and promotional`
    *   `Sarcastic and witty`
    *   `Concise and direct`
*   If the subject is outside the agent's abundant knowledge, the agent should ask for more detailed information or context from the user.

### b. Subject (Required)

What is the main topic or subject of the tweet? Provide enough detail for context.

*   **Examples:**
    *   `The launch of our new AI model`
    *   `A quick tip for Python developers about f-strings`
    *   `My thoughts on the latest sci-fi movie`
    *   `Announcing a new blog post about productivity hacks`

### c. Is it a reply? (Optional)

Is this tweet a reply to someone else's tweet? If yes, please provide the Twitter handle of the person you are replying to.

*   **Examples:**
    *   `No`
    *   `Yes, @username`

## 2. Output Formatting

The output will be the generated tweet text, ready to be posted.

``````
[Generated Tweet Text Here]
``````