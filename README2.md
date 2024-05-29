## Git Hub Configurations

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



Set Git hub Configuratin for this project
```bash
git config --global user.name "yourusername"
git config --global user.email "yourEmail"
```

For gpgSign Config

```bash
gpg --version
git config --global commit.gpgSign true
gpg --armor --export generatedkey | gpg --import
```