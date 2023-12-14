 <center><h1> NRR Litify Docrio Installation Guide </h1></center>

> <h2> Prerequisites: </h2>

-   **User account used to install packages needs administrative rights**
-   **Litify PM (Version 29 or higher)**
-   **Docrio (Version 14.8 or higher)**

> <h2> Docrio SDK Installation  </h2>

**This step must be completed before NRR Install can begin.** <a href='http://develop.nationalrr.com/#/docrio_sdk'>Link to SDK</a>

> <h2> Install NRR Litify Docrio Integration </h2>

**Use this URL to install the package into any organization:** https://login.salesforce.com/packaging/installPackage.apexp?p0=04t5Y000001aFWp

_Note: If you are installing into a sandbox organization you must replace the initial portion of the URL with: http://test.salesforce.com_

  <img src='/images/docrio_installation/NRR Docrio 1.jpg'>

> <h2> Custom Settings </h2>

1.  Navigate to Custom Settings in Setup
2.  Find ‘NRR Setup’
3.  Click Manage, and then the New Button
4.  Fill in all the settings, they are required to send requests to NRR.
5.  Location: N/A
6.  Client ID: _Contact Lisa Elkins for this info_
7.  Client Key: _Contact Lisa Elkins for this info_
8.  NRR Account Email: _Contact Lisa Elkins for this info_
9.  The endpoint is: https://nationalrr.com/api/index_upgrade.php
10. Click checkbox for Associate with Matter if records should be returned to the Matter
11. Check the NRR Use User email ID box to allow individual users to make requests
12. Do not check box for ‘Is Provider’ selection unless you would like to manually enter all provider details for each request
13. Only check the box for State_Country_Territory if State and Territory picklists are enabled in Litify
14. Leave Check Incoming OR Outgoing field blank
15. Leave Default Service field blank
16. Check Role Create from Facility (Party) if you would like to create roles on the matter for NRR parties used when requesting
17. Check Use Party from Intake if you convert intakes to matters
18. Check Search Party Using Phone if you would like to search Litify party roles using the phone number saved
19. Do not check Auto Send Request To NRR on Create
20. Save and continue to the next step of installation

<img src='/images/docrio_installation/Custom Settings 1.jpg'>
<br>
<br>
<img src='/images/docrio_installation/Custom Settings 2.jpg'>

**Example setup:**

<img src='/images/docrio_installation/Custom Settings 3.jpg'>

> <h2> Add Remote Site settings for the NRR endpoint </h2>

**This is needed to confirm with Salesforce that you want to allow API calls to NRR.**

<img src='/images/docrio_installation/Remote Site Settings 1.jpg'>

> <h2> Put page layout setup for profiles </h2>

1. **Go to the Requests Object**
2. **Select Page Layouts**
3. **Click Page Layout Assignment**
4. **Click Edit Assignment**
5. **Select the profiles you want to have access to the NRR Request page and assign it to _'NRR Request layout 2022APR25'_**

Example:
<br>
<img src='/images/docrio_installation/Page Layout 1.jpg'>

Before layout setup:
<br>
<img src='/images/docrio_installation/Page Layout 2.jpg'>

After layout setup:
<br>
<img src='/images/docrio_installation/Page Layout 3.jpg'>

<h2> Adding Lighting Component Request Page – To Search NRR for Providers </h2>

1. **On Request Object Manager page, select Buttons, Links and Actions**
   <br>
   <img src='/images/docrio_installation/Lighting Component 1.jpg'>
2. **Type ‘New’ into the Quick Find box**
   <br>
3. **Click on the arrow and select ‘Edit’**
   <br>
   <img src='/images/docrio_installation/Lighting Component 2.jpg'>
4. **On the section Lighting Experience Override: select _‘Lighting Component’_ option and select _‘NRRLitifyDocrio:requestAuraComponent’_ page**
   <br>
   <img src='/images/docrio_installation/Lighting Component 3.jpg'>
5. **Click Save**
