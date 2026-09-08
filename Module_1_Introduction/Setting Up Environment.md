# Setting Up the Environment

## Overview

In this lab, will set up an online repository for the project and learn how to create folders and files in the **Skills Network Environment**. Will also understand how to view the output of the code.

## Learning Objectives

After completing this lab, will be able to:

- Create an online repository
- Create folders and files in **Skills Network Environment**.
- Run the code to see the output.
- Perform Git operations.

## Step 1: Create an online repository and create personal access token

1. Create a blank public GitHub repository in your GitHub account without creating any README.md file for this. Make sure to set your repository to public and name it accordingly.

2. Can find more information by visiting the Create GitHub repository page.

3. Personal Access Token is now a mandatory part to push data to GitHub repositories to make sure your authentication is related to GitHub account.

4. To create a **Personal Access Token**, go to your GitHub account and click on your profile icon located in the top-right corner. Then click on settings.

5. Next, select **Developer Settings**. This option is typically available towards the bottom of the window.

6. Navigate to **Tokens (classic)** under **Personal access tokens**.

7. To generate an access token, click **Generate a personal access token**.

8. In the **Generate token** page, fill in the required details and click the **repo** checkbox to enable access for `git` commands.

9. Then, click **Generate token**.

10. Your personal access token will be generated. The token is only valid for **30 days**. Will need to generate a new token once the current token expires.

**REMEMBER**: Make sure to copy your personal access token now. Won't be able to see it again! In case you forgot to save it or misplaced it, delete the already created token and generate a new one.

Note: This repository will be your main repository for all the labs except the practice project lab and the final project lab.

## Step 2: Create files in Skills Network Environment

1. In the right window page, click on the Explorer, as show in the screenshot below (refer to number 1). Next, click on the project folder, and then click the icon highlighted in red (refer to number 2) in the screenshot. Enter the folder name as **Sample Folder**. This action will create a folder for you. Next, select the **SampleFolder** folder shown at number 3, right-click, and select **New File**. Enter the file name as **sample_folder.html** and click OK. This will create the HTML file within the **SampleFolder**.

Note: Do not click on the `.theia` folder before creating a new folder. Make sure that you are in the root project directory.

2. Create a basic template structure in the HTML file **sample_folder.html** by copying the provided content and pasting in the **sample_folder.html** file.

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Sample Folder</title>
  </head>
  <body>
    <h1>Sample Folder</h1>
    <button>SampleFolder</button>
  </body>
</html>
```

After pasting the code, save the file.

## Step 3: Perform Git commands in the terminal

1. Now, click on the "Terminal" tab at the top-right of the window, and then click on "New Terminal".

2. Next, within the path of the terminal, initialize it to create a Git repository to perform all Git commands in this terminal. Use the provided command for this purpose in the terminal and press **Enter**.

`git init`

3. Then, you will need to execute this command in the terminal for performing necessary commands within the **Skills Network Environment** and press **Enter**.

`git config --global --add safe.directory /home/project`

Note: The above command will help you to work inside the project folder environment with git commands.

4. Then, set the `git config --global` for email address by performing given command in terminal by providing email address of your GitHub account within double quotes instead of `you@example.com` and press **Enter**.

`git config --global user.email "you@example.com"`

- Again, set the `git config --global` for username by performing given command in terminal by providing username of the GitHub account within double quotes instead of **Your Name** and press **Enter**.

`git config --global user.name "Your Name"`

5. Next, perform `git add` and `git commit` to save the changes for the GitHub repository by running the following commands one after another:

`git add --a`
`git commit -m "initial commit"`

6. Perform `git push` commands to push the files into your GitHub repository.

- Add your GitHub repository URL in origin2 variable by writing given commands in the terminal.
- Also replace the entire `<git-repo-url>` with your GitHub repository URL such as `git remote add origin2 https://github.com//youraccountname//yourrepositoryname` and click **Enter**.

`git remote add origin2 <git-repo-url>`

Then, perform the given command in the terminal to push the content of the file in the GitHub repository and click **Enter**.

`git push origin2`

7. While pushing the files in GitHub using `git push` command, it will ask you to enter the username for your GitHub account in the terminal. Enter your username and then press enter. Next, it will also ask for your password, here you need to paste the **Personal Access Token** that you generated in step 1.

Note: Upon pasting your **Personal Access Token** into the terminal, it won't show for security reasons, but it's already there. Simply hit enter, and it will push your files and folders to the GitHub repository.

8. It will push all the files directly into your GitHub repository.

Note: Can also refer to `git_commands` for more detailed instruction.

## Step 4: Need to perform Git commands

It is crucial to follow a few essential steps to ensure the proper management and persistence of your data in a GitHub repository:

- **Regular updates**: Whenever you make changes or add new components to your project, adding, committing, and pushing the updates to your GitHub repository is essential. This process ensures that your latest work in safely stored and accessible to collaborators.

- **Session persistence**: During an active session, your data remains accessible. However, it's important to note that if your session expires or you log out, you will need to clone the repository again to resume work.

By adhering to these guidelines, can maintain a well-organized and efficient GitHub repository, ensuring your work is securely stored and easily accessible to you and your collaborators.
