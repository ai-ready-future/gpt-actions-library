# GitHub Actions Setup Guide

This guide explains how to configure the GitHub-specific actions included in the `api.github.com.yml` schema.

---

## Step 1: Generate a GitHub Personal Access Token (PAT)

1. Log in to your GitHub account.
2. Go to [Settings > Developer settings > Personal access tokens](https://github.com/settings/tokens).
3. Click **Generate new token (classic)**.
4. Select the following scopes based on your needs:
   - `repo`: Access private repositories (required for issues and milestones in private repos).
   - `read:org`: Access organizational repositories (optional).
5. Set an expiration date (recommended for security).
6. Copy the token and save it securely.

---

## Step 2: Add the Token as a Credential in ChatGPT

1. Go to [ChatGPT.com](https://chat.openai.com/).
2. Edit your custom GPT.
3. Navigate to the **Settings > Credentials** section.
4. Add a new credential:
   - **Key**: `GITHUB_TOKEN`
   - **Value**: Paste the GitHub PAT you generated.
5. Save the credential.

---

## Step 3: Enable GitHub Actions in Your GPT

1. Open the `api.github.com.yml` file from this repository.
2. Copy the contents into the **Actions > Add Action** section in your GPT settings.
3. Save the action.

---

## Step 4: Test the GitHub Actions

Use the custom GPT to perform tasks, such as:
- Listing issues in a repository.
- Creating a new issue.
- Retrieving milestones.

For testing:
- Ensure the repository you are testing against matches the credentials' access permissions.
- Validate the results by checking the GitHub UI for changes made by the GPT.

---

## Troubleshooting

- Ensure your GitHub PAT has the correct scopes.
- Check the GPT's logs for error messages if an action fails.
- Validate that the API endpoint and parameters in the YAML schema match the desired functionality.

---

## Notes

- Keep your GitHub PAT secure; treat it like a password.
- Regularly rotate your PAT to maintain security.

For additional help, visit the [GitHub REST API documentation](https://docs.github.com/rest).
