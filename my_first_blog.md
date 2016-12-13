# My first blog

## Introduction

In this lesson, you'll learn: 
- How to install Abe on your computer
- How to create an empty blog
- How to add a template in Abe
- How to make your template dynamic with text, image and rich content
- How to link your blog content between your pages
- Publish your blog on the web

## Prerequisites

- A minimal understanding of HTML
- NodeJS installed on your computer

## How to install Abe on your computer

Go in a terminal window and type:
``` npm i -g abe-cli ```

This command will install the last stable version of Abe. 

You're now ready to create blogs !

## How to create an empty blog

In a terminal window, where you want to create your blog directory, type:

``` abe create myBlog ```

``` cd myBlog ```

``` abe serve -i ```

A directory named myBlog is now created and ready, and the command ``` abe serve ``` launches a web server on port 3000 and start your browser on your blog.

> If you want to launch your blog on another port, do ```abe serve -p #port_number```

In your browser, this page is displayed:

The block on the left side gives you the ability to create content. But before being able to create content, you'll need a template. Any HTML template can be used.

## How to add a template in Abe

Abe uses regular HTML templates. You can grab or create any HTML5 template to create your blog. For a template to be able to work inside Abe, you'll to make sure of 2 things:
- The name of your template file will be used as the template name. ie. my_cool_template.html => name: my_cool_template. All the assets directories used in your template (js, css, images, ...) must be enclosed inside a directory named with your template name + "_files". ie. my_cool_template_files
- In your html template, make sure that your assets are linked in absolute format. ie. <script src="my.js"></script> becomes <script src="/my.js"></script>

Once your template is ready, put it + its assets directory in the directory "/templates" of your blog. Abe will automatically detect your changes in the directory /templates. Once done, refresh your browser. On the left side, you'll see that the dropwon list now contains an entry with the name of your template (ie. my_cool_template). 

You're ready to go !

Create a new content:
- Select a template in the drop down list
- Git your content a name
- Click on "create"

You'll see the Editor:

The editor is split into 2 parts:
- Left side: A form containing your content data is displayed
- right side: Your template appears !

## How to make your template dynamic with text, image and rich content

