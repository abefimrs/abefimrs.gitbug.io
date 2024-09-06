### Set Up Git and GitHub:
Install Git (if not already installed):

#### Windows: Download and install from git-scm.com.
#### macOS: Git is typically pre-installed. If not, use Homebrew:
```
brew install git
```
Linux:
```
sudo apt-get install git
```
#### Configure Git (set up username and email):
```
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```
#### Create a new repository on GitHub:

Go to GitHub and log in.
Click the + icon in the top right corner and select "New repository".
Name it team-portfolio, set it to public or private, and click "Create repository".
#### Clone the Repository:
Clone the repository to your local machine:
```
git clone https://github.com/your-username/team-portfolio.git
```
Navigate into the project directory:
```
cd team-portfolio
```
#### Create a Branch for Each Team Member:

#### Create a new branch:

```
git checkout -b header-section
```

Replace header-section with your specific section name (about-section, footer-section, etc.).

#### Build the Website:
Create your section's files (e.g., index.html, style.css, script.js).

Add the new files to Git:
```
git add index.html style.css script.js
```
#### Commit Changes:
Commit the changes:
```
git commit -m "Added header section with navigation"
```
#### Push Changes to GitHub:
Push your branch to the remote repository:
```
git push origin header-section
```
Replace header-section with your branch name.

#### Create a Pull Request:
Go to your repository on GitHub.
Click on the "Compare & pull request" button next to your branch.
Review your changes and click "Create pull request".
#### Resolve Merge Conflicts:
If GitHub indicates there are conflicts, you can resolve them by:

Fetch the latest changes from the main branch:
```
git checkout main
git pull origin main
```

Switch back to your branch and merge the main branch:
```
git checkout header-section
git merge main
```
Resolve any conflicts in the files (Git will mark conflicts with <<<<<< and >>>>>>).
Add and commit the resolved files:
```
git add .
git commit -m "Resolved merge conflicts"
```
#### Push the updated branch:

```
git push origin header-section
```
#### Merge the Branches:

After reviewing the pull request, merge it on GitHub:

Click "Merge pull request" on the GitHub PR page.
Confirm the merge by clicking "Confirm merge".
Delete the branch (optional but recommended):

After merging, you can delete the branch on GitHub by clicking "Delete branch" on the PR page.
Alternatively, delete it locally and remotely:
```
git branch -d header-section
git push origin --delete header-section
```
#### Final Review:
Pull the latest changes into the main branch locally:

```
git checkout main
git pull origin main
```
Open the index.html file in a browser to review the integrated website.
#### Submission:
Submit the GitHub repository link to the instructor
