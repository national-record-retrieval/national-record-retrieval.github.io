<center><h1>Creating a Medical Records Request</h1></center>

> <h2> Methods:</h2>
> <h4> <a href='http://developer.nationalrr.com/#/create_request?id=matters_tab'>Request from the Matters Tab<a> </h4>
> <h4> <a href='http://developer.nationalrr.com/#/create_request?id=requests_tab'>Request from the Requests Tab</a> </h4>

<h2 id='matters_tab'>Requesting from the Matters Tab</h2>

1. **Open the Litify App and then Click on the Matters tab**
2. **Open any Matter record (For Which the user needs to create a Request record)**
   <img src='/images/create_request/Request From Matters 1.png'>

3. **Click on the ‘Related List Quick Link’ named Request**
   <img src='/images/create_request/Request From Matters 2.png'>

4. **Click New Button**
   <img src='/images/create_request/Request From Matters 3.png'>

   **Now the ‘Medical Record Request’ screen will appear**

   <img src='/images/create_request/Create Request From Matters 4.png'>

5. **Fill the form and click on the '<span class='red'>Next</span>' button**

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

**EX: Example of a valid filled page where <span class='red'>NRR All Dates</span> is toggled ON**

   <img src='/images/create_request/Create Request From Matters 7.png'>

**EX: Example of a valid filled page where <span class='red'>NRR All Dates</span> is toggled OFF**

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

Manual Provider Entry Page:

   <img src='/images/create_request/Create Request From Matters 11.png'>

10. **Click on the <span class='red'>Next</span> button.**

11. **If you're ready to send the request to NRR, toggle <span class='red'>Create NRR Order</span> to ON and select the <span class='red'>SAVE</span> button**

   <img src='/images/create_request/Create Request From Matters 13.png'>

**Otherwise, you may leave it toggled OFF and select the <span class='red'>SAVE</span> button.**

   <img src='/images/create_request/Create Request From Matters 12.png'>

12. **If <span class='red'>Create NRR Order</span> was toggled ON, the next page will have you select one or more documents to send with the order to NRR.**

   <img src='/images/create_request/Create Request From Matters 14.png'>

13. **Click on the <span class='red'>Next</span> button and select <span class='red'>Click here</span> to return to the request in Litify**

   <img src='/images/create_request/Create Request From Matters 15.png'>

<h2 id='requests_tab'>Requesting from the Requests Tab</h2>

1. **Select the <span class='red'>Requests</span> Tab and click on the <span class='red'>NEW</span> button.**

   <img src='/images/create_request/Create Request From Requests 1.png'>

2. **Fill the next page including filling the <span class='red'>Matter</span> with the respective matter from Litify**

   <img src='/images/create_request/Create Request From Requests 2.png'>

3. **All remaining steps are identical to creating a request from the Matters tab. Click <span class='large'><a href='http://develop.nationalrr.com/#/create_request?id=step6'>HERE</a></span> to go to the next relevant step.**
