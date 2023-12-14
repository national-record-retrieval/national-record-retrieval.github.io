<center><h1>Creating a Medical Records Request</h1></center>

> <h2> Methods:</h2>
> <h3> <a href='http://develop.nationalrr.com/#/create_request?id=matters_tab'>Request from the Matters Tab<a> </h3>
> <h3> <a href='http://develop.nationalrr.com/#/create_request?id=requests_tab'>Request from the Requests Tab</a> </h3>

<h2 id='matters_tab'>Requesting from the Matters Tab</h2>

1.  **Open the Litify App and then Click on the Matters tab**
2.  **Open any Matter record (For Which the user needs to create a Request record)**
    <img src='/images/create_request/Request From Matters 1.png'>

3.  **Click on the ‘Related List Quick Link’ named Request**
    <img src='/images/create_request/Request From Matters 2.png'>

4.  **Click New Button**
    <img src='/images/create_request/Request From Matters 3.png'>

    **Now the ‘Medical Record Request’ screen will appear**

   <img src='/images/create_request/Create Request From Matters 4.png'>

5.  **<Fill the form and click on the '<span class='red'>Next</span>' button**

 <img src='/images/create_request/Create Request From Matters 5.png'>

6. **<div id='step6'>Fill the next page as follows</div>**

 <img src='/images/create_request/Create Request From Matters 6.png'>

<ul>
   <li><span class='red'>NRR Record Request Type</span> (Required)</li>
   <li>NRR Request Sub Type (Optional. All medical records will be requested if no subtypes are selected)</li>
   <li>NRR All Dates</li>
   <li>NRR Certified</li>
   <li>NRR Rush Order</li>
   <li><span class='red'>Record Start Date</span> (Required if NRR All Dates is toggled off)</li>
   <li><span class='red'>Record End Date</span> (Required if NRR All Dates is toggled off)</li>
   <li>NRR Patient Notes</li>
</ul>

-   **EX: Example of a valid filled page where <span class='red'>NRR All Dates</span> is toggled ON**

     <img src='/images/create_request/Create Request From Matters 7.png'>

-   **EX: Example of a valid filled page where <span class='red'>NRR All Dates</span> is toggled OFF**

     <img src='/images/create_request/Create Request From Matters 8.png'>

7. **Click on the <span class='red'>Next</span> button**

8. **If the Custom Setting named <span class='red'>is_Provider</span> is FALSE:**
    - Search Type <span class='red'>LITIFY / NRR</span> will be visible
    - <span class='red'>Facility (Party)</span> will be visible
    - The next screen will appear as follows and you may use the above features to search Litify or NRR's provider database for your target provider

<img src='/images/create_request/Create Request From Matters 9.png'>

9. **If the Custom Setting named <span class='red'>is_Provider</span> is TRUE:**

    - Search Type <span class='red'>LITIFY / NRR</span> will not be visible
    - <span class='red'>Facility (Party)</span> will not be visible
        - The next screen will appear as follows allowing **only** for <span class='red'>NRR Provider Notes</span> input, followed by an additional page requiring manual entry of provider information after clicking <span class='red'>Next</span>

<img src='/images/create_request/Create Request From Matters 10.png'>

-   **<p>Manual Provider Entry Page:</p>**

     <img src='/images/create_request/Create Request From Matters 11.png'>

10. **Click on the <span class='red'>Next</span> button.**

11. **If you're ready to send the request to NRR, toggle <span class='red'>Create NRR Order</span> to ON and select the <span class='red'>SAVE</span> button**

   <img src='/images/create_request/Create Request From Matters 13.png'>
   
- **If you click on the Create NRR Order button functionality From Request Record, then you’ll see the below Screen:**

    <img src='/images/create_request/Create Request From Matters 16.png'>

12. **The following screen displays File Info Records which are mapped in the Matter OR Matter.Intake object. By Default, screen displays 200 records, showing the most recent file first. You are given an option to select multiple files records. You can also search the Files Using File Name.**
    **To Search for facility: It searches all the files which include those which are not displayed in initial 200 records, and which are available in Matter OR Matter.Intake object.**

-   **<span class='red'>Notes: If Salesforce have Litify v29.4 or later version, it will display ‘File Deleted Column’ and user needs to select only those files which is having a ‘false’ value in this column which indicates the file is present in Docrio and can be used for generating order in NRR.</span>**

    <img src='/images/create_request/Create Request From Matters 17.png'>

-   **In the above screen after selecting the files by clicking the 'Next' button, and order will get created in the NRR System and you will be redirected to Request Record**

**<h2>Error Messages:</h2>**

-   **If you click on Create NRR Order button and if a request record is not satisfying the following condition Request. NRR Order Status = New AND Request.Document # Is Blank, you will be shown different error messages based on additional criteria mentioned below:**

1. **Error 1: If <span class='red'>NRR Order Status = Requested</span>, then below message will be shown:**

 <img src='/images/create_request/Create Request From Matters 18.png'>

2. **Error 2: <span class='red'>NRR Order Status = Received</span>, then below message will be shown:**

 <img src='/images/create_request/Create Request From Matters 19.png'>

3. **Error 3: <span class='red'>NRR Order Status = Error</span> OR <span class='red'>Request. NRR Order Status = Canceled</span>, then below message will be shown**

 <img src='/images/create_request/Create Request From Matters 20.png'>

<h2 id='requests_tab'>Requesting from the Requests Tab</h2>

1. **Select the <span class='red'>Requests</span> Tab and click on the <span class='red'>NEW</span> button.**

 <img src='/images/create_request/Create Request From Requests 1.png'>

2. **Fill the next page including filling the <span class='red'>Matter</span> with the respective matter from Litify**

 <img src='/images/create_request/Create Request From Requests 2.png'>

3. **All remaining steps are identical to creating a request from the Matters tab. Click <span class='large'><a href='http://develop.nationalrr.com/#/create_request?id=step6'>HERE</a></span> to go to the next relevant step.**
