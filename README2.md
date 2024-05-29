
## Setting Up a Micro-Frontend Application
This command leverages the power of NPX (a package runner tool that comes with npm 5.2+ and higher) to create a micro-frontend setup without needing to globally install the create-mf-app package
```bash
# Run the create-mf-app command
npx create-mf-app

# Follow the prompts and provide the inputs as shown below:

# Step 1: Project Name
# Prompt: What is your project name?
# Example Input: my-micro-frontend

# Step 2: Template Selection
# Prompt: Which template would you like to use?
# Example Input: basic

# Step 3: Framework Selection
# Prompt: Which framework do you want to use?
# Example Input: React

# Step 4: Package Manager
# Prompt: Which package manager do you want to use?
# Example Input: npm

```

## Global Git Configuration
Global Git Configuration
Set up your global Git configuration with your username and email. This is necessary for committing changes to your repository.
```bash
git config --global user.name "yourusername"
git config --global user.email "yourEmail"
```
## GPG Signing Configuration
GPG signing adds a layer of security to your commits by verifying your identity. Here’s how to configure GPG signing for your commits:
```bash
gpg --version
# Enable GPG signing for commits
git config --global commit.gpgSign true

# Export and import your GPG key
gpg --armor --export yourkeyID | gpg --import
#or 
gpg --armor --export yourkeyID > mykey.asc

gpg --import mykey.asc

# Configure Git to use your GPG key for signing
git config --global user.signingkey yourkeyID
```