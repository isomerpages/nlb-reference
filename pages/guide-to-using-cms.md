---
title: Guide to using CMS
permalink: /guidetousingcms-1
---
# Preparation

1) Prepare a word doc with all your content vetted and ready to ingest. Keep the layout simple and separate text from images. **You will have to do a lot of copying and pasting.**

2) Prepare all images and files needed separately - These need to be uploaded in a separate step

3) Inform Kevin of where you want the new pages to appear. Kevin will set up the website structure so you can navigate to your new pages when checking/previewing in Staging.  
Kevin also needs to be aware of all the ongoing edits, so that changes are published to the live website only when everything is good-to-go.

# Orientation for CMS

|**Section Name**|**Description**|
|----------------------|--------------------|
|**My Workspace**|Webpages to edit.<br>Also, Main website elements (DO NOT EDIT)|
|**Resources**|Blog posts; Pages organised by date|
|**Images**|Picture, photos, images|
|**Files**|Documents for downloading; PDFs; MS Office files|
|**Settings**|**(DO NOT EDIT)** Website settings|
|**Guide**|Govtech's Isomer CMS Guide (new tab)|
|**Help**|Form to request for Isomer - But you can consult Kevin first|

# Ingesting in CMS
## Setting up
1) Under the **Images** and **Files** Section, upload your images and files 

* If necessary, nest them under the correct folders and create sub-folders to keep the directory tidy

* For ease of understanding, keep filenames short and avoid special characters.

* Filenames should be easily understood

2) Under **My Workspace**, go into the relevant folder (e.g. *Getting Started*)

3) Click *Create new page* to create a new page. If necessary, create sub-folders.

*  Folders do not directly affect the URL

*  URL will be decided by you when you create a new page

4) For the new page, decide on:

* A Page title: Keep it short and simple. Special characters (including non-English) are not allowed.

* A Page URL: By default, it will suggest the URL based on the folder structure. Edit if necessary, and replace "permalink" with your proposed URL (e.g. /getting-started/marketline) 

* Click *Save*

## Editing the page

**Important caveat: SAVE OFTEN, But not too often.**  
The Save button is at the bottom right.  
* Every time you click [Save], an update is 'pushed' to the staging site, which takes some time. Many consecutive 'saves' will queue many updates, which will delay the previewing in staging.   

**Un-doing/[CTRL+Z] does not always work, so take your time to save your time.**

### Text Editor

1) In the next page, the left panel is a text editor that allows you to edit the page. The right side provides a "live" view of what you are changing (though not all formatting is reflected correctly - you need to check in Staging to be sure)

In the left panel: 

* The top bar is for format changes. Highlight the relevant text to change its Heading level, or **Bold**, *Italise* or ~~Strikethrough~~. Note that HTML coding is allowed if you know how, so you can also <u>underline</u>, etc. The coding will be implemented in the text editor automatically.

* You can also include code blocks, have block quotes, or numbered/bulleted lists.

* Buttons to include Images, Files, Hyperlinks and Tables are also available. Follow the instructions to do so. While you can add new images and files through here, this is not advisable as they will not be filed properly, which may be confusing

### Pictures

* For images, you should specify the *Alt text*, for accessibility purposes (for the visually impaired using web readers).

* Images can also have hyperlinks - Select the code representing the image, and click on the Hyperlink button to define the target URL.

### Tables

Tables are coded using text only, within 'pipes' or '|', which denote the cells.
e.g.

```
| Column 1 | Column 2 | Column 3 |
| -------- | -------- | -------- |
| Text     | Text     | Text     |
```

This can be unwieldy, especially with large blocks of text and content, so it is not advised.

### Coding manually

Those who are more familiar with the coding can type manually in the text editor without having to go through the text editor buttons.

### Other editing which may not show up in the preview panel:

* Embed links (e.g. **YouTube and Vimeo** only) may not show up sometimes, as these are HTML codes

* Footnotes [^1] may not be rendered properly in the preview.

[^1]: The footnote text can be included anywhere in the editor, but in staging and live, all footnotes are moved to the <u>bottom</u> of the page.

* If certain things do not render properly, or CMS asks you to 'sanitise' content when you click [Save], Allow CMS to sanitise it and take note of the removed content.  
Let Kevin know so he can code it in manually.

# Preview and check in Staging
1) Changes however take some time to be reflected, depending on how much has been changed. Typically the changes should be reflected within 10 mins.

2) Click on [View Staging] on the top right. This will launch a new tab for the staging website (not the webpage you are currently editing).

3) To preview your webpage, navigate to it accordingly.  
Or if the navigation bars have not been set up yet, type in your new URL accordingly (e.g. https://nlb-reference-staging.netlify.app/getting-started/marketline/) 

4) **<u>TEST EVERY SINGLE LINK.</u>** Updating to the live website takes time, and you want to avoid any broken links in the live website.

# Create a Pull Request

1) Once everything is finalised, you can raise a pull request.

2) Click on [Pull Request] on the top-right. This will lunch a new tab.

3) In the new tab, click on the green [New pull request] button.

4) Under **Compare changes**, change [base : staging] to [base : master]. The page will reload and reflect all the changes  between staging and master.

5) Click [Create pull request].

6) Changes need to be reviewed and approved. On the right panel, under Reviewers, click on the [gear] button and type in the Github user name of the reviewer (e.g. Kevinszy) and request review.

7) An email will be sent to the reviewer to seek approval.  
Separately, you should email the reviewer to inform them and let them know what changes to check/confirm.