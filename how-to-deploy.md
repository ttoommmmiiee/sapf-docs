Deploy a Docusaurus Site to GitHub Pages

This page shows you how to run the initial deployment of your Docusaurus site to GitHub Pages using npm.
Before you begin

To configure and run the deployment, you’ll need:

    A local Docusaurus project
    A GitHub repository for your site
    Node.js version 18.0 or later

Install the gh-pages npm package

In your site directory, run this command:

npm install gh-pages --save-dev

Configure your site for GitHub Pages

Modify your docusaurus.config.js file:

const config = {
	url: 'https://USERID.github.io',  
	baseUrl: '/REPONAME/',  
	organizationName: 'USERID',  
	projectName: 'REPONAME',
 },

Replace the following:

    USERID: your GitHub username
    REPONAME: your Docusaurus GitHub repository name

Enable deployment for gh-pages

Add the following code to your package.json file:

"scripts": {
    "deploy": "gh-pages -d build",
}

Build and deploy your site to GitHub Pages

    Build your site:

npm run build

    Deploy your site:

npm run deploy

Configure the publishing source for your site

To configure the GitHub Pages branch for initial deployment, follow these steps:

    In your Docusaurus repository, go to Settings > Pages.
    Under Build Deployment > Branch, select the gh-pages branch.
