---
title: "Content Publishing Moderation"
slug: content-publishing-moderation
publish: false
date: 2025-05-03
update: 2025-05-03
description: Content Publishing Moderation
categories:
  - start
---

Content publishing moderation
=============================

OnSign TV offers an extremely granular user permission system. This way, it is possible to allow only specific users to review and publish Content to Players.

To better illustrate this example, let’s create three roles in the flow:

1. 🧑‍🎨 Designer - Person in charge of creating layouts and uploading new content to the platform.
2. 🕵️ Editor - Manager in charge of reviewing, approving, and publishing the content created by the Designer.
3. 🧑‍💻 IT Admin - Person in charge of managing all account permissions.

To support the approval flow, we further recommend creating a folder structure which reflects this process. For this, we create the following folder structure:

**\Design** - Folder(s) where the design team will create and upload content

**\Design\Pending review**

**\Editor\Published**

The process at work
-------------------

1. The Designer uploads assets, creates campaigns and Playlists, and places them all in the **\Design folder**.
2. Once the Designer's job is finished and publish-ready, the content should be copied to the folder **\Design\Pending review**.
3. The Designer sends an email to the Editor saying the content is ready to be published to a specific Player or Player group.
4. Once the Editor gets the email, he reviews the content and either:
   1. Approves for publishing, meaning the content will be published following given publishing rules. To keep the structure organized, we also recommend moving the published content to the folder **\Editor\Published**.
   2. Updates, in case any changes need to be made, then approves the content for publishing. Same process as described above.
   3. Rejects, meaning the content will be returned to the Designer for review and updates.
