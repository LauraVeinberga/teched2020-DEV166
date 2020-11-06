# Getting Started - Setting up your development environment

Welcome to the workshop 'Extend SAP S/4HANA with SAP Cloud Platform Extension Suite.\
This workshop will guide you step-by-step through the process of 
- creating new data models and a service using the Cloud Application Programming Model (CAP)
- integrates a service from the 
- creating a List Report Object Page application based on Fiori elements (FE) using the new services
- configuring and running a predefined continuous integration and delivery (CI/CD) pipeline that automatically tests, builds, and deploys your code changes to the SAP Cloud Platform

## Set up Business Application Studio in an SAP Cloud Platform Trial Account

If you don't have an SAP Cloud Platform account already, you can create your own [here](https://www.sap.com/products/cloud-platform/get-started.html).

### New Trial Users

After having registered your new user, start your trial via [this link](https://account.hanatrial.ondemand.com/register)\
At first time log in, you'll be asked to select your preferred region.
This will start the set up of your account.

![Trial Setup](../ex0/images/00_00_0010.png)

Your subaccount, org and space is created automatically, along with the necessary role configurations and subscriptions.\
When done, the subaccount overview page is shown.

### Existing Trial Users

In your subaccount, choose 'Subscriptions' in the left-hand navigation.\
Choose 'SAP Business Application Studio' in the list of available subscriptions.\
Choose 'Subscribe'.\
Navigate back to your subaccount overview page.

### Access SAP Business Application Studio

Click on the Quick Tool Access icon **SAP Business Application Studio**.

![Welcome SCP Trial](../ex0/images/00_00_0020.png)

## Create Dev Space

Click on the button **Create Dev Space**.

![Create Dev Space](../ex0/images/00_00_0030.png)

Enter a name for your dev space and select profile **SAP Fiori**.

![Select Profile](../ex0/images/00_00_0040.png)

In the lower right corner of the page press button **Create Dev Space**.

![confirm](../ex0/images/00_00_0050.png)<br>

Once your dev space has status running, click on the development space name to open it.

![enter dev space](../ex0/images/00_00_0060.png)

## Get the sample scenario

Access the Github Repository via [this link](https://github.com/SAP-samples/teched2020-IIS360)\
Click on the button **Code** (1), then click on the icon (2) to copy the git clone link.

![copy link](../ex0/images/00_00_0070.png)

(3) Open a new terminal via the header menu.

![new terminal](../ex0/images/00_00_0080.png)

In the terminal window, type the following commands and confirm with return:
- cd projects
- git clone https://github.com/SAP-samples/teched2020-IIS360.git (you can paste the copied link here)
- cd teched2020-IIS360
- npm install (this installs all node modules as defined in the projects package.json)
- cds w (this compiles the service and runs it in watch mode)

(4) Click button **Expose and Open** on the appearing dialog

![expose button](../ex0/images/00_00_0110.png)

You can now provide an alias for the exposed port.\
(5)Enter 'preview' in the input field. Confirm with 'Enter'.

![SAP Business Application Studio - Google Chrome](../ex0/images/00_00_0120.png)

A browser is opened.\
(6) Click the **$metadata** link

![metadata](../ex0/images/00_00_0130.png)

## Reopen the exposed port

If you closed the preview browser tab, you can reopen it by applying the following steps.

(7) Click **View -> Find Command...**.

![SAP Business Application Studio - Google Chrome](images/img_039.png)

(8) Enter **port** in the dialogs input field to filter the available commands.

![SAP Business Application Studio - Google Chrome](images/img_039a.png)

(9) Select ![](images/fieldicon03.png) .

![SAP Business Application Studio - Google Chrome](images/img_040.png)

(10) A list with exposed ports is shown. Selecting one opens up a new browser tab.

![SAP Business Application Studio - Google Chrome](images/img_041.png)

## Summary

With the setup procedure done, you now have completed:
- setting up the SAP Cloud Platform trial account
- Access to SAP Business Application Studio (SBAS)
- Creation of your dev space
- Setting up the sample OData V4 service in SBAS

Continue to - [Exercise 1 - Generation of the Fiori elements app](../ex1/README.md)
