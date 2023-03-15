## Section 0: Prerequisites 

To get started, complete the following items if you haven’t already 

- Create a [GitHub](https://github.com/) account  if you do not have one.

- Create an Azure for Students account. 

- Download [Visual Studio Code](https://code.visualstudio.com/Download) if you do not have it. 

- Download the [Azure Static Web Apps extension](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-azurestaticwebapps) for Visual Studio Code.

By completing this demo session, you will grow your skills with Azure and you will become trained on the use of GitHub. 
 
## Section 1: Create a repository 

**Why do this section?**

I have created a template GitHub repository (or repo) specially for this session for your use. When you append `/generate` to the end of the repo URL, you are telling GitHub that you want to generate a new repository, and use the provided repo as a template for the repo you generate. This template repository has the content and styling definitions that allow you to create a web application that can serve as your online resume. 

The template features a starter app used to deploy using Azure Static Web Apps. 

1. Navigate to the following location to create a new repository: https://github.com/salimcodes/CreateYourResume/generate 

2. Name your repository `MyResume`. Note: Azure Static Web Apps requires at least one HTML file to create a web app. The repository you create in this step includes a single index.html file. 

3. Select Create repository from template. 

## Section 2: Clone the repository 

**Why do this section?**

Previously you created a GitHub repository that housed the materials needed to create your web app.  Now you’ll create a local copy (or clone) so you can modify the code on your system. Cloning repos is an important part of a developer’s work. Imagine you’re a software engineer in a large company, and all the engineers at your company are working on the same codebase. You wouldn’t want everyone to make changes to the source code at the same time – so everyone clones the source code to their own local repository, makes and tests the necessary changes, and pushes those changes to the source code when they are ready. This makes for greater organizational collaboration. 

1. Navigate to `File` > `Clone Repository` 

2. Open the `URL` tab 

3. Clone the repository

```
git clone https://github.com/<GITHUB_USERNAME>/MyResume.git
```


Note: Make note of the location where the repository is saved.  

## Section 3: Create a static web app 

**Why do this section?**

With the copy created locally, you’re all set to start working on your code and site. Now you’ll explore how to deploy your site to the cloud. You’ll use Azure Static Web Apps to host your site. A static web app (SWA) is a site built with JavaScript, HTML, CSS and potentially other tools, and SWAs are becoming increasingly common. Using Azure Static Web Apps will allow you to quickly post your site (and resume) to the world. 

1. Open Visual Studio Code and go to `File` > `Open Folder` to open the cloned repository in the editor.  

2. Inside Visual Studio Code, select the Azure logo in the Activity Bar to open the Azure extensions window. 

- Note: You are required to sign in to Azure and GitHub in Visual Studio Code to continue. If you are not already authenticated, the extension will prompt you to sign in to both services during the creation process. 

3. Under the `Static Web Apps` label, select the plus sign. 

4. The command palette opens at the top of the editor and prompts you to select a subscription name. Select your subscription and press <Enter>. 

5. Next, name your application. Type `<YourNameResume` and press <Enter>. 

5. Select a region close to you. 
- Note: Azure Static Web Apps globally distributes your static assets. The region you select determines where your optional staging environments and API function app will be located. 

6. Select Custom  Enter `/src` as the location for the application files and press `<Enter>`. This app does not produce a build output. Ensure the build output location is empty and press `<Enter>`. 

7. Select “Open Actions in GitHub.” This will launch the GitHub Actions tab in your browser. You will see the workflow run as it is creating the app. When your webapp is built and deployed, you will see a check for the workflow run.   

- Once the app is created, navigate back to Visual Studio Code - a confirmation notification is shown there. The Visual Studio Code extension also reports the build status to you as the deployment is in progress – and will update you when your app is built and deployed.  

- Once the deployment is complete, you can navigate directly to your website. 

8. To view the website in the browser, right-click on the project in the Static Web Apps extension, and select Browse Site. 


## Section 4: Customize Your Static Web App 

**Why do this section?**

With your app deployed, let’s turn our attention to updating it with your information. You want to add in your name, contact information, background, social media links, etc. You can do all of this in the HTML by modifying the provided template and replacing the various placeholders. For this exercise you will only update your name, but you should feel free to make whatever changes you might like! 

We will now do a small customization step customize your webapp you can edit it in VS Code and push changes using GitHub Desktop  

1. Navigate to the Explorer Tab in Visual Studio Code   

2. Navigate to the `src` folder, and within it, the “index.html” file  

3. Find the `Your Name` Heading. Replace `Your Name` with your real name.   

4. Save your changes in VS Code.   

5. Now, push your changes to GitHub.   
 
6. When the build is complete, refresh your app and the changes should be reflected  

Thank you for completing this exercise and attending our session!  

### More Resources 
- [An overview of the Azure Static Web App](https://learn.microsoft.com/en-us/azure/static-web-apps/overview)
- Learn more on how to automate your workflow from idea to production using [GitHub Actions](https://github.com/features/actions)
