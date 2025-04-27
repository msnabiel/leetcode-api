# How to Contribute 🤔

## Using Docker 🐳

### Step 1: Fork the Repository
- Create a fork of this repository to your GitHub account
- Look for the "Fork" button in the top right corner of the repository page

### Step 2: Clone Your Fork
```bash
git clone https://github.com/msnabiel/leetcode-api.git
```
### Step 3: Navigate to Project Directory
```
cd leetcode-api
```
### Step 4: Launch with Docker
```
docker compose up
```
## Without Docker
### Step 1: Fork the Repository

Create a fork of this repository to your GitHub account
Look for the "Fork" button in the top right corner of the repository page

### Step 2: Clone Your Fork
```
git clone https://github.com/msnabiel/leetcode-api.git
```
### Step 3: Navigate to Project Directory
```
cd leetcode-api
```
### Step 4: Install Dependencies
```
npm install
```
### Step 5: Start Development Server
```
npm run dev
```
## Making Your Contribution
### Best Practices

Create a new branch with a descriptive name related to your changes (e.g., fix/rate-limit-issue or feature/new-endpoint)
Make your changes with clear, descriptive commit messages
Push your changes to your forked repository
Create a Pull Request (PR) to the main repository

### PR Guidelines

Clearly describe what your changes accomplish
Reference any related issues
Ensure your code follows the project's style and conventions

While not mandatory, creating feature-specific branches helps streamline the review and merge process.
Local Development
The server will be available at http://localhost:3000 by default. You can now test your changes and ensure everything works as expected before submitting your PR.