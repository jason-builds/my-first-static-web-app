<h1 align="center">
  <br>
  <a href="http://www.amitmerchant.com/electron-markdownify"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/Microsoft_Azure.svg" alt="Azure" width="200"></a>
  <br>
  epam Azure Fundamentals Course (Final Task)
  <br>
</h1>

<h4 align="center">A simple guide to building your first static site with <a href="https://azure.microsoft.com/en-us/products/app-service/static" target="_blank"> Azure Static Web Apps </a> </h4>

<p align="center">
  <a href="https://react.dev/"><img src="https://forthebadge.com/images/badges/made-with-react.svg"></a>
  <a href="https://azure.microsoft.com/en-us/products/app-service/"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/powered-by-azure-app-service.svg"></a>
  <a href="https://forthebadge.com"><img src="http://forthebadge.com/images/badges/built-with-love.svg"></a>
</p>

<p align="center">
  <a href="#key-features">Key Features</a> •
  <a href="#prerequisites">Prerequisites</a> •
  <a href="#create-a-repository">Create a repository</a> •
  <a href="#clone-the-repository">Clone the repository</a> •
  <a href="#install-the-azure-static-web-apps-extension">Install the Azure Static Web Apps extensionRelated</a> •
  <a href="#create-a-static-web-app-in-the-10-easy-steps">Create a static web app in the 10 easy steps</a>
</p>

![screenshot](https://raw.githubusercontent.com/amitmerchant1990/electron-markdownify/master/app/img/markdownify.gif)

## Key Features

* <b>Web hosting</b> for static content like HTML, CSS, JavaScript, and images.
* <b>Integrated API</b> support provided by managed Azure Functions, with the option to link an existing function app, web app, container app, or API Management instance using a standard account. If you need your API in a region that doesn't support [managed functions](https://learn.microsoft.com/en-us/azure/static-web-apps/apis-functions), you can [bring your own functions](https://learn.microsoft.com/en-us/azure/static-web-apps/functions-bring-your-own) to your app.
* <b>First-class GitHub and Azure DevOps integration</b> that allows repository changes to trigger builds and deployments.
* <b>Globally distributed</b> static content, putting content closer to your users.
* <b>Free SSL certificates</b>, which are automatically renewed.
* <b>Custom domains</b> to provide branded customizations to your app.
* <b>Seamless security model</b> with a reverse-proxy when calling APIs, which requires no CORS configuration.
* <b>Authentication provider integrations</b> with Microsoft Entra ID and GitHub.
* <b>Customizable authorization role definition</b> and assignments.
* <b>Back-end routing rules</b> enabling full control over the content and routes you serve.
* <b>Generated staging versions</b> powered by pull requests enabling preview versions of your site before publishing.
* <b>CLI support</b> through the [Azure CLI](https://learn.microsoft.com/en-us/cli/azure/staticwebapp?view=azure-cli-latest) to create cloud resources, and via the [Azure Static Web Apps CLI](https://github.com/Azure/static-web-apps-cli#azure-static-web-apps-cli) for local development.

## Prerequisites
* [GitHub](https://github.com/) account
* [Azure](https://portal.azure.com/) account
* [Visual Studio Code](https://code.visualstudio.com/)
* [Azure Static Web Apps extension for Visual Studio Code](https://code.visualstudio.com/)
* [Install Git](https://www.git-scm.com/downloads)

## Create a repository
This article uses a Github template repository to make it easy for you to get started. The template features a starter app to deploy to Azure Static Web Apps.

You may choose from the No Framework, Angular, Blazor, React and Vue list of options below (<b>choose one</b>):

   <table>
        <thead>
            <tr>
                <th align="center">Framework</th>
		<th align="center">Step 1</th>
                <th align="center">Repo</th>
		<th align="center">Step 2</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a> <strong>No Framework</strong></td>
                <td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Navigate to the following location to create a new repository:</td>
		<td align="center"><a href="https://github.com/new?template_name=vanilla-basic&template_owner=staticwebdev" rel="nofollow"><img alt="Static Badge" src="https://img.shields.io/badge/https%3A%2F%2Fgithub.com%2Fstaticwebdev%2Fvanilla-basic?color=blue&link=https%3A%2F%2Fgithub.com%2Fnew%3Ftemplate_name%3Dvanilla-basic%26template_owner%3Dstaticwebdev" alt="Create a new repository" data-canonical-src="https://github.com/new?template_name=vanilla-basic&template_owner=staticwebdev" style="max-width: 100%;"></a></td>
		<td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Name your repository <strong>my-first-static-web-app</strong></td>
            </tr>
            <tr>
                <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/Angular_full_color_logo.svg"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/Angular_full_color_logo.svg" alt="Angular" width="36"></a> <strong>Angular</strong></td>
                <td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Navigate to the following location to create a new repository:</td>
		<td align="center"><a href="https://github.com/new?template_name=angular-basic&template_owner=staticwebdev" rel="nofollow"><img alt="Static Badge" src="https://img.shields.io/badge/https%3A%2F%2Fgithub.com%2Fstaticwebdev%2Fangular-basic%2Fgenerate?color=blue&link=https%3A%2F%2Fgithub.com%2Fnew%3Ftemplate_name%3Dvanilla-basic%26template_owner%3Dstaticwebdev" alt="Create a repository" data-canonical-src="https://github.com/new?template_name=angular-basic&template_owner=staticwebdev" style="max-width: 100%;"></a></td>
		<td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Name your repository <strong>my-first-static-web-app</strong></td>
            </tr>
            <tr>
                <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/Blazor.png"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/Blazor.png" alt="Blazor" width="36"></a> <strong>Blazor</strong></td>
                <td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Navigate to the following location to create a new repository:</td>
		<td align="center"><a href="https://github.com/new?template_name=blazor-basic&template_owner=staticwebdev" rel="nofollow"><img alt="Static Badge" src="https://img.shields.io/badge/https%3A%2F%2Fgithub.com%2Fstaticwebdev%2Fblazor-basic%2Fgenerate?color=blue&link=https%3A%2F%2Fgithub.com%2Fnew%3Ftemplate_name%3Dvanilla-basic%26template_owner%3Dstaticwebdev" alt="Create a repository" data-canonical-src="https://github.com/new?template_name=blazor-basic&template_owner=staticwebdev" style="max-width: 100%;"></a></td>
		<td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Name your repository <strong>my-first-static-web-app</strong></td>
            </tr>
            <tr>
                <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/React-icon.svg"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/React-icon.svg" alt="React" width="36"></a> <strong>React</strong></td>
                <td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Navigate to the following location to create a new repository:</td>
		<td align="center"><a href="https://github.com/new?template_name=react-basic&template_owner=staticwebdev" rel="nofollow"><img alt="Static Badge" src="https://img.shields.io/badge/https%3A%2F%2Fgithub.com%2Fstaticwebdev%2Freact-basic%2Fgenerate?color=blue&link=https%3A%2F%2Fgithub.com%2Fnew%3Ftemplate_name%3Dvanilla-basic%26template_owner%3Dstaticwebdev" alt="Build &amp; Test" Create a repository" data-canonical-src="https://github.com/new?template_name=react-basic&template_owner=staticwebdev" style="max-width: 100%;"></a></td>
		<td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Name your repository <strong>my-first-static-web-app</strong></td>
            </tr>
            <tr>
                <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/vue.js-logo-brandlogo.net_-512x512.png"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/vue.js-logo-brandlogo.net_-512x512.png" alt="Vue" width="36"></a> <strong>Vue</strong></td>
                <td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Navigate to the following location to create a new repository:</td>
		<td align="center"><a href="https://github.com/new?template_name=vue-basic&template_owner=staticwebdev" rel="nofollow"><img alt="Static Badge" src="https://img.shields.io/badge/https%3A%2F%2Fgithub.com%2Fstaticwebdev%2Fvue-basic%2Fgenerate?color=blue&link=https%3A%2F%2Fgithub.com%2Fnew%3Ftemplate_name%3Dvanilla-basic%26template_owner%3Dstaticwebdev" alt="Create a repository" data-canonical-src="https://github.com/new?template_name=vue-basic&template_owner=staticwebdev" style="max-width: 100%;"></a></td>
		<td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Name your repository <strong>my-first-static-web-app</strong></td>
            </tr>
        </tbody>
    </table>
</body>
</html>


> **Note**
> <br>
> If you choose to not use a specific framework (<strong>No Framework</strong> option), please be advised that Azure Static Web Apps requires at least one HTML file to create a web app. The repository you create in this step includes a single <i>index.html</i> file.

Select <strong>Create repository.</strong>
<br>
<img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/create-repo.png" alt="Clone repo">


## Clone the repository
With the repository created in your GitHub account, clone the project to your local machine using the following command.
``` bash
git clone https://github.com/<YOUR_GITHUB_ACCOUNT_NAME>/my-first-static-web-app.git
```
Make sure to replace <strong><YOUR_GITHUB_ACCOUNT_NAME></strong> with your GitHub username.

Next, open Visual Studio Code and go to <strong>File > Open Folder</strong> to open the cloned repository in the editor.

## Install Azure Static Web Apps extension

If you don't already have the [Azure Static Web Apps extension for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-azurestaticwebapps) extension, you can install it in Visual Studio Code.

<ol>
	<li>Select <b>View > Extensions.</b></li>
	<li>In the <b>Search Extensions in Marketplace</b>, type <b>Azure Static Web Apps.</b></li>
	<li>Select <b>Install</b> for <b>Azure Static Web Apps.</b></li>
</ol>

## Create a static web app
<ol>
	<li>Inside Visual Studio Code, select the Azure logo in the Activity Bar to open the Azure extensions window.</li>
	<img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/az-black-logo.png" alt="Azure small black logo">
	<br>
	<a>
	<b>Note</b>
		<br>
	You are required to sign in to Azure and GitHub in Visual Studio Code to continue. If you are not already authenticated, the extension prompts you to sign in to both services during the creation process.
	</a>
	<li>Select <kbd>F1</kbd> to open the Visual Studio Code command palette.</li>
	<li>Enter <strong>Create static web app</strong> in the command box.</li>
	<li>Select <i>Azure Static Web Apps: Create static web app....</i></li>
	<li>Select your Azure subscription.</li>
	<li>Enter <strong>my-first-static-web-app</strong> for the application name.</li>
	<li>Select the region closest to you.</li>
	<li>Enter the settings values that match your framework choice.</li>
	<br>
	<table>
        <thead>
            <tr>
                <th align="center">Framework</th>
		<th align="center">Setting</th>
		<th align="center">Value</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a> <strong>No Framework</strong></td>
                <td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Framework</td>
		<td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Select <strong>Custom</strong></td>
            </tr>
	    <tr>
                <td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a> <strong>No Framework</strong></td>
                <td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Location of application code</td>
		<td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Enter <code>/src</code></td>
            </tr>
	     <tr>
                <td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a> <strong>No Framework</strong></td>
                <td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Build location</td>
		<td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Enter <code>/src</code></td>
            </tr>
            <tr>
                <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/Angular_full_color_logo.svg"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/Angular_full_color_logo.svg" alt="Angular" width="36"></a> <strong>Angular</strong></td>
                <td><a target="_blank" rel="noopener noreferrer" alt="Angular" style="max-width: 100%;"></a>Framework</td>
		<td><a target="_blank" rel="noopener noreferrer" alt="Angular" style="max-width: 100%;"></a>Select <strong>Angular</strong></td>
            </tr>
	    <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/Angular_full_color_logo.svg"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/Angular_full_color_logo.svg" alt="Angular" width="36"></a> <strong>Angular</strong></td>
                <td><a target="_blank" rel="noopener noreferrer" alt="Angular" style="max-width: 100%;"></a>Location of application code</td>
		<td><a target="_blank" rel="noopener noreferrer" alt="Angular" style="max-width: 100%;"></a>Enter <code>/</code></td>
            </tr>
	    <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/Angular_full_color_logo.svg"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/Angular_full_color_logo.svg" alt="Angular" width="36"></a> <strong>Angular</strong></td>
                <td><a target="_blank" rel="noopener noreferrer" alt="Angular" style="max-width: 100%;"></a>Build location</td>
		<td><a target="_blank" rel="noopener noreferrer" alt="Angular" style="max-width: 100%;"></a>Enter <code>dist/angular-basic</code></td>
	    </tr>
            <tr>
                <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/Blazor.png"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/Blazor.png" alt="Blazor" width="36"></a> <strong>Blazor</strong></td>
                <td><a target="_blank" rel="noopener noreferrer" alt="Blazor" style="max-width: 100%;"></a>Framework</td>
		<td><a target="_blank" rel="noopener noreferrer" alt="Blazor" style="max-width: 100%;"></a>Select <strong>Blazor</strong></td>
            </tr>
	    <tr>
                <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/Blazor.png"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/Blazor.png" alt="Blazor" width="36"></a> <strong>Blazor</strong></td>
                <td><a target="_blank" rel="noopener noreferrer" alt="Blazor" style="max-width: 100%;"></a>Location of application code</td>
		<td><a target="_blank" rel="noopener noreferrer" alt="Blazor" style="max-width: 100%;"></a>Enter <code>client</code></td>
            </tr>
	    <tr>
                <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/Blazor.png"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/Blazor.png" alt="Blazor" width="36"></a> <strong>Blazor</strong></td>
                <td><a target="_blank" rel="noopener noreferrer" alt="Blazor" style="max-width: 100%;"></a>Build location</td>
		<td><a target="_blank" rel="noopener noreferrer" alt="Blazor" style="max-width: 100%;"></a>Enter <code>wwwwroot</code></td>
            </tr>
            <tr>
                <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/React-icon.svg"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/React-icon.svg" alt="React" width="36"></a> <strong>React</strong></td>
                <td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Framework</td>
		<td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Select <strong>React</strong></td>
            </tr>
		<tr>
                <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/React-icon.svg"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/React-icon.svg" alt="React" width="36"></a> <strong>React</strong></td>
                <td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Location of application code</td>
		<td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Enter <code>/</code></td>
            </tr>
		<tr>
                <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/React-icon.svg"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/React-icon.svg" alt="React" width="36"></a> <strong>React</strong></td>
                <td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Build location</td>
		<td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Enter <code>build</code></td>
            </tr>
            <tr>
                <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/vue.js-logo-brandlogo.net_-512x512.png"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/vue.js-logo-brandlogo.net_-512x512.png" alt="Vue" width="36"></a> <strong>Vue</strong></td>
                <td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Framework</td>
				<td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Select <strong>Vue.js</strong></td>
            </tr>
		  <tr>
                <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/vue.js-logo-brandlogo.net_-512x512.png"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/vue.js-logo-brandlogo.net_-512x512.png" alt="Vue" width="36"></a> <strong>Vue</strong></td>
                <td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Location of application code</td>
				<td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Enter <code>/</code></td>
            </tr>
		  <tr>
                <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/vue.js-logo-brandlogo.net_-512x512.png"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/vue.js-logo-brandlogo.net_-512x512.png" alt="Vue" width="36"></a> <strong>Vue</strong></td>
                <td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Build location</td>
				<td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a>Enter <code>dist</code></td>
            </tr>
        </tbody>
    </table>
	<li>Once the app is created, a confirmation notification is shown in Visual Studio Code.</li>
	<br>
 	<img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/vs-1.png" alt="vs-1">
	<br>
	If GitHub presents you with a button labeled <strong>Enable Actions on this repository</strong>, select the button to allow the build action to run on your repository.
	<br>
	As the deployment is in progress, the Visual Studio Code extension reports the build status to you.
	<br>
	<img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/vs-2.png" alt="vs-2">
	<br>
	Once the deployment is complete, you can navigate directly to your website.
	<br>
	<li>To view the website in the browser, right-click the project in the Static Web Apps extension, and select <strong>Browse Site.</strong></li>
	<br>
	<img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/vs-3.png" alt="vs-3">
</ol>
<br>

## Clean up resources
<br>

If you're not going to continue to use this application, you can delete the Azure Static Web Apps instance through the extension.
<br>
In the Visual Studio Code Azure window, return to the <i>Resources</i> section and under <i>Static Web Apps</i>, right-click <strong>my-first-static-web-app</strong> and select <strong>Delete</strong>.

## Before cleaning up your resources...
<ol>
	<li>Verify your webapps's settings</li>
	<img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/vs-1.png" alt="vs-1">
	<li>...And why not? ... Visit your newly created site!</li
        <img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/vs-1.png" alt="vs-1">
</ol>
