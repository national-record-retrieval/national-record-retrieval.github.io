<center><h1> Installing and configuring Docrio SDK </h1></center>

**Purpose: The purpose of the Docrio SDK package is to enable Salesforce developers to easily integrate with Docrio. This package is required by a number of other packages for that reason.**

> <h2> Prerequisites: </h2>

- You will need a user account for the client with administrative setting on salesforce
- Ensure the Litify package is installed and configured
  - Latest Release Link: https://help.litify.com/hc/en-us/articles/360044776533-Latest-Releases
- Ensure the Docrio package is installed and configured
  - Latest Release Link: https://help.litify.com/hc/en-us/articles/360044776533-Latest-Releases

> <h2> Installation of SDK </h2>

**The Latest version of SDK is available at:** https://login.salesforce.com/packaging/installPackage.apexp?p0=04t1R000001QiLCQA0

> <h2> Configuration </h2>

After installing the package, configure the SDK as follows:

1. **Visit the Docrio SDK tab in Salesforce (if the tab is not visible, you may need to enable it for your profile)**

   <img class='image' src="/images/docrio_sdk/Docrio SDK 1.jpg"/>

2. **Click the Start button. This will configure a Connected App in your Salesforce org. Connected apps take 10-30 minutes to fully configure so you may need to wait a bit for the next step to succeed.**

  <img class='image' src="/images/docrio_sdk/Docrio SDK 2.jpg"/>

3. **After waiting 10 minutes, click the Generate Access Token button**

  <img class='image' src="/images/docrio_sdk/Docrio SDK 3.jpg"/>

4. **A window will pop up. If you receive the error below it’s because the Connected App is still being set up by Salesforce. Don’t worry, just wait another 10 minutes and try again.**

  <img class='image' src="/images/docrio_sdk/Docrio SDK 4.jpg"/>

5. **Once the Connected App is configured properly the popup should look like this. Type in your login credentials for your org to authenticate against it.**

  <img src="/images/docrio_sdk/Docrio SDK 5.png"/>

6. **Click the Allow button**

  <img src="/images/docrio_sdk/Docrio SDK 6.jpg"/>
