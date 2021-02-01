This method (used first by tunip3) allows apps to be installed to an Xbox in retail mode that would normally only be available in dev mode.

## Guide to Installing Apps to an Xbox in Retail Mode

### Table of Contents

Empty

### Introduction

This guide will describe the process of uploading a Universal Windows Platform (UWP) app to the Microsoft Store for use on an Xbox in retail mode.  Apps that you install to your Xbox in this way will not need to be sideloaded in dev mode.  This is useful for several reasons: allowing use of Xbox remote play, avoiding having to restart the Xbox, and bypassing the 2 GB file size limit imposed on dev mode.  Currently, only apps for which the source code is freely available can be installed in this way to retail mode.

There are some things you should be aware of if you choose to follow this guide.  Installing emulation apps to an Xbox in retail mode is against Microsoft’s terms of service.  For example, it is possible to install RetroArch and PPSSPP to an Xbox in retail mode.  The consequences of breaking these terms of service, if any, are unknown.  In addition, you will need to pay $20 in order to acquire a developer account from Microsoft.  If you can currently sideload apps in dev mode, you have already paid and you don’t need to pay again.  For the purposes of this guide, an FTP app will be uploaded for use on retail mode.

To summarize what must be done, you must first create a template for an app on Microsoft Partner Center (used for releasing UWP apps to the Microsoft Store), indicate that the app will only be available to a private audience (so that it doesn’t need to pass certification), add your email address to that private audience, associate the app’s source code with the project you created in Partner Center, generate a package that can be uploaded to Partner Center, upload the package to Partner Center, submit the Partner Center project to Microsoft, create a website with a link to your app’s Microsoft Store page, and then click on that link using your Xbox’s Edge browser.

### Requirements

Empty

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

Now we will use the Partner Center to create an app that you can submit to your own private Microsoft Store.  This will be the bulk of the required work.

#### Step 2.1: Enter availability settings

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

**9.**  First, place your cursor on the symbol with three squares on the left-hand portion of the page.  Then, click on the name of your app.

![return](https://i.imgur.com/zePt574.png "Return to the product overview page")

**10.**  Click on the "submission 1" link under the "submissions" heading.

**11.**  Click on the "pricing and availability" link again.

**12.**  Select "private audience" again in the visibility section.

**13.**  Click on the checkbox for the customer group that you just created.

![customers](https://i.imgur.com/iyhJS7v.png "click on the checkbox")

**14.**  Scroll down to the discoverability section and click on the radio button for "make this product available but not discoverable in the Microsoft Store."

**15.**  Make sure the "direct link only" radio button is also selected.

![directlink](https://i.imgur.com/bnRnzrH.png "make sure the app is for a private audience")

**16.** Scroll down to the pricing section and choose "free" in the base price dropdown list.

**17.** Scroll all the way down and click on the "save draft" button.

#### Step 2.2: Enter properties settings

**1.**  Click on the "properties" link.

![properties](https://i.imgur.com/nkztM6A.png "fill out the properties section")

**2.**  In the topmost dropdown list, select "games" for the category.

**3.**  Click on the checkbox for any genre.

**4.**  Scroll down to the support info section and read the App Developer Agreement.  If the agreement says that a privacy policy is not required for your app, click on the "no" radio button and leave the other fields blank.

![policy](https://i.imgur.com/z3QsbXr.png "select the appropriate radio button for your app")

**5.**  Scroll down to the display mode section and click on both Xbox checkboxes.

![display](https://i.imgur.com/BDZfhSZ.png "display mode checkboxes")

**6.**  No further input is required.  Scroll all the way down and click on the "save" button.

#### Step 2.3: Enter age ratings settings

**1.** Click on the "age ratings" link

![ageratings](https://i.imgur.com/8x9HMJh.png "age ratings")

**2.**  Go ahead and select the radio buttons that best describe your app.  Nothing specific is required here except for the last question.

**3.**  Scroll down and select the "no" radio button for the final question.

![ratingsboard](https://i.imgur.com/x6LI0ra.png "select no here")

**4.**  Click on the "save" button.

#### Step 2.4: Enter store listing settings

**1.**  Click on the "add/remove languages" link in the store listings section.

![addlanguage](https://i.imgur.com/ZtrN9G2.png "add a language")

**2.**  Type "English" into the first textbox and press the enter key.

**3.**  A new window is displayed.  Type "English" into the textbox and click on the "English" checkbox.

![languages](https://i.imgur.com/tAwESG0.png "select the appropriate language")

**4.**  Click on the "update" button.

**5.**  Click on the "save" button at the bottom of the screen.

**6.**  Click on the "English" link that is now displayed in the store listings section.

![englishlink](https://i.imgur.com/ud9KS4Q.png "click on the language link")

**7.**  Enter the app's description into the required "description" textbox.

**8.**  Scroll down to the screenshots section.  Click on the "Xbox" option.  You will now need to upload at least one screenshot.
