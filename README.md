# Table of Contents

* [Purpose](#purpose)
* [Prerequisites](#prerequisites)
* [Instructions](#instructions)
* [Further resources/readings](#further-resourcereadings)
* [Frequently Asked Questions (FAQ)](#faq)
* [Credits](#credits)

# Purpose

The purpose of this README is to showcase how easy it is to host a static site generator. This will cater to those who have never hosted a website before and wants to start, as well as those who have never hosted a website with GitHub Pages before. 

With this README, I will go through the steps on how you too can host a website like [this one](https://kayerm.github.io/). 

# Prerequisites

1. You will need a [GitHub](https://github.com/) account. GitHub allows you to host one website with your github name. Choose one that applies to you:

    - [ ] **Log in to your account**. 
        * Make sure you don't have a website running already by typing this one your web browser [your_username].github.io
            * If an error code, 404 came up, that's good. 
            * If not, then delete that repository as it will conflict with that website.

    - [ ] **Create an account**.
        * Make sure the username you pick is what you want your website to be.

2. You will also need a place to edit your repository I like to use Visual Studio Code. 

    - [ ] **Download [Visual Studio Code](https://code.visualstudio.com/)**. If you are on Windows, the download button is right on top of the page. 

# Instructions

## Creating the Repository

1. Refer to the upper-right side of your screen. Click the **"+"** and select **New Repository**.

2. Under **Repository Name**, put [username].github.io. `username` should be what your username is on GitHub. For instance, my username is `kayerm`, therefore my Repository Name is `kayerm.github.io`.

3. READMEs allow for you to give some context about your website. Therefore, under the **Add README** switch, turn it **On**.

    ![Creating the repository picture](images/image_01.png)

    **NOTE**: _Since my website already exists after making this tutorial, `kayerm.github.io` is already made and taken by me. However, if it's your first time making your website, it should say "**`username.github.io` is available**."_

4. After comparing your screen with the website, your can click **Create respository**. 

5. You should now see a page similar to the page below. I will refer to this page as your "_Repository_."

    ![Respository image](images/image_02.png)

    **NOTE:** _Only difference is that you should only have a README.md. We will make these files later on._

6. On options on top, click on **Settings**.

    ![Settings in Repository](images/image_05.png)

7. With the options on the side, look for the **Code and automation** section, and click on the **Pages** tab. 

8. Under **Build and deployment**, the dropdown under **Source** should be **Deploy from a branch**. 

9. Under **Build and deployment**, the dropdown under **Branch** should be **None**. 

    ![Steps 8 and 9](images/image_06.png)

## Editing with Visual Studio Code (VSCode)

1. Assuming it's already downloaded, open **Visual Studio Code**.

2. On the top-left corner, click on **File**, **Open Folder**, and select the folder you want to download your repository in, then click **Select folder**. 

3. Once your folder is opened, click on **Terminal**, and then **New Terminal**. A new tab should open under your VSCode. 

    ![VSCode Terminal](images/image_03.png)

4. In your _repository_, you will see a dropdown named **Code**. Click on it and a link should appear. Copy it. 

    ![Code repository](images/image_04.png)

5. In your _terminal_, copy the following code below and then press **Enter**.

    ```
    git clone https://github.com/kayerm/kayerm.github.io.git
    ```
    **NOTE**: "https://github.com/kayerm/kayerm.github.io.git" should be what you copied from Number 4. 

6. To place your terminal into that repository, copy the following code below and then press **Enter**.

    ```
    cd .\kayerm.github.io\
    ```
    **NOTE**: If you only have your repository in your folder, you can also type `cd` and then **Tab**, then click **Enter**. 

## Making our First Page

1. In your VSCode, create a File named `_config.yml`. 

2. Open the file and type the code below. This will be the base of our website. 

    ```
    title: [Title of your website]
    description: [Summary/Purpose of what your website]
    theme: jekyll-theme-hacker
    ```
    **NOTE**: _The theme of your website can be changed. A list of themes are provided in the [further resources/readings](#further-resourcereadings) section._

3. On the top-right corner of the screen, click on **File** and then **Save**.

4. To create our first page, the page that people will see when they first go to your website, create another File named `index.md`.

5. Inside `index.md`, type the following header:

    ```
    ---
    layout: default
    title: "Main page"
    permalink: "/"
    ---
    ```
    To break everything down:

    * _Layout_ being _default_ means that we will let our chosen theme be our layout in our main page. 
    * _Title_ will be what is shown on your tab of where you are. 
        ![Name of tab](images/image_07.png)
    * _Permalink_ will be where the page is located. `/` means that this page will be seen in `https://kayerm.github.io/`, which is the landing page of your website.

6. Under the header of `index.md`, your can put whatever you'd like. As seem below, I added headers and hyperlinks to organize my data. 

    ![Main page in VSCode](images/image_08.png)

    **NOTE**: _If you are unfamiliar with Markdown, which the language above is written in, I recommend reading more about it in [further resource/readings](#further-resourcereadings) section._

## Adding More Pages

# FAQ

* Installing Jekyll

* What does the directory look like

# Further Resource/Readings

* View Markdown tutorials: **[Markdown tutorial](https://www.markdownguide.org/basic-syntax/)**
    * Everything you know about Markdown syntax and best practices when coding in Markdown. 

* View tutorials for Git: **[Git Tutorial with clone](https://earthdatascience.org/workshops/intro-version-control-git/basic-git-commands/)** and **[Git tutorial without clone](https://graphite.com/guides/git-add-commit-push)**
    * This will explain in detail what it means when we clone, pull, push, and commit code to our repository. 

* View more available themes: **[GitHub Page Themes](https://github.com/pages-themes)**
    * You can view what each theme looks like by clicking a theme you're interested in > Scrolling down to their README > find a hyperlink that says "_preview the theme to see what it looks like_."

* View examples of README: **[README examples](https://github.com/matiassingers/awesome-readme?tab=readme-ov-file)**
    * A README is very important to have in your GitHub respository. It explains what your website is about, how to check it out, and any comments you want to include but not on your website. 

# Credits

Credit goes to: 

* Group 11 (Mateo DeSousa and Andrew Driver) of the COMP 2600 class of Winter 2026.
* The authors of [GitHub Pages](https://docs.github.com/en/pages/quickstart) that helped me get started. 
* The creator of the Jekyll Hacker theme, Jason Costello. 