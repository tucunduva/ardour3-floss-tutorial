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

In order to make or propose edits, uou will need to create a GitHub account (http://gihub.com)

## Submtting an an issue

An issue can be anything: reporting a typo, a mistake, an outdated passage; or any suggestions for improving the content and structure of the tutorial. This can be done directly through your browser, nothing else is needed.

1. Log in to your GitHub account.

2. Go to https://github.com/brunoruviaro/ardour3-floss-tutorial

3. On the right side column, click on "Issues"

4. Click on the green button "New Issue"

5. Give it a straightforward title, and describe the issue in details in the comment section.

### TIPS

* Always specify the name of the page (post title) you are referring to. For example, *"In the Recording Audio section..."*

* Before submitting a new issue, take a look at existing ones. Perhaps you will find that your idea or suggestion has already been posted by someone else. In this case, feel free to add a comment to that existing thread, instead of opening a duplicate issue.

* Submitting an issue is the easiest way to contribute: you just post your suggestion or idea and I'll review and fix the issue as appropriate.

* If you have a little more experience with GitHub (or are willing to learn it), you can do more than just submitting issues. For example, you could edit the page yourself and propose the change ("pull request") to be included in the tutorial ("merged").


## Editing pages on your browser

Another good way of proposing changes (like fixing a typo or a link) is to edit a post directly on the GitHub website. All the text lives inside the **_post** folder in the repository (yes, the one starting with an underline character, not just **post**). Simply follow these steps:

1. Go to https://github.com/brunoruviaro/ardour3-floss-tutorial/tree/gh-pages/_posts and find the section you want to edit. For example, the text for the section "Using Automation" is in the file named **2014-07-15-using-automation.md**.

2. Click on the file name to see its content.

3. In the header portion of that page, you will see the icon of a little pencil to the right of the button "History". Click on the little pencil.

4. GitHub will show you a message saying something like *"You're editing a file in a project you don't have write access to. We've created a fork of this project for you to commit your proposed changes to. Submitting a change to this file will write it to a new branch in your fork, so you can send a pull request."* That is all good and fine. It just means it created a working copy ("fork") of the tutorial in your own GitHub account, and you will be editing *that* copy instead. Only at the end of the process you will propose that change to my original repository ("pull request")  Go to next step.

5. You can now edit the raw text for that file. Find the paragraph you want to edit, and type your changes right in. Be careful not to change anything else by mistake.

6. Once you are finished, scroll down all the way to the bottom of the page to the "Propose file change" part.

7. Write a short descriptive title (for example, "Fix typo in Recording Audio), and optionally explain the change in the comment box.

8. Click on the green button, "Propose file change". You will be directed to another page to confirm; we are not done yet.

9. In the following page, you will see the change you are proposing, and a green button "Create pull request". Click on this button to send the proposal to me. You will have another chance to review you title and description of the proposal. Click on "Create pull request" to confirm.

10. You are done! I will receive the proposal, review it, and merge it to the published tutorial if appropriate.

## Advanced editing

You can do quite a lot of editing and writing directly from your browser using the method outlined above. For more extensive contributions, however, a common workflow is to clone the GitHub repository on your computer, make changes locally, preview them with Jekyll, and later create a pull request. The description below assumes you are minimally comfortable using the command line from a terminal. It also assumes you have successfully installed jekyll to preview changes locally.

Basic steps:

* Log in to your GitHub account and go to

`https://github.com/brunoruviaro/ardour3-floss-tutorial`

* **Fork** your own copy of the repository to your account (Click on the Fork button on the upper right corner). You will be directed to your own fork of the tutorial:

`https://github.com/yourname/ardour3-floss-tutorial`

Your URL will have your own user name in place of "youname".

* Clone your forked repository on your computer:

`
git clone https://github.com/yourname/ardour3-floss-tutorial.git
`

* Go into the newly cloned directory:

`cd ardour3-floss-tutorial/`

* Start jekyll for a preview of the cloned website:

`jekyll serve --watch`

* Open a browser and go to http://localhost:4000 to see the preview.

* Open your favorite text editor, open a post from the **_posts** folder to make edits. You may also save as from an existing file to start with a template. Save it with same name convention as the others (the earlier the post date, the more to the bottom of Table of Contents).

* After finishing an edit, add and commit from the terminal. For example, after I first created this file, I went to the terminal and ran these two lines:

`git add 2014-04-20-how-to-contribute.md`

`git commit -m "Add new post"`

* At this point you should be able to preview the new page locally, that is, in your browser window. For example, when after add and commmit for this new "how-to-contribute" page, I was able to preview it at http://localhost:4000/how-to-contribute/.

* Finally, after previewing the change and confirming it all looks good, push the change to your online repository:







### Header

The first thing inside a post file should always be the header:
```
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
```

You should change the title and the tags field. By convention, the title field and the file name should match. For example, the title above is "How to Contribute", and the file name is **2014-04-20-how-to-contribute.md**.

The tags field determines where in the table of contents that page will show up.


### Footer

I have included something like this at the end of every post:
```
Next: [SAVING A TEMPLATE](../saving-a-template)
```

The uppercase word in square brackets is the name of the next section (as shown in the Table of Contents), and the shortcut path in parentheses is the title of the page. Simply change it accordingly on each newly created page.


### Images

Images should be saved in the **images** folder, and linked as:

`![template1]({{ site.url }}/images/Ardour3_Save_Template1.png)`

`![limiter]({{ site.url }}/images/Ardour3_Limiter_Fast_Lookahead.png)`

...where the word in square brackets is just a short word describing the image, and `blah.png` is the exact file name. Nothing else should be changed.


### Jekyll

...UNFINISHED SECTION...
...in progress...

Jekyll can render to html _sites but this content is not checked into git and github does not need it to be rendered. They will render using their own Jekyll anytime you push to the repo.
Jekyll
Github Flavored Markdown
Check out this repository, install gem and jekyll (plenty of help online) and start up the server to view changes in preview mode:
jekyll serve --watch


It is written in GitHub markdown, which means there is a specific syntax to indicate titles, formatting, etc (see https://help.github.com/articles/markdown-basics/).

Learn more about GitHub work flow in the browser: https://github.com/blog/1557-github-flow-in-the-browser














**Appendices:**
[FURTHER HELP](../further-help)   ||
[GLOSSARY](../glossary)   ||
[LINKS](../links)   ||
[CREDITS](../credits)
