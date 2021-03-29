---
title: Kevin's cheatsheet
permalink: /guides/cheatsheet
breadcrumb: Kevin's cheatsheet
collection_name: guides
third_nav_title: 
published: true
---

# Guide Index

- [Introduction](#introduction)
- [What you will need](#what-you-will-need)
- [Headings](#headings)
- [Content Pages](#content-pages) (or Anchors/Bookmarks)
- [Plain text and formatting](#plain-text-and-formatting)
- [Hyperlinks](#hyperlinks)
- [Images](#images)
- [Videos](#videos)
- [Footnotes](#footnotes)
- [Tables](#tables)
- [KIV Content](#kiv-content)
- [Useful Websites for Reference](#useful-websites-for-reference)

## Introduction

This cheatsheet contains the markdown syntaxes you can use to copy directly into your Isomer pages.

The examples and descriptions should illustrate what it will appear like in your page.

The grey boxes `such as this one` will indicate the code you can copy. Copy everything inside the grey box to your Isomer page.

In Typora, the relevant syntax only appears when your cursor is in the respective portions of the text. So do not worry if the syntax is missing, or if the syntax suddenly appears when your cursor is in the respective text.

Do note also that what you see in Typora is not the same as what you will see in the Isomer site. What you are able to edit is the **structure** and the **content** of the page only. For those who are familiar, there is an overarching CSS style for Isomer sites that cannot be changed. For general users, this means that Typora gives you a visual indication of the different styles of text you can see, but it will not be exactly the same. For e.g. heading style, typeface/font, font size, etc. cannot be changed. To illustrate, if you change the Theme of your Typora (in the toolbar), what you see in Typora changes, but the Isomer page will remain the same.

I am basing this cheatsheet on a user who will not be using the **Source Code Mode** (denoted by the button that looks like '</>' at the bottom of Typora to edit. However, the coding elements may seem clearer if you are using Source Code Mode. Feel free to toggle between the two to suit your needs.

Please also explore right-clicking on the relevant text/content while editing in Typora. Generally, the necessary functions will be there to help you format whatever content you need.

## What you will need

Before you begin editing any page, it is strongly suggested to have the following prepared, so as to make editing less disruptive:

- [ ] Your page content in a Word doc or other format which is easier to copy sections from.


- [ ] Your page content already **reviewed and approved** by the relevant persons. This is because Typora is mainly for ingesting content. Content uploading to a staging website takes time and many steps, and hence is not so suitable for clearing content with bosses.

- [ ] Any images to be uploaded, to be downloaded into your PC beforehand. Best practice is to avoid spaces in the filename. PDFs and other files are also possible to include.

## Headings

Headings are sections within an Isomer page.

Headings can be denoted by using the `#` syntax, where each additional `#` adds a deeper heading level. i.e. `# Heading 1` `## Sub-heading 2` `###sub-sub-heading 3` and so on.

You can also refer to "Paragraph" in the toolbar for more options.

### Example

For example: `# Guide Index`, `## Headings` and `### Example` are illustrated within this page.

## Content Pages

The content page like the one on top of this page is actually a list of anchors/bookmarks within the page. Clicking on a heading/anchor link will jump the user to the respective heading.

For simple purposes, any heading is automatically ready for an anchor. That means you don't need to code for the destination where the user will jump to.

The syntax for an anchor is `[heading](#heading)`.

For example, the code for the 'Introduction' anchor above is `[Introduction](#introduction)`, and the code for 'Content Pages' anchor is `[Content Pages](#content-pages)`.

Note that the text in `#heading` has to follow the actual heading, in **lowercase** and with **'spaces' replaced with 'dashes'**.

> Optional: Apart from headings, you can also add anchors to other sections. This requires an additional line of code to be added.
>
> For example, [this anchor](#specialanchor) is coded like this:` [this anchor](#specialanchor)`, Clicking on that link above will jump to the next block text below.

<a name="specialanchor"></a>

> As you can see, there is a piece of code  `<a name="specialanchor"></a>` which defines the location in the page for the anchor and the anchor name "specialanchor". 

## Plain text and formatting

Plain text can simply be copied directly into Typora from a Word doc, text file, etc.

For most times, any basic formatting (e.g. **bold**, <u>underlined</u>, *italic* or a **<u>*combination*</u>**) should transfer over properly, but **you should always check to make sure**.

There are some basic formatting styles available in Typora/Isomer. You can refer to "Format" in the toolbar for more options and the keyboard shortcuts. For most of them, the usual shortcuts can be used (e.g. highlighting the relevant text and typing Ctrl+B to bold text).

The most basic syntaxes are as follows:

- **Bolded text:** `**bolded text**`

- *Italic text*: `*italic text*`

- <u>Underlined text:</u> `<u>Underlined text</u>`

- The above can be ***<u>combined:</u>*** `***<u>combined</u>***`

- Horizontal line: `------`:

    ------

## Hyperlinks

A full hyperlinks come in three parts: The visual link, the actual URL, and the code to open a new tab/window for the link.

The full syntax is like this: `[visual link](actual URL){:target="_blank"}`.

- `[visual link]` refers to the actual hyperlink text that the user will see. e.g. [Eye on Asia](https://www.eyeonasia.gov.sg/) or [https://www.eyeonasia.gov.sg](https://www.eyeonasia.gov.sg/)
- `(actual URL)` refers to the actual full URL to direct the user to.
- `{:target="_blank"}` is a bit of code so that when a user clicks on the link, it opens the link in a new browser tab or window. This third part is optional, but provides a better user experience.

> Strictly speaking, a hyperlink can simply be the full URL of the website. You just need to add the angle brackets '<' and '>' to enclose the URL. For instance, you can just type `<www.eyeonasia.gov.sg/>`, which shows up as  <www.eyeonasia.gov.sg/>.
>
> However, this may not be suitable for long links, and you still need the `{:target="_blank"}` code to launch a new tab/window.

For example, `[www.eyeonasia.gov.sg](https://www.eyeonasia.gov.sg/asean-countries/know/living-in-asean-countries/customs-costumes-etiquette-in-brunei/){:target="_blank"}` will appear like this : [www.eyeonasia.gov.sg](https://www.eyeonasia.gov.sg/asean-countries/know/living-in-asean-countries/customs-costumes-etiquette-in-brunei/){:target="_blank"}.

For another example, a typical reference citation to an NLB book may look like this: Ahlers, A. L., Hansen, M. H., & Svarverud, R. (2020). [*The great smog of China : a short event history of air pollution*](https://eservice.nlb.gov.sg/item_holding_s.aspx?bid=205255789){:target="_blank"}. Ann Arbor, MI: Association for Asian Studies, Inc. 

When editing in Typora, you will realise that the visual URL appears 'normal' when your cursor is outside of it, but when your cursor is in the URL, the full code expands. You will also realise the `{:target="_blank"}` remains visible, but this bit of code will not appear in the live page.

Within Typora, you can Ctrl + click any URL or hyperlink to open the website in our web browser.

## Images

Images can be inserted into Isomer pages. By default, all images are centralised in their respective sections.

The image source is usually an image file from the repository, usually in the `/images` folder and sub-folders for tidier file management (e.g. `/images/visualarts/NLB.jpg`). Note that the directory link begins without the root or repository folder (in this case `nlb-reference`).

- Important Note: **You will need to copy the image files you had previously downloaded or prepared into the `\image` folder in the repository.** This can be done by opening the repository in Github using the `Show in Explorer` button in the landing page.
- For Reference@NLB, there are specific folders for each category of guide (e.g. arts, sci-tech, literature), so please use the correct folder. This is to ensure good housekeeping, and reduce the chances of having multiple copies of the same image.
- For Reference@NLB, there are specific folders for each category of guide (e.g. arts, sci-tech, literature), so please use the correct folder. This is to ensure good housekeeping, and reduce the chances of having multiple copies of the same image.

However, online images can be used as well, so long as the URL is active (e.g. https://i.imgur.com/HXMwtll.jpg).

Note: If you are using directory links, Typora usually does not provide image previews. To preview the images, you will need to commit the changes to staging and view them there.

> Although Typora has the function to `mouse right-click -> Insert -> Image`, this will only upload images from your PC, and the directory link will not work on Github or Isomer. **Please do not rely on this function**.
>
> However, this function may still be useful to avoid typing out the full directory link, provided you have already copied the image file into the correct directory in the repository on your PC. 

For instance, <img src="`/images/temp/visualarts/NLB.jpg`" style="width:180px;" />  does not have a preview in Typora.

There are two ways to insert images into a page: what I call the 'banner' method and the 'sized' method.

### Banner images

Banners are images that will automatically scale to the full width of the window. They are slightly easier to code, and will scale to any screen (mobile or PC).

The syntax for a banner image comes in three parts: the '!' denoting an image, the alt text , and the image source.

The full syntax for a banner image is: `![alt text](image URL or directory)`

- `[alt text]` refers to the alternate text for the image. This sometimes appears when a user mouseovers the image and leaves the mouse cursor there. More importantly, accessibility tools will read aloud this text if a visually impaired person is using the website. Although this is freetext, you should use it to indicate what the image is. This is also because there is no preview for images in Isomer pages within Typora.

- `(image URL or directory)`refers to the source for the image. As explained earlier, this can either be a URL, e.g. (https://i.imgur.com/HXMwtll.jpg) or more usually a directory link within the repository, e.g. (`/images/temp/visualarts/NLB.jpg`). Note that .JPG, .PNG and .GIF files all suitable.

For example, `![Sample image](https://media.giphy.com/media/AwF74xIsyoiKQ/source.gif) ` will result in this image below:

![Sample image](https://media.giphy.com/media/AwF74xIsyoiKQ/source.gif) 

Important note: **This is not suitable for images in portrait layout**, because the auto-scaling will result in a HUGE image that wastes space and will annoy the user.

### Sized images

Sized images allows some control over the sizing of the image file. These images will not scale to the screen size for the user.

The syntax for a sized image comes in two parts: the source and the style. 

The full syntax is: `<img src="image source here" style="width:1234px;" />`

- `img src`refers to the source for the image, which can be a URL or a directory link.

- `style` refers to the styles to be defined for the images. For the general user, `"width=180px"` is sufficient, and you can change the value for width to your preference.

>  For advanced users, this is HTML coding. You may define other style parameters like padding, height, etc.

For example, `<img src="https://i.imgur.com/HXMwtll.jpg" style="width:180px;" />` will show this image below:

<img src="https://i.imgur.com/HXMwtll.jpg" style="width:180px;" />

Notice this image does not span the whole screen and is limited in size.

## Videos

Videos can usually be embedded by copying the embed HTML code from the respective websites. Embedded videos typically span the width of the frame and will scale with respect to screen size.

Some tried and tested websites that work are: **YouTube** and **Vimeo**.

These usually look something like this: `<iframe src="https://player.vimeo.com/video/85683143" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>`, which is the video that appears below.

<iframe src="https://player.vimeo.com/video/85683143" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/85683143">cat</a> from <a href="https://vimeo.com/chipstea">chips &amp; tea</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

## Footnotes

Footnotes can be created as well, for example if citations and references are needed.

The syntax for footnotes in the main text is `[^number or text]`, and will appear in superscript like this: [^number or text]

> If you mouse over the footnote, a pop-up text will display the footnote text. You can try it out here. [^number or text]

As you can tell in the above example, the number or text can be customised by you. Usually it should be numerical, e.g. 1, 2, 3 etc.

The syntax for the corresponding footnote/citation is `[^number or text]: citation text`. In Typora, it will appear like this when typed out:

[^number or text]: citation text

> Notice the blue arrow(s) that appears at the end of the footnote. This arrow will appear in the live webpage, and allows users to jump back to the original footnote.
>
> Notice that there are two blue arrows. That is because I have used this same footnote twice. The first blue arrow will jump to the first instance of the footnote, while the second will jump to the second.
>
> This means that you can have multiple footnotes in the main text that refer to the same reference. Note however that your original reference document to copy from should reflect the same numbering, to avoid any copying errors.

Important Notes:

- The actual superscript footnote texts in the main text and the citation **must be exactly the same** (in this case, `number or text`.) 
- It does not matter where you put the footnote with the citation text (i.e.`[^number or text]: citation text`). All footnotes will appear at the very bottom of the live webpage.
- For ease of reference, you may wish to place footnotes just after the paragraphs they appear in. However, there is no issue to list all references only at the end of the page.
- All footnotes at the bottom of the page will be automatically listed and sorted in alphabetical order. Hence, you do not need to specifically sort/order the footnotes and their names/numbers.

## Tables

My suggestion is that tables are only suitable in Typora/Markdown if they contain small phrases. This is because tables are denoted/coded using plain text, and is not visually easy to read/edit in Typora/Markdown if the content inside it contains a lot of text. This applies also to images and videos, since those are coded using text.

- **For beginners, you may choose to use Typora's table creator to assist you visually. This is found under Paragraph -> Table -> Insert Table**.

- Once the table is created, you can right-click the table to add/remove rows and columns, etc.

The syntax for tables uses the vertical line character `|` to mark out individual rows and columns. (This `|` character is above the forward-slash character on your keyboard.)

For example, this syntax here is a table for some subject headings and call numbers:

`| **Search Terms**                                             | **Call Numbers** |`
`| ------------------------------------------------------------ | ---------------- |`
`| Intergovernmental cooperation (Southeast Asia), Southeast Asia Environmental conditions | 341.2473         |`
`| Forest fires (Environmental aspects), Forest fires (Research), Smaze (Environmental aspects), Smaze (Research), Forest ecology | 363.379          |`
`| Air Pollution                                                | 363.7            |`
`| More ActionsForest fires (Southeast Asia, Prevention and control), Forests and forestry, Fire management (Southeast Asia) | 634.9618         |`

Each line defines a row, and each bunch of text bounded by `|` on the left and right defines the content in each cell/column of that row.

This visually appears as the table here:

| **Search Terms**                                             | **Call Numbers** |
| ------------------------------------------------------------ | ---------------- |
| Intergovernmental cooperation (Southeast Asia), Southeast Asia Environmental conditions | 341.2473         |
| Forest fires (Environmental aspects), Forest fires (Research), Smaze (Environmental aspects), Smaze (Research), Forest ecology | 363.379          |
| Air Pollution                                                | 363.7            |
| Forest fires (Southeast Asia, Prevention and control), Forests and forestry, Fire management (Southeast Asia) | 634.9618         |

As you can see, a table becomes increasingly complex the more content/text you put into it. Hence, the use of tables must be considered carefully before including.

## KIV Content

Occasionally, you may have content which is already prepared, but can only go live at a later date (e.g. waiting for an event date to pass, or waiting for publicity to go live). In that case, you may wish to type out the content first in Isomer to avoid having to rush last minute updates. You are able to 'hide' it within a page that is live by using the comments function or syntax.

> Comments are coding syntax that allow descriptive comments for a coder to better understand in common English what is happening. The usefulness comes in the fact that comments are visible during editing but not visible in the live webpage.

A comment's syntax looks like this: `<!-- this is a comment -->`.

It is made up of three parts: the opening (`<!--`), the comment text, and the closing (`-->`)

An example will look like this in Typora: <!-- this is a comment -->

This application may be more apparent with an example. Say I have content that can only be released in a weeks' time. I can type out this as follows in comments, but this isn't visible in the webpage:

> <!-- This image can only be publicly viewed on Black Friday. <br><img src="https://i.imgur.com/HXMwtll.jpg" style="width:180px;" /> <br>Insert 500 word essay here. -->

When the commit is made to staging and then production, this comment remains invisible. When I am ready to publish the content, I can just delete the opening and closing syntaxes, and the content is good to go live.

> This image can only be publicly viewed on Black Friday. <br><img src="https://i.imgur.com/HXMwtll.jpg" style="width:180px;" /> <br>Insert 500 word essay here.

## Useful Websites for Reference

- Govtech's Isomer cheatsheet: <https://v2.isomer.gov.sg/get-started/markdown/markdown-cheatsheet>
- Blog post explaining Markdown and some formatting functions: <https://blog.bit.ai/what-is-markdown/>
- Cheatsheet of syntaxes: <https://blog.bit.ai/wp-content/uploads/2017/12/Markdown-Infographic-1.jpg>