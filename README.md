# Collaborative Coffee Shop Events Page

This project is a collaborative effort to create a multi-section web page showcasing a coffee shop's events and location. Each team member will take responsibility for one section: header, body, or footer. The project emphasizes teamwork and the use of Git and GitHub for version control, including creating pull requests and resolving merge conflicts.

## Project Overview

The goal is to design and develop a webpage similar to the given design:
- **Header**: Includes the logo, navigation links (e.g., Home, Story, Menu, Space, etc.), and buttons for "Order" and "Sign In."
- **Body**: Displays upcoming events and closed events, with a "Load More" button.
- **Footer**: Shows location details, customer service contact, operating hours, and social media links.

## Tasks and Steps

### 1. Initial GitHub Repository Setup
#### Create Repository
- One team member creates a new GitHub repository named `collaborative-coffee-page`.
- Initialize it with a `README.md` file.

#### Add Collaborators
- Invite the other two team members as collaborators with write access.

---

### 2. Project Initialization
#### Clone Repository
- Each team member clones the repository to their local machine.

#### Initial Commit
- Create a basic `index.html` file with standard HTML boilerplate.
- Optionally, add a `styles.css` file and link it to `index.html`.
- Commit and push these initial files to the `master` branch.

#### Set Up Branch Protection
- Navigate to **Settings > Branches > Add rule**.
- Protect the `master` branch by:
  - Requiring pull request reviews before merging.
  - Preventing direct pushes to `master`.

---

### 3. Feature Development Without Conflicts
#### Create Feature Branches
- Each team member creates a feature branch from `master`:
  - `feature/header`
  - `feature/body`
  - `feature/footer`

#### Implement Sections
- **Header**: Add a `<header>` section with the logo, navigation links, and buttons for "Order" and "Sign In."
- **Body**: Add a `<main>` section displaying:
  - **Upcoming Events**: Cards with event images, titles, and dates.
  - **Closed Events**: Cards for past events.
  - Include a "Load More" button.
- **Footer**: Add a `<footer>` section with:
  - Location details.
  - Customer service contact.
  - Operating hours.
  - Social media links.

#### Commit Changes
- Commit your changes with meaningful messages.

#### Push and Pull Request
- Push the feature branch to GitHub.
- Open a pull request (PR) to merge into `master`.
- Assign one team member as a reviewer.

#### Review and Merge
- Reviewer checks the code and approves the PR.
- Merge the PR into `master`.

---

### 4. Introducing Merge Conflicts
#### Create New Feature Branches
- Each member creates a new branch from `master`.

#### Make Conflicting Changes
- Modify the same lines in `styles.css` and/or the same section in `index.html`.
  - For example, each member adds a different background color to the `<body>` or styles the event cards differently.

#### Commit and Push
- Commit the conflicting changes.
- Push the branch to GitHub.
- Open PRs for each branch into `master` but do not merge yet.

---

### 5. Resolving Merge Conflicts Locally

#### Fetch and Merge `master` into Feature Branch
- In your local branch, run:
  ```bash
  git fetch origin
  git merge origin/master
  ```

#### Resolve Conflicts
 **Open the Conflicting Files**
   - Identify the files with conflicts and open them.

 **Manually Resolve Conflicts**
   - Choose which changes to keep or combine conflicting code.

 **Mark Conflicts as Resolved**
   - After resolving, mark the files as resolved:
     ```bash
     git add <file>
     ```

 **Commit Resolved Changes**
   - Commit the merge with a descriptive message:
     ```bash
     git commit -m "Resolved merge conflicts between master and <branch>"
     ```

 **Push Changes**
   - Push the updated branch to GitHub:
     
 **Update Pull Request**
   - The pull request will automatically update to reflect the resolved conflicts.

 **Review and Merge**
   - Assign a reviewer for the updated pull request.
   - After approval, merge the pull request into `master`.

---

## 6. Finalizing the Project
 **Update Local `master` Branch**
   - Switch to the `master` branch and pull the latest changes:
     ```bash
     git switch master
     git pull origin master
     ```

 **Test the Web Page**
   - Open `index.html` in a browser to ensure all sections display correctly.
   - Verify that all styles and functionality are applied as intended.

## 7. Publish the Web Page with GitHub Pages
   - Open the GitHub Pages link in a browser.
   - Verify that all sections and styles display correctly on the live site.
