---
date: "2022-01-09T00:00:00+01:00"
draft: false
linktitle: Going Further
menu:
  example:
    parent: Going Further
    weight: 2
title: Customizing your site further
toc: true
type: book
weight: 2
---

Hi and welcome to the second part of the `{coursedown}` userguide! Since
this part is aimed at users wanting to go a little further, it will be
structured a little differently than other guides i.e. it will be a FAQ-type
post that will be extended as the writing of the documentation progresses.
We hope that the following lines will be helpful in your journey with
`{coursedown}`!

## Content

### What are these images on each class section?

These are "featured" images. You can find them in each post folder. To remove
them simply delete them from that folder. If you'd like to change them, simply
replace them with a new one and don't forget to call the new image
`featured.jpg`.

### Where do I add/remove/edit slides for my classes?

Currently, you can find the slides in the `static` folder. You'll be
able to edit them there. Simply follow the file structure of the ones already
present and link them on the corresponding "class post" you'll find in the
`content/post/yourclass/index.Rmarkdown` folder.

### Where do I add/remove/edit lab sessions?

Currently, you can find the lab sessions in the `static` folder. You'll be
able to edit them there. Simply follow the file structure of the ones already
present and link them on the corresponding "class post" you'll find in the
`content/post/yourclass/index.Rmarkdown` folder.

### Where do I add images?

Following Alison Hill's answer on [this issue](https://github.com/rstudio/blogdown/issues/45),
you should usually put images in the `static` folder since it's content will
be copied directly to the root of the `public` folder after running
`blogdown::build_site()`. For instance, the screenshots that illustrate the
user guide can be found in `static/media/courses/userguide`. They are then
referenced in the markdown document by typing
`![createrepository](/media/courses/userguide/yourimage.png)`.

## More customization !

### I don't like the 404 page, where can I change it?

The HTML code for the 404 page is in the `layouts` folder. Feel free to tweak
it to your liking!

### Where do I tweak the CSS?

The IHEID color theme lives in the `assets/scss/custom.scss` file where you
can tweak everything from shadows to colors of the elements on your site. These
can then be picked up by an HTML block you wrote or a standard one provided with
the Academic theme.

### I have a great idea for a custom HTML element. Where should it go?

Rule #1: **Never** change the `theme` folder since this is where the original
Academic theme lives. You should add your additional HTML elements in the
`layouts` folder just like we already did for the `courseinfo.html` file.
Note that these custom HTML elements use the Mustache logicless language to
carry over elements from various config files.


This post will be extended in the future! Suggestions in the form of a Github
issue are welcome!
