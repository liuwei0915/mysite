---
title: "Blog0 - Hugo Basics"
date: 2021-09-05T00:38:13-07:00
---
## what is the hugo?
   Hugo is a fast and modern static site generator written in Go, and designed to make website creation fun again.
    Hugo is a general-purpose website framework. Technically speaking, Hugo is a static site generator. Unlike systems that dynamically build a page with each visitor request, Hugo builds pages when you create or update your content. Since websites are viewed far more often than they are edited, Hugo is designed to provide an optimal viewing experience for your websitebs end users and an ideal writing experience for website authors.
## How to QUICK start hugo on MAC?
   ### Step 1: Install Hugo        
            Simply type command 'brew install hugo' or 'port install hugo'
            To verify your installation, type 'hugo version'
   ### Step 2: Create a New Site
            'hugo new site quickstart'
   ### Step 3: Add a Theme
            download the theme from GitHub and add it to your sitebs themes directory
            command: cd quickstart
                     git init
                     git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke
   ### Step 4: Add Some content
            You can manually create content files (for example as content/<CATEGORY>/<FILE>.<FORMAT>) and provide metadata in them, however you can use the new command to do a few things for you (like add title and date)
            hugo new posts/my-first-post.md
            then you can use editor like vi, vim or nano to create the content
   ### Step 5: start the Hugo Server
            Now, start the Hugo server with drafts enabled
            hugo server -D
            Feel free to edit or add new content and simply refresh in browser to see changes quickly (You might need to force refresh in webbrowser, something like Ctrl-R usually works).
   ### Step 6: Customize the Theme
            Site Configuration 
            Open up config.toml in a text editor:
                baseURL = "https://example.org/"
                languageCode = "en-us"
                itle = "My New Hugo Site"
                theme = "ananke"
            Replace the title above with something more personal. Also, if you already have a domain ready, set the baseURL. Note that this value is not needed when running the local development server.
   ### Step 7: Build static pages 
            It is simple. Just call:
                hugo -D
            Output will be in ./public/ directory by default (-d/--destination flag to change it, or set publishdir in the config file).

