# SKKU Scholarship Assistant (스꾸장학비서)

This repository serves as the main project hub, bringing together **aid-frontend** and **aid-backend** as Git submodules.  
It also contains a `docs/` folder for project documentation.

## Overview
**SKKU Scholarship Assistant** is a project designed to make it easier for Sungkyunkwan University (SKKU) students to gather and check scholarship-related notices and announcements.

## Repository Structure

```
project/
├─ frontend/     # Submodule: https://github.com/SKKU-aid/aid-frontend.git
├─ backend/      # Submodule: https://github.com/SKKU-aid/aid-backend.git
└─ docs/         # Documentation folder
```

## Cloning & Initializing Submodules

1. **Clone the main repository:**
   ```bash
   git clone https://github.com/SKKU-aid/project.git
   cd project
   ```
2. **Initialize and update submodules:**
   ```bash
   git submodule update --init --recursive
   ```
   - This command pulls in the code from `aid-frontend` and `aid-backend` into their respective folders.

## Working with Submodules

- If you need to **pull the latest commits** from the submodule repositories (assuming you have them set to track a specific branch), run:
  ```bash
  cd frontend  # or backend
  git checkout main
  git pull origin main
  cd ..
  git add frontend  # or backend
  git commit -m "Update submodule to latest commit"
  git push origin main
  ```
- Other team members should then perform `git submodule update --init --recursive` again to get the updated submodule references.

## Documentation

- The `docs/` folder holds any project documentation.
