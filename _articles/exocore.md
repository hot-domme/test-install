---
layout: article
category: article
subtitle:
topic: Computers
date: 27 jan 2021
tags: exocore remilia computers web
---

# The Exocore Package

![](/attachments/exocore.png)

## Executive Summary

Do you take notes, or conduct personal research? Do you output or collect text or image content in any form, such as a blog, poetry, diary or visual art? Do you intake any form of media, and want to catalogue your findings or thoughts? Do you forget information? The Exocore is a means to store and organize and publish such a bank of information in an easily navigable form.

The exocore comprises a set of a few programs and plugins, rolling them into a package which can be customized infinitely and modularly; without any technical knowledge it can still be made your own, and with even a touch of technical knowledge (particularly CSS or HTML facility) it can be made into anything at all.

Its online component is a scaffolding for a website, and its offline component (fully functional without the online) is a filing system for notes, written output, or other data. Out of the box, it's a local directory of folders and interacting files forming an empty template for a [zettelkasten](https://zettelkasten.de/introduction/)/wiki, a platform for longform articles, a library of documents, a gallery of images, and an automatically created daily note. Mix and match these features as you wish; they are fully modular and independent.

in future, these Exocores can comprise a webring linked by automatically updated network pages, as well as a [hyper-realtime IRC](https://xcela.org/#realtime-communicaiton) for which the Exocore will operate as a personal homepage. They can also feature things like an automatically updated 'latest posts' feed from all other (or selected) Exocores, or just 'related posts' (by [metadata](https://jekyllrb.com/docs/front-matter/) tags) from your own site.

As mentioned, a user would be free to use or not use any of these features, so if they want to create a self-hosted platform like Substack with no extra features, this is facilitated.

### User experience:

A user will download the package in the form of a Github repository template, which will live on their local machine as a directory that can be manually or automatically pushed (synced) via [git](https://git-scm.com) to a web domain, which will represent the documents in the directory after they are processed into an eaily-navigable and feature-rich website.

A user can get by just fine only interacting with simple plaintext [markdown](https://www.markdownguide.org) files, and can write posts and create hyperlinks between them, add pictures or PDFs and more, without going beyond in-text markdown syntax (read more about the Exocore's syntax [[syntax|here]]). They are also able to control how their generated website handles their documents in a human-readable [[start-here#Using Metadata|metadata section]] at the top of each post: tags, title, subtitle, categories, layouts, date, and any others that the user cares to add.

![](/attachments/girl-online.png){:.right}

Locally, the directory of notes (which will also be a git repository if you wish to publish as a website online) will be managed and maintained through a [VS Code](https://code.visualstudio.com) workspace. The recommended extensions for your workspace arrives as a package of two things:

1. A template directory including templates for simple creation of new markdown documents of different kinds (article, journal entry, wiki note, daily note), each treated differently in the rendering of your website.

2. A set of VSCode plugins which offer a suite of features for the user to add to their directory of posts by facilitating easy linking between notes, URL management, and many other features. The directory can be easily hosted for free with [Netlify](https://www.netlify.com), for which a setup guide is available [[installation-instructions#Publishing Your Exocore|here]].

### Jekyll
To view your site before it is pushed online, a user can set up their Exocore directory to build a local instance of the site with [Jekyll](https://jekyllrb.com). When publishing, Netlify runs Jekyll server-side, so running it locally produces the same site as will be published.

### Customizability

The stack is an open-source repo and a suite of open-source programs and plugins, and is therefore ultimately customizable. The level of customizability depends only on your technical know-how, but minimal learnings yield compounding rewards. Here is an idea of the level of control over your final website yielded by advancing levels of technical knowledge:

- **No technical knowledge:**
  - You can implement all of the above, and choose from a set of .CSS templates for your website to adjust its aesthetics. You can create posts, use the daily note functionality, store documents in the Library, create ZK notes and links between them, use backlinking, embed notes, and all other features mentioned above. In other words, all features are fully available with no technical knowledge. You should become acquainted with the Exocore's [[syntax]], but this is easy enough to guess at, or to learn in under half an hour. 

    For publishing, a very cursory knowledge of git will come in handy, but git has a helpful GUI, and Exocore [[installation-instructions#Publishing Your Exocore|documentation]] includes a guide on how to publish your site.
  
- **HTML and CSS**
  - You will be able to edit included stylesheets and HTML templates to create a site which looks any way that you wish. Both these languages are simple to learn, and even without learning them comprehensively a user can edit the provided templates and stylesheets to make major changes.  

- **Jekyll/Liquid**
  - You will be able to create logic functions to manipulate metadata stored in the markdown front matter, create custom menus or boxes with automatically generated content based on the front matter, assign your own custom front matter variables, and more. 

- **Ruby**
  - Learning Ruby is not at all necessary, but familiarity with it will facilitate you in packaging themes you have created for your exocore as Ruby Gems in case you would like to publish them for use by others. If you want to proliferate your particular model of the exocore, this is an easy way to package it.


## Full Tech Stack

- [VS Code](https://code.visualstudio.com) (and plugin package)
- [Git](https://git-scm.com) (for publishing)
- [Jekyll](https://jekyllrb.com) (optional)

**VSCode Plugins:**
- [Foam](https://marketplace.visualstudio.com/items?itemName=foam.foam-vscode)
- [Netlify](https://marketplace.visualstudio.com/items?itemName=shailen.netlify)
- [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)
- [Paste Image](https://marketplace.visualstudio.com/items?itemName=mushan.vscode-paste-image)
- [Spell Right](https://marketplace.visualstudio.com/items?itemName=ban.spellright)

[//begin]: # "Autogenerated link references for markdown compatibility"
[syntax|here]: syntax "Exocore Syntax Examples"
[start-here#Using Metadata|metadata section]: start-here "Start Here"
[installation-instructions#Publishing Your Exocore|here]: installation-instructions "Exocore Installation Instructions"
[syntax]: syntax "Exocore Syntax Examples"
[installation-instructions#Publishing Your Exocore|documentation]: installation-instructions "Exocore Installation Instructions"
[//end]: # "Autogenerated link references"