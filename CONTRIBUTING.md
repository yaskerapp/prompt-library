# Contribution Guidelines
Before contributing to this repository, please ensure you are adhering to the following general guidelines. Further, if you are submitting a new prompt to the repository, be sure you are also following the prompt-specific guidelines. These checks will ensure that your contributions can be easily integrated into the main repository, without any headache for the owners.

## General Guidelines
The following guidelines should be followed when making any open-source contributions:
- [ ] Contributions should be made via a pull request to the main repository from a personal fork.
- [ ] Pull requests should be accompanied by a descriptive title and detailed explanation.
- [ ] Submit all pull requests to the repository's main branch.
- [ ] Before submitting a pull request, ensure additions/edits are aligned with the overall repo organization.
- [ ] Be sure changes are compatible with the repository's license.
- [ ] In case of conflicts, provide helpful explanations regarding your proposed changes so that they can be approved by repo owners.

## New Prompt Guidelines
To add a new prompt to this repository, a contributor should take the following steps (in their personal fork):
1. Create and test the new prompt.
    - See the [README](https://github.com/yakerapp/prompt-library/blob/main/README.md) for guidance on how to write effective prompts.
    - Ensure prompts generate intended results and can be used by other users to replicate those results.
2. Add the prompt to `prompts.json`.
    - Find suitable category for the prompt. (If no category exists, create a new one.)
    - Append the prompt to the category's list of prompts.
    - Provide a name, description, and example for the prompt.
    - Ensure the prompt is formatted correctly. It must satisfy following interface:
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
4. Submit a pull request on the repository's main branch.
    - If possible, provide some documentation of how you tested your prompt and the kinds of results you received.
    - Be sure to include a detailed name and description.

### New Prompt Checklist:
- [ ] I've confirmed the prompt works well
- [ ] I've added to the `prompts.json` file
- [ ] I've ensured the prompt is formatted correctly
- [ ] I've submitted a pull request

Please ensure these requirements are met before submitting a pull request.
