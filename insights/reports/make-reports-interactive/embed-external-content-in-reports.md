---
description: Add videos and content from other sites to your reports
---

# Embed external content in reports

Use the URL embed component to display content hosted on other sites in your reports. For example, you can include YouTube videos, web pages, and Google Docs to create robust multi-media experiences for your viewers.

### To embed external content <a href="#to-embed-external-content" id="to-embed-external-content"></a>

1. Edit your report.
2. In the toolbar, click <img src="../../../.gitbook/assets/image (2390).png" alt="" data-size="line">**.**
3. A blank content frame appears on the canvas. Move and resize this as needed.
4. On the right, In the _DATA_ tab of the properties panel, enter the URL to the desired content in the **External Content URL** field.
5. Use the _STYLE_ tab to configure the content frame's border and background properties.

### How URL embed works <a href="#how-url-embed-works" id="how-url-embed-works"></a>

The URL embed component allows content hosted on other websites to appear within a box in your report. Report viewers can interact with that content as if viewing it in the content's native environment: viewers can play videos, use web applications, apply Insights filters, view or edit Google Docs and Sheets, etc., depending on the kind of content you embed. You configure the size and style of the content box in the same way as other report components.

You can embed virtually any content that is accessible via a URL. However, the provider of that content must allow it to be embedded, and the content must be visible to your report viewers. If you try to embed content from a blocked site, the embedded content box will remain blank, and you'll see an error in the External Content URL field.

### Kinds of content you can embed <a href="#kinds-of-content-you-can-embed" id="kinds-of-content-you-can-embed"></a>

#### Embed a YouTube video <a href="#embed-a-youtube-video" id="embed-a-youtube-video"></a>

To embed a YouTube video in your report, copy and paste the video's shareable link into the External Content URL field. Here's how to get the sharable link:

1. View the video on YouTube.
2. On the lower right, click **Share**.\
   ![Screenshot of YouTube Share button.](https://lh3.googleusercontent.com/HTKwqZviRHrpYvI-RVJaoB4VGP48HqlX72XpqaTR9W2deWunGfoYqD5SkquQrUb2T5o=w600)
3. On the lower right, click **COPY**.\
   ![Screenshot of the YouTube embed button.](https://lh3.googleusercontent.com/HquCKzIKSQX0VUZtFciNOT4Bk4GUB1crQqD19hPOuggW5tgQKigJwQuj4xwcmMIJj90v=w400)
4. In Insights, paste this link into the **External Content URL** field.

#### Embed a Google Drive document <a href="#embed-a-google-drive-document" id="embed-a-google-drive-document"></a>

You can add Google Docs, Sheets, and Presentations to your reports to provide additional commentary and storytelling. To do this, you must first share the document publicly. Then, just copy and paste the URL to the document into the **External Content URL**.

If you share a document with edit privileges, report viewers will be able to edit the contents.

#### Embed a Insights report <a href="#embed-a-data-studio-report" id="embed-a-data-studio-report"></a>

You can frame a Insights report into another Insights report. The report you frame must have embedding enabled. You can then use the embeddable link as the **External Content URL**.

### Limits of URL embed <a href="#limits" id="limits"></a>

* Some websites may block the ability to embed their content.
* Recursive embedding is not allowed: while you can embed a Insights report into itself, you won't see the URL embed component in the embedded report.

### Related resources <a href="#related-resources" id="related-resources"></a>
