````markdown
# RoBoToMaZe Assignment

Group assignment repository for the RoBoToMaZe search-algorithm project.

## Files

```text
Assingment-1-AI-DIS/
├── README.md
└── AI_programming_1_RoBoToMaZe.ipynb
```

The notebook is a file. The repository is the folder containing it.

## Requirements

Install:

- Git
- Python 3
- VS Code
- VS Code Python and Jupyter extensions
- Pygame
- NumPy

Install Python packages:

```powershell
python -m pip install pygame numpy
```

Test Pygame:

```powershell
python -c "import pygame; print(pygame.__version__)"
```

## Clone the Repository

Each team member clones the repository once:

```powershell
git clone https://github.com/phil10181/Assingment-1-AI-DIS.git
cd "Assingment-1-AI-DIS"
code .
```

Check the remote:

```powershell
git remote -v
```

Configure Git identity if needed:

```powershell
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

## Branch Rules

`main` contains the approved version.

Never work directly on `main`. Each task gets its own branch:

```text
task-1-customisation
task-2-bfs
task-3-dfs
task-4-comparison
task-5-game-integration
task-6-path-description
documentation-readme
```

## Start a New Task

Update `main` first:

```powershell
git switch main
git pull origin main
```

Create and switch to a task branch:

```powershell
git switch -c task-2-bfs
```

Check your branch:

```powershell
git branch --show-current
```

## Working on the Notebook

Before editing:

```powershell
git status
```

Tell the team which task or notebook section you are editing.

Only one person should edit the same notebook section at a time. Jupyter notebooks are stored as one JSON file, so simultaneous edits can create difficult conflicts.

After editing:

1. Save the notebook.
2. Run the cells you changed.
3. Test the code.
4. Check that unrelated cells were not changed.

Review changes:

```powershell
git status
git diff --stat
git diff
```

## Commit Changes

Add the notebook:

```powershell
git add AI_programming_1_RoBoToMaZe.ipynb
```

Add the README if it changed:

```powershell
git add README.md
```

Or add all changed files:

```powershell
git add .
```

Commit with a clear message:

```powershell
git commit -m "Implement BFS search algorithm"
```

Good commit messages describe the work:

```text
Add BFS implementation
Add DFS test scenarios
Document algorithm comparison
Integrate search algorithms with game
Update collaboration instructions
```

## Push Your Branch

First push:

```powershell
git push -u origin task-2-bfs
```

Later pushes:

```powershell
git push
```

Do not use force push:

```powershell
git push --force
```

## Pull Requests

After pushing:

1. Open the repository on GitHub.
2. Create a pull request.
3. Set the base branch to `main`.
4. Set the compare branch to your task branch.
5. Explain what changed and how it was tested.
6. Ask a teammate to review it.
7. Merge only after review.

Do not push directly to `main`.

## After Merging

Update local `main`:

```powershell
git switch main
git pull origin main
```

Delete the completed local branch:

```powershell
git branch -d task-2-bfs
```

Create the next task branch:

```powershell
git switch -c task-3-dfs
```

## Updating an Existing Task Branch

If `main` changed while you were working:

```powershell
git fetch origin
git switch main
git pull origin main
git switch task-2-bfs
git merge main
```

If there are no conflicts:

```powershell
git push
```

## Merge Conflicts

Check the conflict:

```powershell
git status
```

For a normal text file:

1. Open the file.
2. Keep the correct changes.
3. Remove conflict markers.
4. Save the file.

Then run:

```powershell
git add filename
git commit -m "Resolve merge conflict"
git push
```

For notebook conflicts, make a backup first and resolve the changes with the teammate who edited the other section.

Cancel an unfinished merge if necessary:

```powershell
git merge --abort
```

## Useful Commands

```powershell
git status
git branch --show-current
git branch --all
git log --oneline --max-count=5
git fetch origin
git pull origin main
git push
```

## Daily Workflow

```powershell
cd "Assingment-1-AI-DIS"
git switch main
git pull origin main
git switch -c task-name

# Edit and test the notebook

git status
git add .
git commit -m "Describe the change"
git push -u origin task-name
```

Then create a pull request on GitHub.

## Team Rules

- Use one branch per task.
- Pull before starting work.
- Do not edit the same notebook section simultaneously.
- Test changes before committing.
- Use descriptive commit messages.
- Review pull requests before merging.
- Do not push directly to `main`.
- Do not use force push.
- Do not commit passwords, tokens, or unrelated files.
````
