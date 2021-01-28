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

**1.**  Go to this URL (https://developer.microsoft.com/en-us/store/register/) and click on the “sign up” button.

**2.**  If you are not already signed in with your Xbox’s Microsoft account, sign in using the prompt displayed.

**3.**  On the next page, select the “individual” account type option.
![AccountType](https://i.imgur.com/QMwdTjV.png "Sign up for an individual account")

**4.**  Scroll down to the “publisher display name (company name)” textbox and enter your desired publisher name.  This can be anything as long as it hasn’t already been claimed by someone else.

**5.**  Scroll down and fill in the “contact info” textboxes.  Then, press the “next” button at the bottom of the page.

**6.**  On the next page, click on “add a new payment method.”

**7.**  Enter your payment information, go to the Review page, and complete the purchase.  You now have a Microsoft developer account.

### Step 2: Create an application in Microsoft Partner Center

Now we will use the Partner Center to create an app that you can submit to your own private Microsoft Store.

**1.**  Navigate to this URL (https://partner.microsoft.com/overview).

**2.**  Press the "create a new app" button.

**3.**  Enter an app name into the "name" field and click on the "reserve product name" button.  Like the publisher name, your app's name can be anything that has not already been reserved.

**4.**  The application overview page is now displayed.  Click on the "start your submission" button.

**5.**  All these sections will need to be completed in order to create your app.  Click on the "pricing and availability" link first.

![availability](https://i.imgur.com/SqQ4huM.png "Click on the topmost link")

**6.**  In the visibility section of the next page, click on the "private audience" radio button, and then click on the "create a new group" link.

![visibility](https://i.imgur.com/uSnYjw8.png "Add yourself to a group")

**7.**  Enter anything you desire in the "group name" textbox, and then enter your email address into the bottom textbox.

**8.**  Click on the "save" button.

**9.** First, place your cursor on the symbol with three squares on the left-hand portion of the page.  Then, click on the name of your app.

![return](https://i.imgur.com/zePt574.png "Return to the product overview page")

