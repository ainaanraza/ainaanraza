# 🛠️ Setup Instructions for Your Cyberpunk GitHub Profile

Welcome to your new premium, cyberpunk-themed GitHub Profile README! Since you want this to look like the portfolio of an AI Engineer from the future, I have built highly advanced SVG animations and configured several automated data pipelines (GitHub Actions) for you.

Follow these steps to make your profile live:

## 1. Replace the Placeholder Username

Right now, the `README.md` uses `<YOUR_GITHUB_USERNAME>` as a placeholder for URLs (so widgets and trackers know whose data to fetch).

1. Open `README.md` in a text editor.
2. Use **Find and Replace** (Ctrl+F or Cmd+F) to find all instances of `<YOUR_GITHUB_USERNAME>`.
3. Replace them with your actual GitHub username (e.g., `AinaanRaza`).
4. Save the file.

## 2. Push to GitHub

1. Ensure the directory name matches your GitHub username exactly.
2. Initialize a git repository if you haven't already:
   ```bash
   git init
   git add .
   git commit -m "Initial commit of Cyberpunk Profile"
   ```
3. Push to your special repository (`https://github.com/your-username/your-username`).

## 3. Enable GitHub Actions (Crucial for Widgets!)

This repository contains three powerful GitHub Action workflows that automatically update your README's dynamic elements:
1. **Snake Animation (`snake.yml`)**: Generates the animated 2D contribution grid snake.
2. **Metrics (`metrics.yml`)**: Generates your achievements showcase.
3. **3D Contribution Render (`3d.yml`)**: Generates a 3D isometric view of your contribution graph.

To make these work:
1. Go to your repository on GitHub.
2. Click on the **Actions** tab.
3. You will see a prompt saying "Workflows aren't being run in this repository". Click **I understand my workflows, go ahead and enable them**.
4. You can click on each workflow on the left sidebar and click **Run workflow** manually to generate the initial images immediately, rather than waiting for the schedule (midnight/evening).

> **Note on `metrics.yml` Token**: For the metrics workflow to fetch all your data, you must create a Personal Access Token (PAT) with `public_repo` scope and add it as a repository secret named `METRICS_TOKEN`.

## 4. Final Verification

Once the actions have run successfully:
- You should see the dark mode snake animation appear.
- The `github-metrics.svg` file will be generated in your repo, and the README will display your achievements.
- The `profile-3d-contrib` folder will be created, and the 3D grid will appear on your profile.

Enjoy your masterpiece! 👾
