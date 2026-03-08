# hackathon-practice

## How to Generate a GitHub Personal Token (Classic) and Clone the Repo

### Step 1: Generate a Personal Access Token (Classic)

1. Go to GitHub and click your profile picture → **Settings**
2. In the left sidebar, scroll down and click **Developer settings**
3. Click **Personal access tokens** → **Tokens (classic)**
4. Click **Generate new token (classic)**
5. Give your token a descriptive **Note** (e.g., "hackathon-practice")
6. Set an **Expiration** (recommend 30-90 days)
7. Select scopes: Check **repo** (full control of private repositories)
8. Click **Generate token**
9. **Copy the token immediately** - you won't be able to see it again!

### Step 2: Clone the Repository Using the Token

Replace `YOUR_TOKEN` with your generated token and `YOUR_USERNAME` with your GitHub username:

```bash
git clone https://YOUR_TOKEN@github.com/Jeong1996/hackathon-practice.git
```

Or use this format:

```bash
git clone https://YOUR_USERNAME:YOUR_TOKEN@github.com/Jeong1996/hackathon-practice.git
```

### Note
- Never share your token with anyone
- Add the token to your Git credentials if you want to avoid entering it each time:
  ```bash
  git config --global credential.helper store
  ```

## How to Create a Pull Request Against the Main Branch

### Step 1: Create a New Branch

```bash
git checkout -b my-feature-branch
```

### Step 2: Make Your Changes

Edit or add files, then commit:

```bash
git add .
git commit -m "Description of your changes"
```

### Step 3: Push Your Branch to GitHub

```bash
git push origin my-feature-branch
```

### Step 4: Create the Pull Request

1. Go to the repository on GitHub
2. You should see a **Compare & pull request** button for your branch
3. Click it and set:
   - **base repository**: Jeong1996/hackathon-practice
   - **base**: main
   - **compare**: my-feature-branch
4. Add a title and description
5. Click **Create pull request**

### Alternative: Create PR from Command Line (using gh CLI)

If you have GitHub CLI installed:

```bash
gh pr create --base main --head my-feature-branch --title "My Feature" --body "Description"
```
