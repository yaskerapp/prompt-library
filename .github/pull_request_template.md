# Add New Prompt

You'll need to add your prompt into `prompts.json` file.

## Description

This prompt is intended to be used for ...

- [ ] I've confirmed the prompt works well
- [ ] I've added to the `prompts.json` file
- [ ] I've ensured the prompt is formatted correctly and satisfies the following interface:
  ```TypeScript
  interface Prompt {
    name: string;
    prompt: string;
    contributor: string;
    reference?: string;
    description?: string;
    example?: { role: 'user' | 'assistant', content: string }[];
  }
  ```
- [ ] I've submitted a pull request

Please make sure you've completed all the checklist.
