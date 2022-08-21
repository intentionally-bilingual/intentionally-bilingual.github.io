# Nimke.nl Website

Welcome to the code of your website.
In here is the instruction to update things on the website.

The website is made using [hugo](https://gohugo.io).
This is a static site generator that uses markdowns.
If you need to update text you only need to though the markdown.

## Local testing

If you want to test the site locally [install hugo](https://gohugo.io/getting-started/installing/), open your terminal (powershell, cmd, bash, ect.), go to the root of this folder, and run `hugo server -D`.
You now have the site running at [localhost:1313](http://localhost:1313/).

## Updating text

To update text go the `/content` and locate the text you want to alter.
Every page has it own folder.

`_index.md`: Main text of this page.
The one `/content/_index.md` is for the main page (nimke.nl), `/content/contact/_index.md` is for contact page (nimke.nl/contact), and `/content/contact/_index.nl.md` is for the Dutch contact page (nimke.nl/nl/contact)

### Example

```
---
title: "This is the main tittle and what showns up if you list all items"
weight: 15 // lower weight means higher in the list (or farther to the left)
image: IMAGENAME.jpg // The image name in static\main_files\IMAGENAME.jpg use for lists
---

This is the first paragraph.
So is this text.
This is also first paragraph but a new line because the line above ended with 2 spaces

After a double enter a new paragraph starts

## This is a sub header

links:
[I am a link to google](google.com)

images:
![I am the alt text of the image for blind people or if the image does not load](/main_files/stage_5plus.png)

### I am a sub sub header

- This
- is
- a
- LIST!!!!

{{< columns >}}
{{< column "2/5" >}}
I am the first column with a width of 2/5 of the page
{{< /column >}}

{{< column "1/5" >}}
I am a smaller column but I have an image!
![Main page logo](/main_files/stage_5plus.png)
{{</ columns >}}

{{< column "2/5" >}}
I am the third and last column.
{{< /column >}}

{{</ columns >}}

```

# Launch a new version of the side

Create pull request to main and complete it.

# TODO

- Improve layout bullet point
- more blank space above a (+subsub) header, slightly less space under
- in the list: next level should be stripe, not dot. plus further to the right
- how do I do a part of text in smaller letters? (it's a sidenote)
- how do I do italics?
