# Task 3: Version-Controlled DevOps Project

This repository is my submission for Task 3 of the Elevate Labs DevOps Internship.

## 1. Task Objective

The objective of this task was to manage a simple project using Git best practices, including proper branching, pull requests, versioning, and documentation.

## 2. My Git Workflow

I implemented a GitFlow-style workflow. This separates new development from stable, production-ready code. Here are the exact steps I took:

1.  **Initialization:** Initialized a local Git repo and created a `.gitignore` file to exclude system files and logs, per best practices.
2.  **Branching Strategy:** Created two primary branches:
    * `main`: This branch is for production-ready code.
    * `dev`: This is the primary development branch for integrating new features.
3.  **Branch Protection:** I applied a **branch protection rule** to `main` on GitHub, requiring a pull request to merge any changes. This prevents accidental pushes and ensures all code is reviewed.
4.  **Feature Development:**
    * For each new feature (e.g., "add-page-title"), I created a new `feature/*` branch *from* the `dev` branch.
    * I made my commits on these feature branches.
5.  **Pull Requests (Code Review):**
    * I opened a **Pull Request (PR)** for each feature branch to merge into `dev`. This simulates a team code review.
    * After merging, the feature branch was deleted to keep the repository clean.
6.  **Release to Main:**
    * Once all features were on `dev`, I opened a final PR to merge `dev` into `main`, simulating a "release."
7.  **Tagging:**
    * Finally, I **tagged** the latest commit on `main` as `v1.0.0` to mark the official release.

### My Project Structure:
* **main branch:** The stable, protected "production" branch.
* **dev branch:** The integration branch for new features.
* **Pull Requests:** Used to merge `feature/*` -> `dev` and `dev` -> `main`.
* **Tag:** `v1.0.0` marks the final release.

### Proof of Work:
**1. Branching Workflow (Network Graph)**
<img width="1920" height="874" alt="Screenshot 2025-10-24 173630" src="https://github.com/user-attachments/assets/66063e5d-288b-4470-8f87-ea8c349b944b" />

**2. Final Release Tag (v1.0.0)**
<img width="1920" height="886" alt="Screenshot 2025-10-24 173659" src="https://github.com/user-attachments/assets/ebf43343-0e69-43ed-a905-cfdae39a6e1d" />



