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
                <th align="center">Repo</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td><a target="_blank" rel="noopener noreferrer" alt="No Framework" style="max-width: 100%;"></a> <strong>No Framework</strong></td>
                <td align="center"><a href="https://dev.azure.com/mseng/PipelineTools/_build/latest?definitionId=7634" rel="nofollow"><img src="https://camo.githubusercontent.com/a7501ef8cf6294e9011b5c4efcc23280c16f472e8d5accd62819b093f8d94e43/68747470733a2f2f6465762e617a7572652e636f6d2f6d73656e672f506970656c696e65546f6f6c732f5f617069732f6275696c642f7374617475732f617a7572652d706970656c696e65732d7461736b732e63692d77696e646f7773" alt="Build &amp; Test" data-canonical-src="https://dev.azure.com/mseng/PipelineTools/_apis/build/status/azure-pipelines-tasks.ci-windows" style="max-width: 100%;"></a></td>
            </tr>
            <tr>
                <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/Angular_full_color_logo.svg"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/Angular_full_color_logo.svg" alt="Angular" width="36"></a> <strong>Angular</strong></td>
                <td align="center"><a href="https://dev.azure.com/mseng/PipelineTools/_build/latest?definitionId=7635" rel="nofollow"><img src="https://camo.githubusercontent.com/d1dae6ae68b6625a6ef27f4d354d79a6d56a7af4e7112b8ad54d5d85cab89e79/68747470733a2f2f6465762e617a7572652e636f6d2f6d73656e672f506970656c696e65546f6f6c732f5f617069732f6275696c642f7374617475732f617a7572652d706970656c696e65732d7461736b732e63692d6d61636f73" alt="Build &amp; Test" data-canonical-src="https://dev.azure.com/mseng/PipelineTools/_apis/build/status/azure-pipelines-tasks.ci-macos" style="max-width: 100%;"></a></td>
            </tr>
            <tr>
                <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/Blazor.png"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/Blazor.png" alt="Blazor" width="36"></a> <strong>Blazor</strong></td>
                <td align="center"><a href="https://dev.azure.com/mseng/PipelineTools/_build/latest?definitionId=7636" rel="nofollow"><img src="https://camo.githubusercontent.com/930bbab6753c486b6b2dc0bdd637b76f2d92b89f57f9e0649ec1d9173fabafc5/68747470733a2f2f6465762e617a7572652e636f6d2f6d73656e672f506970656c696e65546f6f6c732f5f617069732f6275696c642f7374617475732f617a7572652d706970656c696e65732d7461736b732e63692d6c696e7578" alt="Build &amp; Test" data-canonical-src="https://dev.azure.com/mseng/PipelineTools/_apis/build/status/azure-pipelines-tasks.ci-linux" style="max-width: 100%;"></a></td>
            </tr>
            <tr>
                <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/React-icon.svg"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/React-icon.svg" alt="React" width="36"></a> <strong>React</strong></td>
                <td align="center"><a href="https://dev.azure.com/mseng/PipelineTools/_build/latest?definitionId=7636" rel="nofollow"><img src="https://camo.githubusercontent.com/930bbab6753c486b6b2dc0bdd637b76f2d92b89f57f9e0649ec1d9173fabafc5/68747470733a2f2f6465762e617a7572652e636f6d2f6d73656e672f506970656c696e65546f6f6c732f5f617069732f6275696c642f7374617475732f617a7572652d706970656c696e65732d7461736b732e63692d6c696e7578" alt="Build &amp; Test" data-canonical-src="https://dev.azure.com/mseng/PipelineTools/_apis/build/status/azure-pipelines-tasks.ci-linux" style="max-width: 100%;"></a></td>
            </tr>
            <tr>
                <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/vue.js-logo-brandlogo.net_-512x512.png"><img src="https://github.com/jason-builds/my-first-static-web-app/blob/main/README_images/vue.js-logo-brandlogo.net_-512x512.png" alt="Vue" width="36"></a> <strong>Vue</strong></td>
                <td align="center"><a href="https://dev.azure.com/mseng/PipelineTools/_build/latest?definitionId=7636" rel="nofollow"><img src="https://camo.githubusercontent.com/930bbab6753c486b6b2dc0bdd637b76f2d92b89f57f9e0649ec1d9173fabafc5/68747470733a2f2f6465762e617a7572652e636f6d2f6d73656e672f506970656c696e65546f6f6c732f5f617069732f6275696c642f7374617475732f617a7572652d706970656c696e65732d7461736b732e63692d6c696e7578" alt="Build &amp; Test" data-canonical-src="https://dev.azure.com/mseng/PipelineTools/_apis/build/status/azure-pipelines-tasks.ci-linux" style="max-width: 100%;"></a></td>
            </tr>
        </tbody>
    </table>
</body>
</html>


> **Note**
> <br>
> If you choose to not use a specific framework (option 1), please be advised that Azure Static Web Apps requires at least one HTML file to create a web app. The repository you create in this step includes a single <i>index.html</i> file.

## Download

You can [download](https://github.com/amitmerchant1990/electron-markdownify/releases/tag/v1.2.0) the latest installable version of Markdownify for Windows, macOS and Linux.

## Emailware

Markdownify is an [emailware](https://en.wiktionary.org/wiki/emailware). Meaning, if you liked using this app or it has helped you in any way, I'd like you send me an email at <bullredeyes@gmail.com> about anything you'd want to say about this software. I'd really appreciate it!

## Credits

This software uses the following open source packages:

- [Electron](http://electron.atom.io/)
- [Node.js](https://nodejs.org/)
- [Marked - a markdown parser](https://github.com/chjj/marked)
- [showdown](http://showdownjs.github.io/showdown/)
- [CodeMirror](http://codemirror.net/)
- Emojis are taken from [here](https://github.com/arvida/emoji-cheat-sheet.com)
- [highlight.js](https://highlightjs.org/)

## Related

[markdownify-web](https://github.com/amitmerchant1990/markdownify-web) - Web version of Markdownify

## Support

<a href="https://www.buymeacoffee.com/5Zn8Xh3l9" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>

<p>Or</p> 

<a href="https://www.patreon.com/amitmerchant">
	<img src="https://c5.patreon.com/external/logo/become_a_patron_button@2x.png" width="160">
</a>

## You may also like...

- [Pomolectron](https://github.com/amitmerchant1990/pomolectron) - A pomodoro app
- [Correo](https://github.com/amitmerchant1990/correo) - A menubar/taskbar Gmail App for Windows and macOS

## License

MIT

---

> [amitmerchant.com](https://www.amitmerchant.com) &nbsp;&middot;&nbsp;
> GitHub [@amitmerchant1990](https://github.com/amitmerchant1990) &nbsp;&middot;&nbsp;
> Twitter [@amit_merchant](https://twitter.com/amit_merchant)








# React basic

[Azure Static Web Apps](https://docs.microsoft.com/azure/static-web-apps/overview) allows you to easily build [React](https://reactjs.org/) apps in minutes. Use this repo with the [React quickstart](https://docs.microsoft.com/azure/static-web-apps/getting-started?tabs=react) to build and customize a new static site.

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).
