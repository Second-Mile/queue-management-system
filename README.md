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
### Customizing the Spreadsheet
    
