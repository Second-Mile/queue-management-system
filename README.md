# Queue Management System for Second Mile

## Introduction
This is a queue management system designed for the non-profit organization, Second Mile. It uses Google Sheets and Twilio in concert to allow Second Mile staff to sign their clients, or Neighbors, in and display the queue on to a screen.

## Installation and Initiation
### To install the display portion of the system
 1. Download the file called smmc-queue from the [main Github page](https://github.com/Second-Mile/queue-management-system)
 2. In the upper right-hand corner, click on the green <i><b> Clone or Download </b></i> button
 4. Click <i><b> Download ZIP </b></i>
 5. Once the file is downloaded and shows up in the computer, unzip the file by either double-clicking it or right-clicking       and selecting <i>"Unzip File"</i>
 5. Once unzipped, the smmc-queue folder will contain several files. Right-click the file called <i><b> index.html </b></i>
 6. Hover over the <i> "Open With" </i> option
 7. Select the browser of your choice
    - If the browser you want to use is not listed, make sure that the browser is installed. Otherwise, we recommend using           Chrome
#### Notes on the Display Portion:
- The display portion of the system refreshes every 10 seconds. To change the refresh time, read the 
[customization section](###Refreshing the Display).
- A connection to the internet is necessary in order for the display to connect to the spreadsheet.
- It is imperative that none of the files in the smmc-queue folder move. Moving files out of the smmc-queue folder can result in a broken system.


### To log into the Lobby:
  1. Go to the [Google Drive Homepage](drive.google.com)
  2. If you are already logged into another account, log out
  3. Log into the smmc-queue account using the credentials provided in the User Guide
  4. Once you've signed in successfully, [change the password](https://myaccount.google.com/signinoptions/password) 
  
  <b>CAUTION! Once you have changed your password, neither Team Morningstar nor any other affiliate of the University of          Houston have access to your new credentials. Any password recovery must be done through Google.</b>
  
### Setting up the Email Parse:
This step only needs to be done once during setup. Once the email is set up, there is no need to return to the email account unless it is to troubleshoot. This email will ONLY communicate with Apricot.
<b>PREREQUISITES</b>: In Apricot, at least one Secure Web Form must be created with Email Triggers enabled. The Email Triggers must be set to be sent to the smmc-queue email provided in the User Guide.

  1. Go to the [Gmail Homepage](mail.google.com)
  2. Again, if you are logged into any other account besides the Second Mile Queue account, you will need to log out
  3. Log in using the credentials provided in the user manual. Since the Google Drive and Gmail accounts are linked, you must   use the new password to log in.
  4. Create a label called 'Apricot' once logged into the Gmail account
     - On the left, scroll down, then click More
     - Click Create new label
     - Name your label
     - Click Create
  5. Create a filter to automatically add the 'Apricot' label to incoming emails from Apricot
     - Navigate back to the Inbox screen
     - In the Search bar located at the top of the screen, click the arrow to the far right of the search bar
     - In the <i><b>"From:"</b></i> field, enter <i>apricotsoftwarealerts@gmail.com</i>
     - Click <i><b>Create Filter</b></i>
     - Click the checkbox next to "Apply the label" and select 'Apricot'
     - Click <i><b>Create Filter</b></i> again
### Linking a Twilio account to the Google Spreadsheet Lobby
In order to link a Twilio account, you will first need to create a Twilio account. For personal or business use, click [this link](twilio.com) to set up an account. For non-profit use, visit [this link](twilio.org) to learn more about setting up a non-profit Twilio account. 
  1. In your Twilio dashboard, locate the AuthToken and the SID linked to your account
  2. 

## Customization
### Customizing the Display
#### The HTML Page
Before attempting any of the steps mentioned below, make sure that the smmc-queue folder is downloaded onto the computer system.

##### Changing the Refresh Time

By default, the HTML page is set to automatically refresh every 10 seconds. To change the length of time between each refresh,

1. Within the smmc-queue folder, locate the index.html file
2. Right-click the file, then select Open With
3. Click Notepad (Windows) or Text Edit (Mac)
4. Locate the line of code that says:
`<meta http-equiv="refresh" content="10”;url=“index.html">`
5. Replace the 10 within the double quotes with the desired amount in seconds
6. Save the file

##### Changing the Font Color and Size
1. To change the font color of the Welcome/Table text:
2. In the smmc-queue folder, locate the file called main.css
3. Right-click the file, then select Open With
4. Click Notepad (Windows) or Text Edit (Mac)
5. Locate the line of code called “/*Welcome Text*/” or “/*Table Text*/”
6. Within that block of code locate the line of code that says:
`color: #333; or color: #fff;`
7. Replace the numbers or letters after the pound sign. The numbers represent hexadecimal code. To find the hexadecimal code for a particular color, use [this tool](https://www.google.com/search?q=color+picker) by Google.
##### To change the size of the Welcome/Table text:
1. In the smmc-queue folder, locate the file called main.css
2. Right-click the file, then select Open With
3. Click Notepad (Windows) or Text Edit (Mac)
4. Locate the line of code called “/*Welcome Text*/” or “/*Table Text*/”
5. Within that block of code, locate the line of code that says:
		`font-size: 3em;`
6. Replace the number before the “em” with the desired size
7. Save the file
##### Changing the Logo Image
1. Locate or download the image file you’d like to use on the page
2. Move the file into the smmc-queue folder
3. Within the smmc-queue folder, locate the index.html file
4. Right-click the file, then select Open With
5. Click Notepad (Windows) or Text Edit (Mac)
6. Locate the line of code that says:
`<img src="smmc-logo.png" alt="Second Mile" class="center" style="width:40%;height:40%;">`
7. Replace the smmc-logo.png in between the double quotes with the name of the image file you moved in step 2
8. To resize the image, replace the percentages in width:40%;height:40% with the desired size
9. Save the file
##### Changing the Shortcut Icon
1. Locate or download the image file you’d like to use on the page
2. Move the file into the smmc-queue folder
3. Within the smmc-queue folder, locate the index.html file
4. Right-click the file, then select Open With
5. Click Notepad (Windows) or Text Edit (Mac)
6. Locate the line of code that says:
`<link href="smmc-favicon.png" rel="shortcut icon">`
7. Replace the smmc-favicon.png in between the double quotes with the name of the image file you moved in step 2
8. Save the file
##### Linking the Spreadsheet to the HTML Page
1. Open the Google Spreadsheet file called Second Mile Queue
2. In the URL of the browser, locate the document ID. The document ID of the example URL below is after the "/d/".
https://docs.google.com/spreadsheets/d/1PAD-26rPGniQg6pZ5PYCVl72FmFlvYjasuJ4b-hlRJU/edit#gid=1812966397
3. In the smmc-queue folder, locate the google-sheets-html.js file
4. Right-click the file, then select Open With
5. Click Notepad (Windows) or Text Edit (Mac)
6. Locate the line of code that says:
`var query = new google.visualization.Query('https://spreadsheets.google.com/tq?key=1PAD-26rPGniQg6pZ5PYCVl72FmFlvYjasuJ4b-hlRJU&output=html&usp=sharing');`
7. Replace the alphanumeric string after the “tq?key=” and the “&” sign (highlighted in yellow above) with the document ID you gathered in step 2
8. Save the file

### Customizing the Spreadsheet
#### Editing the Font or Cells
Google Sheets has a very robust set of customization options. To learn how to change the font or cell color of the sheet, refer to Google’s documentation at https://support.google.com/docs/answer/46973?co=GENIE.Platform%3DDesktop&hl=en. 

##### Some important things to note when making alterations to the spreadsheet:
- Some of the cells contain formulas necessary to perform several tasks ranging from importing data to calculating time. We strongly advise against altering these formulas, however you may still edit them at your own risk.
- The current system is limited to only 2 Counselors at a time
- The spreadsheet does not have an automated dashboard yet but can be expanded in the future

    
