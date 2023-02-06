# Forking this vault
---
If you want to create your own page using my template, follow the next steps. For a more minimal approach, follow [jobindj's Template](https://github.com/jobindj/obsidian-publish-mkdocs). 

### Features of this vault
- get the Obsidian/Roam style `[[wikilinks]]` from your vault in your published notes
- Toggle between light and dark mode
- Supports LaTeX, admonition style and all the basic Markdown syntax. 

### Quick start 
**Step 1 :** On GitHub, click the "fork" button on the top right of this repository's main page. 

**Step 2 :** **Give a name** to your repository. By default, your notes will be published at `<https://username.github.io/repo-name/>`

**Step 3 :** Clone the forked repository to your local machine using the command `git clone repo_url`

**Step 4 :** Go to `Settings > Pages` and select the **Source** as your `gh-pages` branch.


![[gh-pages.png]]

==Once above steps are done, wait for a couple of minutes or so for the website to build. You should see the following in your== `settings > Pages` ==and you can check if your website which looks like mine right now is build or not.==

![[gh-pages-link.png]]
!!! tip
	Even if it is not showing the website, do not worry, we will fix that later by re-initializing the repository from our local terminal. 


### Configuring your website
There are several files that contain references to this repository's name and URL, which is different to the new forked repository URL, since the username and the repository name might have changed. Also, you would like your notes to be shown in your website instead of mine. 

!!! tip
	We will make the changes locally and then push the changes to GitHub, but remember that, you can do everything from the website as well. 

1. **Enter into your newly forked repository, where you should see the similar folder structure as in this repository now.**
	1. `docs :` This will contain the folders which contains your notes in Markdown format, which will then appear on your website. For example, I have two folders which `Academics` and `LinuxStuffs` which has notes that you see on the website. ==Put your own notes after removing things related to my website==
	2. `index.md :` This is stored in `docs` folder, and it is your homepage. Edit it according to your choice. 
	3. `javascripts :` ==Do not delete this folder== as it contains the code required for LaTeX support on the website
	4. `Misc :` This folder can be deleted as it is catering to my workflow.
	5. `LiCENSE :` This contains the license. 
	6. `mkdocs.yml :` This is the most important file for this website, and it contains everything needed to customize and build the mkdocs pages. Try to not tamper with options which you might feel uncomfortable with. Having said that, we will edit this file for customizations later. 
	7. `README.md :` This is the README file for this repository. Edit it accordingly. 
	8. `requirements.txt :` This file contains all the dependencies required to build the website locally. You will need Python and pip installed in your system.


2. **Build website locally before deployment** 

In order to be able to build your site, some Python dependencies are needed. You can install them by running, 
```bash
pip install -r requirements.txt
```

!!! note "Removing the old commits"
	A way of doing so is removing the _.git_ folder and re-initializing the repository. Within the repository directory, do the following steps one by one.


```bash
rm -rf .git
git init
git config user.name {user}
git config user.email {email}
git remote add origin {your repo url}
git add .
git commit -m "Initial commit"
git push --force --set-upstream origin master # Force push
```
Now, your website should be up within a couple of minutes. Start making changes according to your needs. To build your website locally, simply use the following command(in the repo directory which contains the `mkdocs.yml` file)
```bash
mkdocs serve 
```
Then you will get a prompt in your terminal saying your website is hosted at `127.0.0.1:8000/` or something like this. You can open this link in your browser and your website will be visible there. You can see the changes to your website quickly here. 

**Customizing your website**

For this, we will edit the `mkdocs.yml` file. Since we will be making changes a lot, start the local build of your website and then make the changes. Saving the changes will build your website in a couple of seconds. Finally, when you are satisfied, you can push the changes to GitHub. Most of the fields are self-explanatory, and hence I will explain only a few of them. 

The section on `features` is the one you can play with while building locally. Uncomment the features you want to see or remove. For example, `navigation.tabs` will create a tabbed layout like a browser. If you do not like it, just comment it out. The section on `palette` can also be configured to change the look of the website. You can change the colors for light/dark mode here by changing the `primary` and `accent` subsections.  The features of Markdown like highlighting using (=), underlining using a caret(^) is set up in `markdown_extensions` section. Finally, the last section on `extra` can be used to set up social media links. You should definitely edit this part. 

!!! tip
	You should definitely checkout [Getting started - Material for MkDocs](https://squidfunk.github.io/mkdocs-material/getting-started/) for features and stuffs. 







