# ChatGPT Actions Library

Welcome to the **ChatGPT Actions Library**, a curated collection of useful actions for custom GPTs on [ChatGPT.com](https://chat.openai.com/). This repository serves as a library for pre-defined actions that can be easily integrated into your custom GPTs, enabling them to interact with external APIs or services.

## Repository Structure

- `api.github.com.yml`: OpenAPI schema for GitHub's REST API v3, including actions to manage issues and milestones.
- `GitHub.md`: Detailed instructions on how to set up GitHub-specific actions, including authentication and integration.

## Getting Started

To use this library:
1. Clone this repository or download the specific YAML files you need.
2. Follow the instructions in each service-specific guide (e.g., `GitHub.md`) to set up the corresponding actions.
3. Configure your GPT on [ChatGPT.com](https://chat.openai.com/) to use these actions.

---

## General Setup for ChatGPT Actions

### Step 1: Access the Actions Section
1. Go to [ChatGPT.com](https://chat.openai.com/).
2. Create or edit a custom GPT.
3. Navigate to the **Actions** tab.

### Step 2: Add Actions from This Library
1. Click **Create Action**.
2. Copy the contents of the desired OpenAPI YAML file (e.g., `api.github.com.yml`) into the **Schema** section.
3. Save the action.

### Step 3: Add Credentials
Some actions may require credentials (e.g., API tokens). Follow the instructions in the service-specific documentation (e.g., `GitHub.md`) to securely configure these.

---

## Included Actions

### GitHub Actions
The `api.github.com.yml` schema provides actions for interacting with GitHub's REST API, including:
- Listing, creating, retrieving, and updating issues.
- Listing and managing milestones.

For GitHub-specific setup, see [GitHub.md](./GitHub.md).

---

## Contributing

We welcome contributions to expand this library! To contribute:
1. Fork this repository.
2. Add or improve actions.
3. Submit a pull request with a description of your changes.

---

## License

This project is licensed under the [MIT License](https://spdx.org/licenses/MIT.html).
