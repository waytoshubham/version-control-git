# 🚀 DevOps Version-Controlled Project with Git

This repository demonstrates a **DevOps project setup using Git best practices**, showcasing how to manage code collaboratively and efficiently using version control, branching strategies, pull requests, tagging, and markdown documentation.

---

## 📌 Project Objective

To build and manage a version-controlled DevOps project using Git and GitHub, implementing industry-standard workflows and practices such as:

- Git initialization and remote setup
- Branching strategies (`main`, `dev`, `feature/*`)
- Pull Request (PR)-based code integration
- Semantic version tagging
- Proper use of `.gitignore`
- Task documentation via markdown

---

## 📂 Project Structure

```bash
devops-project/
├── .gitignore             # Git ignore file to exclude unnecessary files
├── Dockerfile             # Docker configuration for containerizing the app
├── README.md              # Project overview and documentation
├── TASKS.md               # Markdown documentation of all tasks completed
└── src/
    └── app.py             # A simple Python script
```

---
---
 ## 💡 Approach and Workflow

**🔹 Step 1: Project Initialization**
            Initialized Git locally using git init.

            Created a new GitHub repository and connected it as the remote.

            Pushed the initial commit containing essential files.

**🔹 Step 2: Branching Strategy**
            We adopted a clean and simple branching model:

            main: Production-ready code only.

            dev: Integrates features before pushing to production.

            feature/*: For individual features.

    **Branches were created using:**

            git checkout -b dev
            git checkout -b feature/your-feature-name

**🔹 Step 3: Feature Development**
            Features (e.g., Docker support, app enhancements) are developed on feature/* branches.

            Code is pushed to GitHub and merged via Pull Requests into the dev branch.

            git checkout -b feature/add-dockerfile

         - Add files and commit

            git push origin feature/add-dockerfile

**🔹 Step 4: Pull Requests**

            Pull Requests were used to merge feature branches into dev.

            After testing in dev, it is merged into main.

**🔹 Step 5: Version Tagging**

            After major features are merged into main, a release is tagged:

            git tag -a v1.0.0 -m "Initial release with Docker and base app"
            git push origin v1.0.0

---

---
##  TASK Highlights (from TASKS.md) 

    ✅ Initialized local & remote Git repo

    ✅ Created branching model: main, dev, feature/*

    ✅ Added sample app & Docker support

    ✅ Used Pull Requests for collaboration

    ✅ Applied version tagging (v1.0.0)

    ✅ Documented tasks and usage with markdown

---