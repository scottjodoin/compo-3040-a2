# Resume

## Purpose

This guide will walk you through the steps to upload a resume to your GitHub repository using Markdown, Jekyll theming, and GitHub pages. This guide will also make references to the suggestions as outlined in Etter's book, **Modern Technical Writing**. 

## Prerequisites

* A resume formatted in Markdown.
* A GitHub account and dedicated repository

## Instructions

### 1. **According to Etter: Use a lightweight markup language**

The first thing to do is to create a Markdown file `index.md`. This is the file that will be used to create your resume. See below for a link to the **Markdown Cheat sheet** in case this is your first time using Markdown. See **[Why is Markdown better than a word processor?](https://github.com/scottjodoin/scottjodoin.github.io#faq)** for more information on why you should use Markdown.

Here is a template you are free to use to structure your resume in Markdown. Add any extra sections as you need.

```
# YOUR NAME

## Your Role

## TECHNICAL SKILLS

* Technical skills

## RELEVANT WORK EXPERIENCE

### Work Experience Title
Work location, date range

* Description of work

## EDUCATION

### School Name
School location, date range

* Description of achievements

## VOLUNTEER EXPERIENCE

Volunteer location, date range

* Description of work

```

### 2. **According to Etter: Share / host documents on a distributed version control system**

Etter recommends that you use a version control system to manage your documents. This is a good way to ensure that your documents are always up-to-date. We recommend using GitHub.

Now that you have your resume in Markdown, you need to upload it to a GitHub repository
#### a. Create a GitHub repository for your resume in the following format: `username.github.io`.

#### b. Grab the link to your repository from the GitHub page

#### c. Download the repository in VS Code

Open up a new instance of VS Code and click **Clone a Git Repository**. Copy the link from the GitHub page and paste it into the **Repository URL** field. Click **Clone** and wait for the repository to download. You should see a new folder in your workspace.

#### d. Add your resume to the directory as `index.md`

#### e. Commit your changes.

#### f. Push your changes to your repository

In VS Code, click the **Git** tab, add a commit message and click **Sync now**. You should see a message that your changes have been pushed to your repository.

#### g. Open your GitHub repository in your browser and see that your file has successfully been uploaded

If you can't see your file, you may need to refresh the page.

### 3. **According to Etter: Format a document with a static site generator**

While styling with HTML and CSS can be fun, it can also tend to time consuming and detract from the actual work of writing. Etter recommends using a static site generator to create a website that is easy to read and navigate from the beautiful markdown you produced in an earlier step.

Jekyll is our tool of choice that will convert a Markdown document into a static site. While is possible to run Jekyll on your own machine, we will let GitHub pages take care of this for us.

#### a. Set up GitHub Pages for your repository
* From your GitHub repository, go to the **Settings** then **Pages** section.
* Choose the   **Main** or **Master** branch and **Save**.
* Choose a Jekyll theme that suits your fancy and commit the changes.

When you go back to your repository, you will find a new file called `_config.yml`. This file contains the configuration for your Jekyll site. So far, the file only contains the `theme:` setting.

#### b. Choose a more specific theme for your resume

If you want to see more Jekyll themes than the default ones that GitHub provides, you can visit the [Jekyll themes page](https://jekyllrb.com/docs/themes/) to see more. Each theme has a unique name, so when you find one you like, you can replace the `theme:` setting in `_config.yml` with the name of the theme you want and GitHub will take care of the rest.

#### c. Configure your Jekyll site
  
The `_config.yml` file contains a lot of settings that can be configured to your liking. Here are a few of the most important ones:

  * `title`: The title of your site that shows up in the tab of your browser.
  * `name`: The text that appears at the top of your site.
  * `theme`: This is the theme that you selected earlier.

Jekyll has a lot of other settings that you can configure as well. The settings that you can configure will depend on the theme you choose, and these settings are usually listed on the GitHub repository of the theme.

#### d. Update your site continually

Now that you have set up version control, whenever you want to update your resume, you can simply update the `index.md` file and commit your changes.


### Conclusion

Congrats! If you have followed the steps in this guide, you should have an easy-to-update resume that has been uploaded to GitHub, ready to be read by anyone. If you have any questions, feel free to reach out to me through my GitHub profile.

### More Resources

* [Markdown Tutorial](https://www.markdowntutorial.com/)
* [Markdown Cheatsheet](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf)
* [Andrew Etter's Book, Modern Technical Writing: An Introduction to Software Documentation](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)
* [COMP 3040 course guide at the University of Manitoba](https://aurora.umanitoba.ca/banprod/bwckctlg.p_disp_course_detail?cat_term_in=202210&subj_code_in=COMP&crse_numb_in=3040) 

## Authors and Acknowledgements

This resume and README was created by myself, Scott Jodoin in fulfillment of Assignment 2 from COMP 3040. The Jekyll theme [Slate](https://github.com/pages-themes/slate) used by this resume was created by [Ben Balter and the open source community](https://github.com/pages-themes/slate/graphs/contributors). My group members include: Kyle Calinisan, Raven Mico Carencia, Tahmidul Hasnain Zidaan, and Hao Qin. 


## FAQ

### Why is Markdown better than a word processor?

Markdown is simple and clean text content language designed for the web; it is all that it needs to be and nothing more. Did I mention that it is free? Markdown's bare-bones syntax makes it easy for writers to write, collaborate, and use version control. In contrast, word processors filled with print-formatting tools distract from the hard work of writing and restrict authors to use proprietary software, file formats, and collaboration tools. 

### Why is my resume not showing up?
  
Your resume could be not showing for a couple reasons. Did you forget to push your index.md file or _config.yml file? If you just pushed your code, try waiting a little bit; GitHub pages can take up to 20 minutes to deploy. You can view the deployment progress by following the **github-pages** under the Environments section on your respository's main page. 