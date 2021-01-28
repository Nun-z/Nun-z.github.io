This method (used first by tunip3) allows apps to be installed to an Xbox in retail mode that would normally only be available in dev mode.

## Guide to Installing Apps to an Xbox in Retail Mode

### Table of Contents

Empty

### Introduction

This guide will describe the process of uploading a Universal Windows Platform (UWP) app to the Microsoft Store for use on an Xbox in retail mode.  Apps that you install to your Xbox in this way will not need to be sideloaded in dev mode.  This is useful for several reasons: allowing use of Xbox remote play, avoiding having to restart the Xbox, and bypassing the 2 GB file size limit imposed on dev mode.  Currently, only apps for which the source code is freely available can be installed in this way to retail mode.

There are some things you should be aware of if you choose to follow this guide.  Installing emulation apps to an Xbox in retail mode is against Microsoft’s terms of service.  For example, it is possible to install RetroArch and PPSSPP to an Xbox in retail mode.  The consequences of breaking these terms of service, if any, are unknown.  In addition, you will need to pay $20 in order to acquire a developer account from Microsoft.  If you can currently sideload apps in dev mode, you have already paid and you don’t need to pay again.  For the purposes of this guide, an FTP app will be uploaded for use on retail mode.

To summarize what must be done, you must first create a template for an app on Microsoft Partner Center (used for releasing UWP apps to the Microsoft Store), indicate that the app will only be available to a private audience (so that it doesn’t need to pass certification), add your email address to that private audience, associate the app’s source code with the project you created in Partner Center, generate a package that can be uploaded to Partner Center, upload the package to Partner Center, submit the Partner Center project to Microsoft, create a website with a link to your app’s Microsoft Store page, and then click on that link using your Xbox’s Edge browser.

### Step 1: Sign up for a developer account

If you have a Microsoft account that you log into on your Xbox and $20, you have everything you need to complete this step.  If you have a developer account already, skip this step.
