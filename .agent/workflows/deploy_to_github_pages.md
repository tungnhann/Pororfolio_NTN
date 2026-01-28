---
description: How to push code to GitHub and deploy with GitHub Pages
---

This workflow guides you through initializing a Git repository, pushing your code to GitHub, and deploying it using GitHub Pages.

1.  **Initialize Git Repository**
    Run the following command to initialize a new Git repository in your project folder.
    ```bash
    git init
    ```

2.  **Add Files and Commit**
    Stage all your files and create the initial commit.
    ```bash
    git add .
    git commit -m "Initial commit - Portfolio V1"
    ```

3.  **Create a Repository on GitHub**
    *   Go to [GitHub.com](https://github.com) and log in.
    *   Click the **+** icon in the top right and select **New repository**.
    *   Name your repository (e.g., `my-portfolio`).
    *   Make sure it is **Public** (required for free GitHub Pages).
    *   Do **not** check "Initialize this repository with a README" (since you already have code).
    *   Click **Create repository**.

4.  **Connect to GitHub**
    Copy the commands shown on GitHub under "…or push an existing repository from the command line". It will look like this (replace `YOUR_USERNAME` and `REPO_NAME`):
    ```bash
    git remote add origin https://github.com/YOUR_USERNAME/REPO_NAME.git
    git branch -M main
    git push -u origin main
    ```
    *Run these commands in your terminal.*

5.  **Enable GitHub Pages**
    *   Go to your repository on GitHub.
    *   Click on **Settings** (top tab).
    *   On the left sidebar, click **Pages** (under "Code and automation").
    *   Under **Build and deployment** > **Source**, select **Deploy from a branch**.
    *   Under **Branch**, select `main` and `/ (root)`.
    *   Click **Save**.

6.  **Verify Deployment**
    *   Wait a minute or two.
    *   Refresh the Pages settings page. You should see a box at the top saying "Your site is live at...".
    *   Click the link to visit your portfolio!
