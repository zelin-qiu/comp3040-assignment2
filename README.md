# How to Host Your Resume on Github Pages <br />
Github is a website collaboration community with a variety of mechanisms for everyone to work with you to contribute to the project. This readme file is written for people who have no experience in Github and Jekyll, but have some knowledgement about Atom and Markdown. In this readme file, you will learn how to ues Github to host your resume with a Jekyll theme. <br />
<hr>

## Prerequisites <br />
* a resume written in markdown (you can use atom to do that) <br />
* a Github account <br />

<hr>

## Step 1: Create a new repository <br />
1. First of all, clicking "start a project" to begin the trail. <br />
<div align=center><img width="450" height="150" src="https://github.com/zelin-qiu/comp3040-assignment2/raw/master/img/startaproject.png"/></div> <br />


2. Now, we need to create a repository in this page, using it to hold all files of your project. <br />
<div align=center><img width="545" height="405" src="https://github.com/zelin-qiu/comp3040-assignment2/raw/master/img/createpage.png"/></div> <br />

3. Giving your repository a short and clear name. <br />
<div align=center><img width="440" height="125" src="https://github.com/zelin-qiu/comp3040-assignment2/raw/master/img/giphy.gif"/></div> <br />

4. Select **Public** and **Initialize this repository with a README**. <br />
<div align=center><img width="450" height="150" src="https://github.com/zelin-qiu/comp3040-assignment2/raw/master/img/public.png"/></div> <br />

5. Click **Create repository**.
<div align=center><img width="450" height="50" src="https://github.com/zelin-qiu/comp3040-assignment2/raw/master/img/confirm.png"/></div> <br />

6. You have your repository now! <br />

<hr>

## Step 2:  Upload your resume <br />
1. First, go into your repository page and click the **Upload files** button. <br />
<div align=center><img width="480" height="300" src="https://github.com/zelin-qiu/comp3040-assignment2/raw/master/img/upload%20file.png"/></div> <br />

2. Drag your resume file to file adding area. <br />
<div align=center><img width="480" height="215" src="https://github.com/zelin-qiu/comp3040-assignment2/raw/master/img/giphy2.gif"/></div> <br />

3. Click **Commit changes** button at botton. <br />
<div align=center><img width="450" height="35" src="https://github.com/zelin-qiu/comp3040-assignment2/raw/master/img/commit.png"/></div> <br />

4. Now, you have successfully uploaded your resume. <br />

<hr>

## Step 3: Set your GitHub Pages <br />
### When you have uploaded your resume you need a web page to show it. So you need a GitHub Pages to host your resume. <br />
1. First, go into your repository page and click **settings** button. <br />
<div align=center><img width="450" height="100" src="https://github.com/zelin-qiu/comp3040-assignment2/raw/master/img/settings.png"/></div> <br />

2. Scroll down to "GitHub Pages" section. <br />
<div align=center><img width="450" height="170" src="https://github.com/zelin-qiu/comp3040-assignment2/raw/master/img/scroll%20down.png"/></div> <br />

3. Choose "master branch" in Source. <br />
<div align=center><img width="450" height="200" src="https://github.com/zelin-qiu/comp3040-assignment2/raw/master/img/select%20branch.png"/></div> <br />

4. Click **Change theme** button. Using Theme Chooser to select a theme for your resume. <br />
<div align=center><img width="450" height="60" src="https://github.com/zelin-qiu/comp3040-assignment2/raw/master/img/change%20theme.png"/></div> <br />

5. Choose your the theme you like, and click **Select theme**. <br />
<div align=center><img width="100" height="30" src="https://github.com/zelin-qiu/comp3040-assignment2/raw/master/img/select%20button.png"/></div> <br />

6. This is your Github Pages link, click it to check if it works. <br />
<div align=center><img width="450" height="200" src="https://github.com/zelin-qiu/comp3040-assignment2/raw/master/img/link.png"/></div> <br />

<hr>

## Step 4: Show your resume on your GitHub Pages <br />
### GitHub Pages show readme file automatically, so you need to change something to make sure your resume will be shown on Github Pages. <br />
1. Go into your repository page, <br />
 * if there is a **_config.yml** file in your file list, click it and add following code into it. <br />
 * if no **_config.yml** file in your file list, then create a new file name **_config.yml** and copy and paste following code into it. <br />
 
```
plugins:
  - jekyll-relative-links
relative_links:
  enabled: true
  collections: true
include:
  - CONTRIBUTING.md
  - README.md
  - LICENSE.md
  - COPYING.md
  - CODE_OF_CONDUCT.md
  - CONTRIBUTING.md
  - ISSUE_TEMPLATE.md
  - PULL_REQUEST_TEMPLATE.md
```
2. Rename your resume file to **index.md** <br />

3. Your GitHub Pages will show your resume when you refresh it. <br />

<hr>

## Step 5: change your theme by forking (optional)<br />
### You can change your theme by Theme Chooser (Step3 NO.5) or forking an existing theme. <br />
1. Using search bar to find a theme that interests you. For example, I search hack theme here. <br />
<div align=center><img width="450" height="100" src="https://github.com/zelin-qiu/comp3040-assignment2/raw/master/img/searchtheme.png"/></div> <br />

2. Choose the best match one. <br />
<div align=center><img width="450" height="200" src="https://github.com/zelin-qiu/comp3040-assignment2/raw/master/img/bestmatch.png"/></div> <br />

3. Click **Fork** button at right-top corner. <br />
<div align=center><img width="450" height="130" src="https://github.com/zelin-qiu/comp3040-assignment2/raw/master/img/forkbutton.png"/></div> <br />

4. Now, you have got a copy of this theme file. Find **_config.yml** in this theme file list, and click it. <br />
<div align=center><img width="450" height="185" src="https://github.com/zelin-qiu/comp3040-assignment2/raw/master/img/link.png"/></div> <br />

5. Copy the line that starts with "theme". <br />
<div align=center><img width="500" height="150" src="https://github.com/zelin-qiu/comp3040-assignment2/raw/master/img/line.png"/></div> <br />

6. Go back to your resume repositories, and overwrite the line that starts with "theme" in your **_config.yml** file. Also, click commit changes button when you finished. <br />
<div align=center><img width="550" height="175" src="https://github.com/zelin-qiu/comp3040-assignment2/raw/master/img/giphy3.gif"/></div> <br />

7. You have changed your resume theme now. <br />

<hr>

## Resources: <br />
* Introduction about Github Pages: <https://help.github.com/en/categories/working-with-github-pages> <br />
* Introduction about Github Flavored Markdown: <https://github.github.com/gfm/> <br />

<hr>

## Authors and Acknowledgment <br />
* Template author: <br />
  * Zelin <br />
* Group members: <br />
  * Swetul <br />
  * Darnell <br />

<hr>

## FAQs: <br />
* Why didn't my Github Pages change after I modified it in my template? <br />
* It takes a little time to upload, you can try again in five minutes. <br />
* Can I have more than one Github Pages? <br />
* Yes, just create another repository. 
