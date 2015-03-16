---
layout: post
title: "How to Contribute"
description:
comments: false
tags: [07 APPENDICES]
image:
  feature: Ardour3_Empty_Session_Transparent.png
  credit:  
  creditlink:  
---

Thanks for your interest in contributing to this tutorial. There are many ways to do so, from fixing a small typo to writing whole new sections.

In order to make or propose edits, you will need to create a GitHub account (http://gihub.com)

## Submtting an an issue

An issue can be anything: reporting a typo, a mistake, an outdated passage; or making any suggestions for improving the content and structure of the tutorial. This can be done directly through your browser; nothing else is needed.

1. Log in to your GitHub account.

2. Go to https://github.com/brunoruviaro/ardour3-floss-tutorial

3. On the right side column, click on "Issues"

4. Click on the green button "New Issue"

5. Give it a straightforward title, and describe the issue in details in the comment section.

### TIPS

* Always specify the name of the page (post title) you are referring to. For example, *"In the Recording Audio section..."*

* Before submitting a new issue, take a look at existing ones. Perhaps you will find that your idea or suggestion has already been posted by someone else. In this case, feel free to add a comment to that existing thread, instead of opening a duplicate issue.

* Submitting an issue is the easiest way to contribute: you just post your suggestion or idea and I'll review and fix the issue as appropriate.

* If you have a little more experience with GitHub (or are willing to learn it), you can do more than just submitting issues. For example, you could edit the page yourself and propose the change ("pull request") to be included in the tutorial ("merge").


## Editing pages in your browser

Another good way of proposing changes (like fixing a typo or a link) is to edit a post directly on the GitHub website. All the text lives inside the **_post** folder in the repository (yes, the one starting with an underline character, not just **post**). Simply follow these steps:

1. Go to https://github.com/brunoruviaro/ardour3-floss-tutorial/tree/gh-pages/_posts and find the section you want to edit. If this is your first time, you may want to try the file **2014-04-20-dummy-page.md** (that page was made just for testing, so no worries of messing it up).

2. Click on the file name to see its content.

3. In the header portion of that page, you will see the icon of a little pencil to the right of the button "History". Click on the pencil icon:
![littlepencil]({{ site.url }}/images/GitHub_Pencil.png)
4. GitHub will show you a message telling you it created a working copy ("fork") of the tutorial in your own GitHub account, and you will be editing *that* copy instead. That is all fine.  Go to next step.

5. You can now edit the raw text for that file. Find the line you want to edit, and type your changes right in. Be careful not to change anything else by mistake.

6. Once you are finished, scroll down all the way to the bottom of the page to the "Propose file change" part.
![propose]({{ site.url }}/images/GitHub_Propose.png)
7. Write a short descriptive title (for example, "Fix typo in Dummy Page"), and optionally explain the change in the comment box.

8. Click on the green button, "Propose file change". You will be directed to another page to confirm; we are not done yet.

9. In the following page, you will see the change you are proposing, and a green button "Create pull request". Click on this button to send the proposal to me. You will have another chance to review your title and description of the proposal. Click on "Create pull request" to confirm.

10. You are done! I will receive the proposal, review it, and merge it to the published tutorial if appropriate.

## Advanced editing

You can do quite a lot of editing and writing directly from your browser using the method outlined above. For more extensive contributions, however, a common workflow is to clone the GitHub repository on your computer, make changes locally, preview them with Jekyll, commit and push changes to your online repository, and later create a pull request. The description below assumes you are minimally comfortable using the command line from a terminal. It also assumes you have successfully installed Jekyll ([http://jekyllrb.com/docs/installation/](http://jekyllrb.com/docs/installation/)) to preview changes locally.

Basic steps:

* Log in to your GitHub account and go to [https://github.com/brunoruviaro/ardour3-floss-tutorial](https://github.com/brunoruviaro/ardour3-floss-tutorial).

* **Fork** your own copy of the repository to your account (Click on the Fork button on the upper right corner). You will be directed to your own fork of the tutorial: **https://github.com/yourname/ardour3-floss-tutorial**. The URL will have your own user name in place of "yourname".

* Clone your forked repository on your computer:

`
git clone https://github.com/yourname/ardour3-floss-tutorial.git
`

* Go into the newly cloned directory:

`cd ardour3-floss-tutorial/`

* Start Jekyll for a preview of the cloned website:

`jekyll serve --watch`

* Open a browser and go to **http://localhost:4000** to see the preview.

* Open a post from the **_posts** folder to make edits. You may also *save as* from an existing file to start with a template. Save it with same name convention as the others (the earlier the post date, the more to the bottom of Table of Contents).

* After finishing an edit, make sure the file is saved.

* At this point you should be able to preview the new page locally, that is, in your browser window. For example, if you make a change to the file **2014-04-19-dummy-page.md** and save it, you will be able able to preview it at **http://localhost:4000/dummy-page/**.

* Finally, after previewing the change and confirming it all looks good, `git add` and `git commit` the modified file. For example, after saving a change to the dummy page file, go to the terminal and run these two lines:

`git add 2014-04-19-dummy-page.md`

`git commit -m "Fix typo in dummy-page"`

* Now you can push the changes to your online repository:

`git push origin gh-pages`

* You can now go to your GitHub online repository **https://github.com/yourname/ardour3-floss-tutorial** ("yourname" is your actual user name), and you will see that the changes are reflected there. It is now time to create a pull request, that is, to propose the changes to the published tutorial (Bruno's repository).

* Click on "Pull requests" in the right side column, and create a new pull request. Click through the pages to confirm the creation of pull request.

* The change will be reviewed, discussed if necessary, and incorporated if appropriate. Thanks!




## Important information on posts

This section explains a few things you should know about the structure of a post and other miscellaneous items

### Header

The first thing inside a post file should always be the header:


\-\-\-  
layout: post  
title: "How to Contribute"  
description:  
comments: false  
tags: [07 APPENDICES]  
image:  
  feature: Ardour3_Empty_Session_Transparent.png  
  credit:  
  creditlink:  
\-\-\-


You should change the **title** and the **tags** field. By convention, the title field and the file name should match. For example, the title above is "How to Contribute", and the file name is **2014-04-20-how-to-contribute.md**.

The date in the beginning of the file name is used to determine order of posts in the Table of Contents. For example, the post **2014-04-19-dummy-page.md** shows up right below   **2014-04-20-how-to-contribute.md**.

The **tags** field determines where in the table of contents that page will show up.


### Footer

I have included something like this at the end of every post:

`Next: [SAVING A TEMPLATE](../saving-a-template)`

This is helpful to direct the reader to the next post in the tutorial sequence.

The uppercase word in square brackets is the name of the next section (as shown in the Table of Contents), and the shortcut path in parentheses is the title of the page. Simply change it accordingly on each newly created page.

If you create a new page that is not necessarily part of a sequence, you may want to write something like "See also" instead of "Next". Or you might just link back to the Table of Contents.


### Images

Images should be saved in the **images** folder, and linked in the body of the text like this:

\!\[template1]({\{ site.url \}}/images/Ardour3_Save_Template1.png)

...where the word in square brackets is just a short word describing the image, and **Ardour3_Save_Template1.png** is the exact file name. Nothing else should be changed. In short, to add a screenshot or image in the text:

* Copy the png or jpg file to the **images** folder. Make sure to add and commit to git.

* Refer to the file in your post using the syntax explained above.


>Note: Because the {site.url} bit creates an absolute path to the original repository, you won't be able to see the preview of your new images in Jekyll, unless you temporarily change the url in _config.yml to localhost:4000 and restart Jekyll.


### GitHub Markdown

This Ardour tutorial is written in GitHub-flavored Markdown, which means there is a specific syntax to indicate titles, formatting, etc. See [https://help.github.com/articles/markdown-basics/](https://help.github.com/articles/markdown-basics/) to learn more.

### Further Help with GitHub

Simple git guide for beginners:
[http://rogerdudler.github.io/git-guide/](http://rogerdudler.github.io/git-guide/)

Learn more about GitHub Work Flow in the browser:
[https://github.com/blog/1557-github-flow-in-the-browser](https://github.com/blog/1557-github-flow-in-the-browser)














**Appendices:**
[FURTHER HELP](../further-help)   ||
[GLOSSARY](../glossary)   ||
[LINKS](../links)   ||
[CREDITS](../credits)
