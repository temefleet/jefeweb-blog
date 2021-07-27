---
title: Rob Learns HTML - Lesson 1
description: This is my attempt to teach Rob to code
date: 2021-07-26
tags:
  - rob
  - code
  - learn
layout: layouts/post.njk
---

Hello there Rob, let's learn HTML. In this lesson you're going to start building a website by creating some content.

HTML stands for HyperText Markup Language. It is used to describe the content of your website. If you right-click this page and click **View Page Source**, you'll see the HTML of this page. It looks pretty confusing, but it's really not.

HTML has many different **tags** or **elements** used to describe the content. For example a paragraph looks like this:

```html
<p>Hello I am a paragraph</p>
```

Your paragraph is placed between <code class="language-">\<p></code> and <code class="language-">\</p></code>. This is the basic structure for most HTML tags except self-closing tags which we will cover later.

Every HTML document needs 3 tags: <code class="language-">\<html></code>, <code class="language-">\<head></code>, and <code class="language-">\<body></code>. For now we'll focus on the <code class="language-">\<body></code>. This is where the bulk of your time will be spent.

So let's start writing some code.

## Installing a text editor

A text editor is a program where we'll write our code. You could open up Notepad and write code there, but there are other programs which will give us features such as syntax highlighting so our code is easier to read, error checking, and many other features.

There are a ton of text editors to choose from, but we're going to use [Visual Studio Code](https://code.visualstudio.com/). So head on over there, download and install it.

## Creating a document

Somewhere on your file system create an HTML file. I don't actually remember how to do this on Windows, but I would start by opening up File Explorer, right-clicking and looking for something like _New File_ or _New Text Document_. If you can't find it, just search the web for 'Windows how to create file'.

You can name this file anything you want, but the extension (the bit after the .) must be html. For example: <code class="language-">cool.html</code>

Open this file with Visual Studio Code (hereby known as VSCode).

## Coding some content

You'll need some **boilerplate** to get started. Boilerplate just means some fundamental code that is needed before we can add our own code. This can be easily done in VSCode. Just type <code class="language-">html:5</code> and then hit <code class="language-">TAB</code>. Boom, you should have a bunch of code that looks like this:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
  
  </body>
</html>
```

If for whatever reason the shortcut didn't work, just copy and paste the code above.

The only **tag** in **head** we'll worry about now is **title**. Go ahead and change *Document* to the title of your website. You can name it whatever you want, this title will appear on the tab in the browser.

Next add a heading to the body. Heading tags are labeled **h1** to **h6** with **h1** being the most important heading and **h6** being the least important. Add a few headings inside the **body** of your document.

Whitespace (tabs, spaces, newlines...etc) will not effect how it looks on the page...

```html
<body>
  <h1>My awesome title</h1>
</body>
```

is the same as

```html
<body>
  <h1>
    My awesome title
  </h1>
</body>
```

and

```html
<body><h1>My awesome title</h1></body>
```

and even

```html
<body>
              <h1>
My awesome title</h1>


</body>
```

but even if the code works whichever way you write it, it's important that it's readable for humans. So usually we'd stick to one of the first 2 examples with each **nested** tag indented a bit further than the line before it.

## Adding an image

An image tag looks like this:

```html
<img src="path/to/image.jpeg" alt="A picture of me when I was younger" />
```

There are a couple of new things here. First of all the tag is **self closing**, meaning there is only the single **img** tag which is closed by the forward slash **/** before the **>**. Next this **element** has 2 **attributes**, **src** and **alt**. These are required for an image element.

The **src** attribute points to the image. It can be a local file on your computer, in which case you need to know where it is in relation to the html file you're working in. If it's in the same folder then you would just use the name of the image <code class="language-">src="picture-of-a-watermelon.jpeg"</code> or <code class="language-">src="grandma.png"</code>. If the file was in a folder called *images* you would write <code class="language-">src="images/grandma.png"</code>.

You can also point to an image on the internet. If you right-click on an image and select *Copy Image Link* or *Copy Image address* you can easily get the url of any image. Then simply paste it in the **src** like so <code class="language-">src="https://www.w3schools.com/w3css/img_snowtops.jpg"</code>

The **alt** attribute describes the image. This is useful in case the image cannot be found, and more importantly for accessibility. If somebody visits your site who is vision impaired the **alt** attribute describes the image.

## Viewing your beautiful hard work

To view your html document, you can double-click it or drag it into your browser of choice. Mine looks like this:

{% image "./img/rob1-1.jpg", "image of fake website", "600px" %}

...beautiful

## Homework

A huge part of programming is searching the internets for what you need. So that's what you'll be doing. Your website can be about anything you want. If you're struggling for ideas just make it a personal profile.

I want you to have a minimum of the following elements:
- 3 different headings
- 2 paragraphs
- an unordered list
- an ordered list
- 2 images
- an embedded youtube video
- some bold text
- some italic text
- a button (doesn't need to do anything)
- a link (also known as an anchor tag)

For all the ones I didn't teach you, you'll need to search (ie **html embed a youtube video**) the internets. Of course, I'm here to answer any questions.

When you're done copy and paste it to [PasteBin](https://pastebin.com/) click **Create New Paste** and send me the link.

I apologize for all the grammatical and spelling errors in this tutorial.

See you at hockey.
