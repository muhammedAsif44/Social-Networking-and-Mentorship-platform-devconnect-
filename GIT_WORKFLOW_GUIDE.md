# Git Workflow Guide

Here is a simple guide on how to save your changes and push them to GitHub when you add new features.

## The Basic Workflow (3 Steps)

Whenever you make changes to your code (edit files, add new files, delete files), follow these 3 steps to save them to GitHub:

### 1. **Add** your changes
This tells Git about the files you have changed.
```bash
git add .
```
*   `git add .` stages **all** your changes at once.
*   If you only want to add specific files, use `git add path/to/file`.

### 2. **Commit** your changes
This saves a "snapshot" of your changes with a message describing what you did.
```bash
git commit -m "Description of what I changed"
```
*   Example: `git commit -m "Added login feature"`
*   Example: `git commit -m "Fixed bug in user profile"`

### 3. **Push** to GitHub
This uploads your commit to the GitHub website.
```bash
git push
```
*   This sends your changes to the `main` branch on GitHub.

---

## Example Scenario

Let's say you just created a new "About Us" page in the frontend.

1.  **Check what changed** (Optional but recommended):
    ```bash
    git status
    ```
    *   *You will see `front-end/src/pages/AboutUs.jsx` in red.*

2.  **Add the files**:
    ```bash
    git add .
    ```

3.  **Commit the save**:
    ```bash
    git commit -m "Created new About Us page"
    ```

4.  **Upload to GitHub**:
    ```bash
    git push
    ```

---

## status Check
At any time, if you are unsure what is going on, run:
```bash
git status
```
It will tell you if you have unsaved changes or if you are ready to push.
