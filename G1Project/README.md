# G1Project

This repository contains the G1Project (.NET 8).

How to publish to GitHub (local steps performed automatically):

- Initialize local git repository and create initial commit (done).

To publish to GitHub (one of the options below):

Option A — Using GitHub website:
1. Create a new repository on GitHub (keep it empty, without README).
2. In your local project folder run:
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git branch -M main
   git push -u origin main

Option B — Using GitHub CLI (gh):
1. Install and authenticate gh (https://cli.github.com/).
2. Run:
   gh repo create <your-username>/<repo-name> --public --source=. --remote=origin --push

After publishing to GitHub, to add GitLab later, create a mirror remote on your machine:
   git remote add gitlab https://gitlab.com/<your-username>/<repo-name>.git
   git push --all gitlab

