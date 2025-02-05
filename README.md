# 🚀 AutoRepoSync

**AutoRepoSync** is a GitHub Actions workflow designed to automate repository synchronization between a personal repository and an organization's repository.

## ✨ Features:
- ✅ **Automatic Trigger** – When a push occurs in a specific branch of your personal repo, the workflow is triggered.
- 🔧 **Repository Creation** – If the target repository does not exist in the organization, it is automatically created with a defined prefix or suffix.
- 🔄 **Branch Synchronization** – Ensures that changes from the specified branch in your personal repo are pushed to a corresponding branch in the organization's repository.
- 🔁 **Continuous Updates** – If the organization repo already exists, it simply pushes updates to the target branch.
- 🔐 **Secure & Configurable** – Uses GitHub tokens for authentication and can be customized for different use cases.

## 🚀 How It Works:
1. Push to a specific branch (e.g., `sync-branch`) in your personal repository.
2. The workflow checks if the corresponding repo exists in the organization.
3. If the repo doesn't exist, it is created with a predefined naming pattern.
4. The branch is pushed to the organization's repository.
5. Subsequent pushes keep syncing changes to the org repo's branch.

## 🛠 Setup Instructions:
1. Ensure you have a **GitHub Personal Access Token (PAT)** with repository permissions.
2. Define your **organization name**, **target repo prefix/suffix**, and **branch name** in the workflow file.
3. Commit and push changes to the specified branch to trigger the sync.

## 📌 Use Case Scenarios:
- Automating repo mirroring from a personal to an organization repo.
- Ensuring branch consistency across multiple repositories.
- CI/CD workflows where changes in a private repo need to be reflected in an org repo.
