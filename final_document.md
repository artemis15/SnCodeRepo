Final Document:
Folder Name:

  - ./Styles/Add attachment icon-list view
    - The above two files scripts are useful to put styles on your field in list view. Below are the steps to achieve this:
1. Open a record. Right click on any field label and select configure style.
2. A list will open with all the styles applied on that field.
3. Click on New button to create your custom style.
4. Enter the code of value.js in Value field of style.
5. Enter the code of style.css in Style field of style.
6. Done. Voila.. You can now have an attachment icon present on the <chosen> field in list view if there is any attachement present in that record.
7. You can use this code on any field in any table.
Folder Name:

  - ./GlideTableDescriptor/getFirstTableName()
    - ## GlideTableDescriptor

When a table is extended, that it creates all new sys_dictionary records for all the fields on the base table instead with just one single sys_dictionary entry. These entries are referred to as “cloned descendant elements” and you need to edit the “first element” in order to modify them. 
You can also programatically interact with them using a “glideElementDescriptor() method on the related “GlideTableDescriptor” object. Here we using “getFirstTableName()” to find out where it was descended from.  
Folder Name:

  - ./Background Scripts/Approval Reminders
    - Use Case: Approval are pending due approver unavailability

Solution : Assign delgates to the approver and send reminder email notification using the Approval reminder code.It will send email to delgates and they will get notified with the approval request to approve/reject per limited period.

Steps: Register an event and create a notification to send  email to manager when the event fired/triggered.
Folder Name:

  - ./Background Scripts/Deactivate groups with no members and inactive manager
    - 
# Deactivate groups with no members and inactive manager

**Use case** : Background script that will deactivate all the groups in which there are 0 members and group manager is inactive

*info* : This method is to achieve the above use-case just with one time run of background script

**Solution** : Open `Scripts - Background` from the application navigator and run the script present in [script.js](https://github.com/ServiceNowDevProgram/code-snippets/blob/main/Business%20Rules/Prevent%20adding%20user%20to%20group%20if%20manager%20is%20inactive/Script.js](https://github.com/ServiceNowDevProgram/code-snippets/blob/Copy-of-Main/Background%20Scripts/Deactivate%20groups%20with%20no%20members%20and%20inactive%20manager/script.js))
Folder Name:

  - ./Background Scripts/QuickCurrent
    - # QuickCurrent

I use this all the time to test out workflow or business rule script logic without having to go through end-to-end testing of a catalog item workflow or fill out mandatory fields or approvals multiple times just to make sure a complex script has the desired output.

By having a quick snippet to create a "current" variable, there is no need to modify the script that may be retrieving or setting values on "current" in the workflow or business rule.

## Use

1. Create the desired record and ensure all needed values are filled in.
2. Enter the table name in the **table** variable (sc_req_item is default)
3. Copy and paste the sys_id from the test record into the **sid** variable
4. Paste script below the comment and run to see if it works as expected
Folder Name:

  - ./Background Scripts/Limit String and Add Elipses
    - This function can be used to show the string with  limited number of characters and add the ellipses to it. This is mostly used on the portal side.
Folder Name:

  - ./Background Scripts/List Stories and Tasks by User and Date Range
    - 
Folder Name:

  - ./Background Scripts/FlushOutbox
    - # Flush Outbox

Delete or Ignore all email sitting in the outbox. Useful when enabling email in sub-prd and not wanting to get spammed with unsent email
Folder Name:

  - ./Background Scripts/Get Journal Entry as HTML Without Header
    - # Get Journal Entry as HTML

This script can be used in a Business Rule or background script, or any other server-side script. It assumes the presence of the `current` object, but can be used with any positioned GlideRecord. 

## Use

Simply change `current` to whatever GlideRecord variable you're using, and change the `journalFieldName` variable so it contains the name of the journal field you want to get the value for.
Folder Name:

  - ./Background Scripts/Copy table name list header action
    - # Add "Copy Table Name" menu item to the List context
* **Description:** This background script programmatically adds a menu item to any list context menu that will copy the respective table name of that list.

    >![Copy Table Name](menu.jpg)
**Example:** In this case, clicking the "Copy Table Name" menu item will copy ```cmdb_ci_win_server``` to your clipboard
* **Usage:** 
    - **addMenuItem.js:** Run this background script to add the menu item to the list context menu.
    - **removeMenuItem.js:** Run this background script to remove a previously added menu item.
Folder Name:

  - ./Background Scripts/Copy table name list header action
    - # Add "Copy Table Name" menu item to the List context
* **Description:** This background script programmatically adds a menu item to any list context menu that will copy the respective table name of that list.

    >![Copy Table Name](menu.jpg)
**Example:** In this case, clicking the "Copy Table Name" menu item will copy ```cmdb_ci_win_server``` to your clipboard
* **Usage:** 
    - **addMenuItem.js:** Run this background script to add the menu item to the list context menu.
    - **removeMenuItem.js:** Run this background script to remove a previously added menu item.
Folder Name:

  - ./Background Scripts/Logout User
    - # Logout Users
Used to log out all users within the platform.

## Usage
Run script in **logoutUser.js** in 'Scripts - Background'

* **Parameters:** 
    - **ignoreUser:** Username of a sys_user that is ignored (ex. 'admin')
Folder Name:

  - ./Background Scripts/Fetch Active Groups list without members
    - 
Folder Name:

  - ./Background Scripts/Force new value to read only or protected field
    - **Background Script**

Background Script, to force update on read only or protected fields. It can be used when it is a need of fixing a value, of field which can not be done from list / form edit. It can be used to any type of table, record and field, need just correct configuration.

**How to use**

You need to fill all four variables which are placed on the begging of the script with values:

- ticketSysId - sys_id value of record which you would like to update
- table - table where this record exists
- field - field which should be forced with new value on record
- value - new value which should be set on record

**Example execution**

Values choosed in this example: 

![Coniguration](ScreenShot_1.PNG)

Execution log:

![Coniguration](ScreenShot_2.PNG)

Execution effect on incident record

![Coniguration](ScreenShot_3.PNG)
Folder Name:

  - ./Background Scripts/Get current logged in user count in all nodes of instance
    - 
# Get current logged in user count in all nodes of instance

**Use case** : Background script that will print the count of all currently logged in users in the instance

*info* : This method is to achieve the above use-case just with one time run of background script

**Solution** : Open `Scripts - Background` from the application navigator and run the script present in [script.js](https://github.com/ServiceNowDevProgram/code-snippets/blob/main/Background%20Scripts/Get%20current%20logged%20in%20user%20count%20in%20all%20nodes%20of%20instance/script.js)
Folder Name:

  - ./Background Scripts/Convert Date Time
    - 
Folder Name:

  - ./Background Scripts/Generate JWT Token
    - 
Folder Name:

  - ./Background Scripts/Discover Datacenters for Service Accounts
    - # Discover the data centers for all the cloud service accounts.
* Description: This script will discover the data centers for all the service accounts. 
> If you have a lot of service accounts, it is best to run the script as a *Scheduled Job*
* Motivation: Using the UI to discover the data centers is impractical if you have many service accounts. It could potentially take hours. This script will perform the task programmatically
Folder Name:

  - ./Background Scripts/Convert comma separated values in string to columns
    - 1.Take any comma separated string to be displayed in columns
2.Apply above logic
3.update to field /Print /Use this in mail scripts to include in the notification.
4. we can also add this arryUtils script include (to convert arry elements to colums)

![image](https://user-images.githubusercontent.com/42912180/195672456-f282c82e-8516-4925-9e71-c80da8329ef3.png)
Folder Name:

  - ./Background Scripts/List fields in table
    - # Get Fields in Table

Quick script to print out the fields on one or multiple tables. Especialy helpful for CMBD tables when a stakeholder inevitably asks "Can you send me a list of all the tables and fields?

## Use

Simply add the table names from you wish to display the fields in the **table** array.

## Current Configuration

A demo list of CMDB tables is included. The script will list the fields numbered, in alphabetical order, and includes actual field name and label name.
Folder Name:

  - ./Background Scripts/Get Instance DB Size
    - 
Folder Name:

  - ./Background Scripts/Find out Duplicate Records
    - This script helps to find out duplicate records in the table.

In this example I have shown how to find out records in incident table.
Folder Name:

  - ./Background Scripts/Attach Workflow to Existing Record
    - # Attach Workflow to existing records

This background script can be useful if you run into a situation where the workflow condition did not trigger on an intended record, or an older version of a workflow had a flaw but the record already began fulfillment.
Folder Name:

  - ./Background Scripts/Compare Roles Between Two Users
    - 
Folder Name:

  - ./Background Scripts/Clone User Record
    - 
Folder Name:

  - ./Background Scripts/Set the status to Retired on Ec2 Instance
    - This background script is used to set the Install_status to Retired if the status is terminated for the Ec2 Instances(Ci's)
We are quering the table against the table cmdb_ci_ec2_instance
Then we have encoded query to search if there is any record with the status as terminated and install_status is not retired
We are sorting based on name and set the limit to 10K records
We are searching if there are any records, If yes, we will set the install_Status to Retired and we are disabling the workflows to false.
Folder Name:

  - ./Background Scripts/Currency Conversion
    - 
Folder Name:

  - ./Background Scripts/Get Instance Info
    - 
Folder Name:

  - ./Background Scripts/Generate statistics about events created today
    - **Background Script** 

Background Script, to easily generate statistics about today's created events in system. You can call getStats() with different parameters to get information about current situation in sysevent table. You can generate statistic about different aggregation functions, different aggregation fields and selected group by fields. It can be helpful for example to detect which type of events have the longest average processing duration or which type of events was created the most today.

**How to use** 

You need to call getStats() function with three parameters:

- field - name of field which should be used in aggregate function
- aggFunction - name of aggregate function which should be used
- orderByField - name of field which should be used to orderBy

**Example execution**

Values choosed in this example:

 ![Coniguration](ScreenShot_0.PNG)
 
Execution log:

 ![Execution](ScreenShot_1.PNG)
Folder Name:

  - ./Background Scripts/Check for duplicates on multiple criteria
    - 
Folder Name:

  - ./Background Scripts/Add Standard Change Model
    - Add the OOTB "Standard Change" model to an existing change record. OOTB, the Standard Change model is applied through an onDisplay business rule, and is not an available choice from the Model field. If you have migrated to use Change Models and generate some change requests with scripts, you may need to add the model with a background script if there is already an existing workflow context or if the model is not set by the generation script. The setter portion can be added to an existing generation script to prevent future need for this background script.
Folder Name:

  - ./Browser Bookmarklets/Quick login to current instance
    - ## Quick login to current instance

If you frequently have to login to the currently used instance with a different user (e.g. with your admin account), this Bookmarklet will be a huge timesaver for you!

All you have to do is to click the Bookmarklet, and a popup window will appear with the current Servicenow instance's login page. After you enter your credentials (or your password manager enters it), the popup will close, and the page will reload to log you in.
Folder Name:

  - ./Browser Bookmarklets/Open copied record
    - ## Open copied record

Someone sent you the Number of a record that belong to the task table (e.g. Incident, SCTASK, RITM, Story, Problem, Change etc.), but not a link to the record itself?

You can save yourself a couple of clicks if you use this Bookmarklet while you are on the instance that the record belongs to.

**Usage**:
- copy the record number,
- make sure that in your browser you are on the same instance that the record belongs to,
- click the Bookmarklet, and the record's form will open in a new tab (with a visible navigation pane).

I use this Bookmarklet on a daily basis, hope you'll like it as well.
Folder Name:

  - ./Performance Analytics/Configure Indicators in Batch
    - 
Folder Name:

  - ./GlideSystem/Session
    - GlideSystem (referred as "gs") is used to get the current user session which we are using to set the custom key and value which are used in client side scripts.

Example client script used to retrieve it

```
function onLoad(){
 var value = g_user.getClientData("custom_key");
 console.log("Client data "+value);
}
```
Folder Name:

  - ./GlideSystem/User Display Name
    - # GlideSystem - getUserDisplayName()


This is used to return the name field of the current user.

It returns Display name of user and not sysid or username

*Example* : It returns "John David" instead of "jdavid"

`script.js` file contains the following Use case : Display info message with current user display name on a form with "Display business rule"

**Sample output**:

![image](https://user-images.githubusercontent.com/36041130/138115452-6519d2a9-6bda-4eb8-8c50-670669e8466a.png)
Folder Name:

  - ./GlideSystem/workflowFlush
    - ### workflowFlush() syntax
#### Description: 
* Deletes any open scheduled job records in the Schedule (sys_trigger) table for the specified GlideRecord. 
* For reference, the below code is a part of OOB 'incident events' Business Rule

* [workflowFlush() API doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-workflowFlush_O?navFilter=workflowFlush)
* [workflowFlush code snippet](workflowFlush.js)
Folder Name:

  - ./GlideSystem/User
    - # GlideSystem User Methods

### userID
* Description: Returns the sys_id of the user associated with this session.
* [userID Code Snippet](userID.js)
* [userID API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-userID)
Folder Name:

  - ./GlideSystem/Trigger Event
    - This shows the example of triggering the event using the gs.eventQueue() or gs.eventQueueScheduled()

eventQueue() - This method inserts an specified event in an event queue
 
 - Event name. Enclose the event name in quotes.
 - GlideRecord object, typically current but can be any GlideRecord object from the event's table.
 - Any value that resolves to a string. This is known as parm1 (Parameter 1). Can be a string, variable that resolves to a string, or method that resolves to a string.
 - Any value that resolves to a string. This is known as parm2 (Parameter 2). Can be a string, variable that resolves to a string, or method that resolves to a string.
 - (Optional) Name of the queue to manage the event.


eventQueueScheduled(String name, Object instance, String parm1, String parm2, Object expiration)

 - Event name. Enclose the event name in quotes.
 - GlideRecord object, typically current but can be any GlideRecord object from the event's table.
 - Any value that resolves to a string. This is known as parm1 (Parameter 1). Can be a string, variable that resolves to a string, or method that resolves to a string.
 - Any value that resolves to a string. This is known as parm2 (Parameter 2). Can be a string, variable that resolves to a string, or method that resolves to a string.
 - (Optional) GlideDateTime object or a date/time type element that specifies the date and time to process the event.

 Using eventQueue() we can specify our own event queue - which makes the event processing faster as we specify a dedictaed queue for the same. But if we are using the eventQueueScheduled this is not possible as we have to provide the time when the event should trigger.
Folder Name:

  - ./GlideSystem/Trigger Event
    - This shows the example of triggering the event using the gs.eventQueue() or gs.eventQueueScheduled()

eventQueue() - This method inserts an specified event in an event queue
 
 - Event name. Enclose the event name in quotes.
 - GlideRecord object, typically current but can be any GlideRecord object from the event's table.
 - Any value that resolves to a string. This is known as parm1 (Parameter 1). Can be a string, variable that resolves to a string, or method that resolves to a string.
 - Any value that resolves to a string. This is known as parm2 (Parameter 2). Can be a string, variable that resolves to a string, or method that resolves to a string.
 - (Optional) Name of the queue to manage the event.


eventQueueScheduled(String name, Object instance, String parm1, String parm2, Object expiration)

 - Event name. Enclose the event name in quotes.
 - GlideRecord object, typically current but can be any GlideRecord object from the event's table.
 - Any value that resolves to a string. This is known as parm1 (Parameter 1). Can be a string, variable that resolves to a string, or method that resolves to a string.
 - Any value that resolves to a string. This is known as parm2 (Parameter 2). Can be a string, variable that resolves to a string, or method that resolves to a string.
 - (Optional) GlideDateTime object or a date/time type element that specifies the date and time to process the event.

 Using eventQueue() we can specify our own event queue - which makes the event processing faster as we specify a dedictaed queue for the same. But if we are using the eventQueueScheduled this is not possible as we have to provide the time when the event should trigger.
Folder Name:

  - ./GlideSystem/date-time
    - # GlideSystem date-time Methods

### beginningOfLastMonth
  
  * [beginningOfLastMonth code snippet](beginningOfLastMonth.js)
  * Description: Returns the date and time for the beginning of last month in GMT.
  * [beginningOfLastMonth() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server/no-namespace/c_GlideSystemScopedAPI#SGSYS-beginningOfLastMonth?navFilter=glidesystem)

### minutesAgoEnd(Number minutes)
  * Description: Returns a date and time for the end of the minute a certain number of minutes ago.
  * [minutesAgoEnd(Number minutes) code snippet](minutesAgoEnd.js)
  * [minutesAgoEnd(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoEnd_N)

### minutesAgoStart(Number minutes)
  * Description: Returns a date and time for the start of the minute a certain number of minutes ago.
  * [minutesAgoStart(Number minutes) code snippet](minutesAgoStart.js)
  * [minutesAgoStart(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoStart_N)

### monthsAgo(Number months)
  * Description: Returns a date and time for a certain number of months ago.
  * [monthsAgo(Number Months) code snippet](monthsAgo.js)
  * [monthsAgo(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgo_N)

### monthsAgoEnd(Number months)
  * Description: Returns a date and time for the last day of the month a certain number of months ago
  * [monthsAgoEnd(Number Months) code snippet](monthsAgoEnd.js)
  * [monthsAgoEnd(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoEnd_N)

### monthsAgoStart(Number months)
  * Description: Returns a date and time for the start of the month a certain number of months ago.
  * [monthsAgoStart(Number Months) code snippet](monthsAgoStart.js)
  * [monthsAgoStart(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoStart_N)

### quartersAgo(Number quarters)
  * Description: Returns a date and time for a certain number of quarters ago.
  * [quartersAgo(Number quarters) code snippet](quartersAgo.js)
  * [quartersAgo(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgo_N)

### quartersAgoEnd(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoEnd(Number quarters) code snippet](quartersAgoEnd.js)
  * [quartersAgoEnd(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoEnd_N)

### quartersAgoStart(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoStart(Number quarters) code snippet](quartersAgoStart.js)
  * [quartersAgoStart(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoStart_N)

### yearsAgo(Number years)
  * Description: Gets a date and time for a certain number of years ago.
  * [yearsAgo(Number years) code snippet](yearsAgo.js)
  * [yearsAgo(Number years) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yearsAgo_N)

### yesterday()
  * Description: Returns yesterday's time (24 hours ago).
  * [yesterday() code snippet](yesterday.js)
  * [yesterday() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yesterday)

### setDisplayValueInternalWithAlternates
  * [setDisplayValueInternalWithAlternates code snippet](setDisplayValueInternalWithAlternates.js)
  * Description: Sets a date and time value using the internal format (yyyy-MM-dd HH:mm:ss) and the current user's time zone. This method attempts to parse incomplete date and time values.
  * [setDisplayValueInternalWithAlternates() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GDT-setDispValInternalAlt_S?navFilter=setDisplayValueInternalWithAlternates)
Folder Name:

  - ./GlideSystem/date-time
    - # GlideSystem date-time Methods

### beginningOfLastMonth
  
  * [beginningOfLastMonth code snippet](beginningOfLastMonth.js)
  * Description: Returns the date and time for the beginning of last month in GMT.
  * [beginningOfLastMonth() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server/no-namespace/c_GlideSystemScopedAPI#SGSYS-beginningOfLastMonth?navFilter=glidesystem)

### minutesAgoEnd(Number minutes)
  * Description: Returns a date and time for the end of the minute a certain number of minutes ago.
  * [minutesAgoEnd(Number minutes) code snippet](minutesAgoEnd.js)
  * [minutesAgoEnd(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoEnd_N)

### minutesAgoStart(Number minutes)
  * Description: Returns a date and time for the start of the minute a certain number of minutes ago.
  * [minutesAgoStart(Number minutes) code snippet](minutesAgoStart.js)
  * [minutesAgoStart(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoStart_N)

### monthsAgo(Number months)
  * Description: Returns a date and time for a certain number of months ago.
  * [monthsAgo(Number Months) code snippet](monthsAgo.js)
  * [monthsAgo(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgo_N)

### monthsAgoEnd(Number months)
  * Description: Returns a date and time for the last day of the month a certain number of months ago
  * [monthsAgoEnd(Number Months) code snippet](monthsAgoEnd.js)
  * [monthsAgoEnd(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoEnd_N)

### monthsAgoStart(Number months)
  * Description: Returns a date and time for the start of the month a certain number of months ago.
  * [monthsAgoStart(Number Months) code snippet](monthsAgoStart.js)
  * [monthsAgoStart(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoStart_N)

### quartersAgo(Number quarters)
  * Description: Returns a date and time for a certain number of quarters ago.
  * [quartersAgo(Number quarters) code snippet](quartersAgo.js)
  * [quartersAgo(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgo_N)

### quartersAgoEnd(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoEnd(Number quarters) code snippet](quartersAgoEnd.js)
  * [quartersAgoEnd(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoEnd_N)

### quartersAgoStart(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoStart(Number quarters) code snippet](quartersAgoStart.js)
  * [quartersAgoStart(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoStart_N)

### yearsAgo(Number years)
  * Description: Gets a date and time for a certain number of years ago.
  * [yearsAgo(Number years) code snippet](yearsAgo.js)
  * [yearsAgo(Number years) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yearsAgo_N)

### yesterday()
  * Description: Returns yesterday's time (24 hours ago).
  * [yesterday() code snippet](yesterday.js)
  * [yesterday() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yesterday)

### setDisplayValueInternalWithAlternates
  * [setDisplayValueInternalWithAlternates code snippet](setDisplayValueInternalWithAlternates.js)
  * Description: Sets a date and time value using the internal format (yyyy-MM-dd HH:mm:ss) and the current user's time zone. This method attempts to parse incomplete date and time values.
  * [setDisplayValueInternalWithAlternates() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GDT-setDispValInternalAlt_S?navFilter=setDisplayValueInternalWithAlternates)
Folder Name:

  - ./GlideSystem/date-time
    - # GlideSystem date-time Methods

### beginningOfLastMonth
  
  * [beginningOfLastMonth code snippet](beginningOfLastMonth.js)
  * Description: Returns the date and time for the beginning of last month in GMT.
  * [beginningOfLastMonth() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server/no-namespace/c_GlideSystemScopedAPI#SGSYS-beginningOfLastMonth?navFilter=glidesystem)

### minutesAgoEnd(Number minutes)
  * Description: Returns a date and time for the end of the minute a certain number of minutes ago.
  * [minutesAgoEnd(Number minutes) code snippet](minutesAgoEnd.js)
  * [minutesAgoEnd(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoEnd_N)

### minutesAgoStart(Number minutes)
  * Description: Returns a date and time for the start of the minute a certain number of minutes ago.
  * [minutesAgoStart(Number minutes) code snippet](minutesAgoStart.js)
  * [minutesAgoStart(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoStart_N)

### monthsAgo(Number months)
  * Description: Returns a date and time for a certain number of months ago.
  * [monthsAgo(Number Months) code snippet](monthsAgo.js)
  * [monthsAgo(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgo_N)

### monthsAgoEnd(Number months)
  * Description: Returns a date and time for the last day of the month a certain number of months ago
  * [monthsAgoEnd(Number Months) code snippet](monthsAgoEnd.js)
  * [monthsAgoEnd(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoEnd_N)

### monthsAgoStart(Number months)
  * Description: Returns a date and time for the start of the month a certain number of months ago.
  * [monthsAgoStart(Number Months) code snippet](monthsAgoStart.js)
  * [monthsAgoStart(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoStart_N)

### quartersAgo(Number quarters)
  * Description: Returns a date and time for a certain number of quarters ago.
  * [quartersAgo(Number quarters) code snippet](quartersAgo.js)
  * [quartersAgo(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgo_N)

### quartersAgoEnd(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoEnd(Number quarters) code snippet](quartersAgoEnd.js)
  * [quartersAgoEnd(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoEnd_N)

### quartersAgoStart(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoStart(Number quarters) code snippet](quartersAgoStart.js)
  * [quartersAgoStart(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoStart_N)

### yearsAgo(Number years)
  * Description: Gets a date and time for a certain number of years ago.
  * [yearsAgo(Number years) code snippet](yearsAgo.js)
  * [yearsAgo(Number years) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yearsAgo_N)

### yesterday()
  * Description: Returns yesterday's time (24 hours ago).
  * [yesterday() code snippet](yesterday.js)
  * [yesterday() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yesterday)

### setDisplayValueInternalWithAlternates
  * [setDisplayValueInternalWithAlternates code snippet](setDisplayValueInternalWithAlternates.js)
  * Description: Sets a date and time value using the internal format (yyyy-MM-dd HH:mm:ss) and the current user's time zone. This method attempts to parse incomplete date and time values.
  * [setDisplayValueInternalWithAlternates() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GDT-setDispValInternalAlt_S?navFilter=setDisplayValueInternalWithAlternates)
Folder Name:

  - ./GlideSystem/date-time
    - # GlideSystem date-time Methods

### beginningOfLastMonth
  
  * [beginningOfLastMonth code snippet](beginningOfLastMonth.js)
  * Description: Returns the date and time for the beginning of last month in GMT.
  * [beginningOfLastMonth() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server/no-namespace/c_GlideSystemScopedAPI#SGSYS-beginningOfLastMonth?navFilter=glidesystem)

### minutesAgoEnd(Number minutes)
  * Description: Returns a date and time for the end of the minute a certain number of minutes ago.
  * [minutesAgoEnd(Number minutes) code snippet](minutesAgoEnd.js)
  * [minutesAgoEnd(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoEnd_N)

### minutesAgoStart(Number minutes)
  * Description: Returns a date and time for the start of the minute a certain number of minutes ago.
  * [minutesAgoStart(Number minutes) code snippet](minutesAgoStart.js)
  * [minutesAgoStart(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoStart_N)

### monthsAgo(Number months)
  * Description: Returns a date and time for a certain number of months ago.
  * [monthsAgo(Number Months) code snippet](monthsAgo.js)
  * [monthsAgo(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgo_N)

### monthsAgoEnd(Number months)
  * Description: Returns a date and time for the last day of the month a certain number of months ago
  * [monthsAgoEnd(Number Months) code snippet](monthsAgoEnd.js)
  * [monthsAgoEnd(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoEnd_N)

### monthsAgoStart(Number months)
  * Description: Returns a date and time for the start of the month a certain number of months ago.
  * [monthsAgoStart(Number Months) code snippet](monthsAgoStart.js)
  * [monthsAgoStart(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoStart_N)

### quartersAgo(Number quarters)
  * Description: Returns a date and time for a certain number of quarters ago.
  * [quartersAgo(Number quarters) code snippet](quartersAgo.js)
  * [quartersAgo(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgo_N)

### quartersAgoEnd(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoEnd(Number quarters) code snippet](quartersAgoEnd.js)
  * [quartersAgoEnd(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoEnd_N)

### quartersAgoStart(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoStart(Number quarters) code snippet](quartersAgoStart.js)
  * [quartersAgoStart(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoStart_N)

### yearsAgo(Number years)
  * Description: Gets a date and time for a certain number of years ago.
  * [yearsAgo(Number years) code snippet](yearsAgo.js)
  * [yearsAgo(Number years) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yearsAgo_N)

### yesterday()
  * Description: Returns yesterday's time (24 hours ago).
  * [yesterday() code snippet](yesterday.js)
  * [yesterday() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yesterday)

### setDisplayValueInternalWithAlternates
  * [setDisplayValueInternalWithAlternates code snippet](setDisplayValueInternalWithAlternates.js)
  * Description: Sets a date and time value using the internal format (yyyy-MM-dd HH:mm:ss) and the current user's time zone. This method attempts to parse incomplete date and time values.
  * [setDisplayValueInternalWithAlternates() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GDT-setDispValInternalAlt_S?navFilter=setDisplayValueInternalWithAlternates)
Folder Name:

  - ./GlideSystem/date-time
    - # GlideSystem date-time Methods

### beginningOfLastMonth
  
  * [beginningOfLastMonth code snippet](beginningOfLastMonth.js)
  * Description: Returns the date and time for the beginning of last month in GMT.
  * [beginningOfLastMonth() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server/no-namespace/c_GlideSystemScopedAPI#SGSYS-beginningOfLastMonth?navFilter=glidesystem)

### minutesAgoEnd(Number minutes)
  * Description: Returns a date and time for the end of the minute a certain number of minutes ago.
  * [minutesAgoEnd(Number minutes) code snippet](minutesAgoEnd.js)
  * [minutesAgoEnd(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoEnd_N)

### minutesAgoStart(Number minutes)
  * Description: Returns a date and time for the start of the minute a certain number of minutes ago.
  * [minutesAgoStart(Number minutes) code snippet](minutesAgoStart.js)
  * [minutesAgoStart(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoStart_N)

### monthsAgo(Number months)
  * Description: Returns a date and time for a certain number of months ago.
  * [monthsAgo(Number Months) code snippet](monthsAgo.js)
  * [monthsAgo(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgo_N)

### monthsAgoEnd(Number months)
  * Description: Returns a date and time for the last day of the month a certain number of months ago
  * [monthsAgoEnd(Number Months) code snippet](monthsAgoEnd.js)
  * [monthsAgoEnd(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoEnd_N)

### monthsAgoStart(Number months)
  * Description: Returns a date and time for the start of the month a certain number of months ago.
  * [monthsAgoStart(Number Months) code snippet](monthsAgoStart.js)
  * [monthsAgoStart(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoStart_N)

### quartersAgo(Number quarters)
  * Description: Returns a date and time for a certain number of quarters ago.
  * [quartersAgo(Number quarters) code snippet](quartersAgo.js)
  * [quartersAgo(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgo_N)

### quartersAgoEnd(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoEnd(Number quarters) code snippet](quartersAgoEnd.js)
  * [quartersAgoEnd(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoEnd_N)

### quartersAgoStart(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoStart(Number quarters) code snippet](quartersAgoStart.js)
  * [quartersAgoStart(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoStart_N)

### yearsAgo(Number years)
  * Description: Gets a date and time for a certain number of years ago.
  * [yearsAgo(Number years) code snippet](yearsAgo.js)
  * [yearsAgo(Number years) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yearsAgo_N)

### yesterday()
  * Description: Returns yesterday's time (24 hours ago).
  * [yesterday() code snippet](yesterday.js)
  * [yesterday() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yesterday)

### setDisplayValueInternalWithAlternates
  * [setDisplayValueInternalWithAlternates code snippet](setDisplayValueInternalWithAlternates.js)
  * Description: Sets a date and time value using the internal format (yyyy-MM-dd HH:mm:ss) and the current user's time zone. This method attempts to parse incomplete date and time values.
  * [setDisplayValueInternalWithAlternates() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GDT-setDispValInternalAlt_S?navFilter=setDisplayValueInternalWithAlternates)
Folder Name:

  - ./GlideSystem/date-time
    - # GlideSystem date-time Methods

### beginningOfLastMonth
  
  * [beginningOfLastMonth code snippet](beginningOfLastMonth.js)
  * Description: Returns the date and time for the beginning of last month in GMT.
  * [beginningOfLastMonth() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server/no-namespace/c_GlideSystemScopedAPI#SGSYS-beginningOfLastMonth?navFilter=glidesystem)

### minutesAgoEnd(Number minutes)
  * Description: Returns a date and time for the end of the minute a certain number of minutes ago.
  * [minutesAgoEnd(Number minutes) code snippet](minutesAgoEnd.js)
  * [minutesAgoEnd(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoEnd_N)

### minutesAgoStart(Number minutes)
  * Description: Returns a date and time for the start of the minute a certain number of minutes ago.
  * [minutesAgoStart(Number minutes) code snippet](minutesAgoStart.js)
  * [minutesAgoStart(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoStart_N)

### monthsAgo(Number months)
  * Description: Returns a date and time for a certain number of months ago.
  * [monthsAgo(Number Months) code snippet](monthsAgo.js)
  * [monthsAgo(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgo_N)

### monthsAgoEnd(Number months)
  * Description: Returns a date and time for the last day of the month a certain number of months ago
  * [monthsAgoEnd(Number Months) code snippet](monthsAgoEnd.js)
  * [monthsAgoEnd(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoEnd_N)

### monthsAgoStart(Number months)
  * Description: Returns a date and time for the start of the month a certain number of months ago.
  * [monthsAgoStart(Number Months) code snippet](monthsAgoStart.js)
  * [monthsAgoStart(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoStart_N)

### quartersAgo(Number quarters)
  * Description: Returns a date and time for a certain number of quarters ago.
  * [quartersAgo(Number quarters) code snippet](quartersAgo.js)
  * [quartersAgo(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgo_N)

### quartersAgoEnd(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoEnd(Number quarters) code snippet](quartersAgoEnd.js)
  * [quartersAgoEnd(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoEnd_N)

### quartersAgoStart(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoStart(Number quarters) code snippet](quartersAgoStart.js)
  * [quartersAgoStart(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoStart_N)

### yearsAgo(Number years)
  * Description: Gets a date and time for a certain number of years ago.
  * [yearsAgo(Number years) code snippet](yearsAgo.js)
  * [yearsAgo(Number years) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yearsAgo_N)

### yesterday()
  * Description: Returns yesterday's time (24 hours ago).
  * [yesterday() code snippet](yesterday.js)
  * [yesterday() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yesterday)

### setDisplayValueInternalWithAlternates
  * [setDisplayValueInternalWithAlternates code snippet](setDisplayValueInternalWithAlternates.js)
  * Description: Sets a date and time value using the internal format (yyyy-MM-dd HH:mm:ss) and the current user's time zone. This method attempts to parse incomplete date and time values.
  * [setDisplayValueInternalWithAlternates() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GDT-setDispValInternalAlt_S?navFilter=setDisplayValueInternalWithAlternates)
Folder Name:

  - ./GlideSystem/date-time
    - # GlideSystem date-time Methods

### beginningOfLastMonth
  
  * [beginningOfLastMonth code snippet](beginningOfLastMonth.js)
  * Description: Returns the date and time for the beginning of last month in GMT.
  * [beginningOfLastMonth() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server/no-namespace/c_GlideSystemScopedAPI#SGSYS-beginningOfLastMonth?navFilter=glidesystem)

### minutesAgoEnd(Number minutes)
  * Description: Returns a date and time for the end of the minute a certain number of minutes ago.
  * [minutesAgoEnd(Number minutes) code snippet](minutesAgoEnd.js)
  * [minutesAgoEnd(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoEnd_N)

### minutesAgoStart(Number minutes)
  * Description: Returns a date and time for the start of the minute a certain number of minutes ago.
  * [minutesAgoStart(Number minutes) code snippet](minutesAgoStart.js)
  * [minutesAgoStart(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoStart_N)

### monthsAgo(Number months)
  * Description: Returns a date and time for a certain number of months ago.
  * [monthsAgo(Number Months) code snippet](monthsAgo.js)
  * [monthsAgo(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgo_N)

### monthsAgoEnd(Number months)
  * Description: Returns a date and time for the last day of the month a certain number of months ago
  * [monthsAgoEnd(Number Months) code snippet](monthsAgoEnd.js)
  * [monthsAgoEnd(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoEnd_N)

### monthsAgoStart(Number months)
  * Description: Returns a date and time for the start of the month a certain number of months ago.
  * [monthsAgoStart(Number Months) code snippet](monthsAgoStart.js)
  * [monthsAgoStart(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoStart_N)

### quartersAgo(Number quarters)
  * Description: Returns a date and time for a certain number of quarters ago.
  * [quartersAgo(Number quarters) code snippet](quartersAgo.js)
  * [quartersAgo(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgo_N)

### quartersAgoEnd(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoEnd(Number quarters) code snippet](quartersAgoEnd.js)
  * [quartersAgoEnd(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoEnd_N)

### quartersAgoStart(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoStart(Number quarters) code snippet](quartersAgoStart.js)
  * [quartersAgoStart(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoStart_N)

### yearsAgo(Number years)
  * Description: Gets a date and time for a certain number of years ago.
  * [yearsAgo(Number years) code snippet](yearsAgo.js)
  * [yearsAgo(Number years) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yearsAgo_N)

### yesterday()
  * Description: Returns yesterday's time (24 hours ago).
  * [yesterday() code snippet](yesterday.js)
  * [yesterday() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yesterday)

### setDisplayValueInternalWithAlternates
  * [setDisplayValueInternalWithAlternates code snippet](setDisplayValueInternalWithAlternates.js)
  * Description: Sets a date and time value using the internal format (yyyy-MM-dd HH:mm:ss) and the current user's time zone. This method attempts to parse incomplete date and time values.
  * [setDisplayValueInternalWithAlternates() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GDT-setDispValInternalAlt_S?navFilter=setDisplayValueInternalWithAlternates)
Folder Name:

  - ./GlideSystem/date-time
    - # GlideSystem date-time Methods

### beginningOfLastMonth
  
  * [beginningOfLastMonth code snippet](beginningOfLastMonth.js)
  * Description: Returns the date and time for the beginning of last month in GMT.
  * [beginningOfLastMonth() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server/no-namespace/c_GlideSystemScopedAPI#SGSYS-beginningOfLastMonth?navFilter=glidesystem)

### minutesAgoEnd(Number minutes)
  * Description: Returns a date and time for the end of the minute a certain number of minutes ago.
  * [minutesAgoEnd(Number minutes) code snippet](minutesAgoEnd.js)
  * [minutesAgoEnd(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoEnd_N)

### minutesAgoStart(Number minutes)
  * Description: Returns a date and time for the start of the minute a certain number of minutes ago.
  * [minutesAgoStart(Number minutes) code snippet](minutesAgoStart.js)
  * [minutesAgoStart(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoStart_N)

### monthsAgo(Number months)
  * Description: Returns a date and time for a certain number of months ago.
  * [monthsAgo(Number Months) code snippet](monthsAgo.js)
  * [monthsAgo(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgo_N)

### monthsAgoEnd(Number months)
  * Description: Returns a date and time for the last day of the month a certain number of months ago
  * [monthsAgoEnd(Number Months) code snippet](monthsAgoEnd.js)
  * [monthsAgoEnd(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoEnd_N)

### monthsAgoStart(Number months)
  * Description: Returns a date and time for the start of the month a certain number of months ago.
  * [monthsAgoStart(Number Months) code snippet](monthsAgoStart.js)
  * [monthsAgoStart(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoStart_N)

### quartersAgo(Number quarters)
  * Description: Returns a date and time for a certain number of quarters ago.
  * [quartersAgo(Number quarters) code snippet](quartersAgo.js)
  * [quartersAgo(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgo_N)

### quartersAgoEnd(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoEnd(Number quarters) code snippet](quartersAgoEnd.js)
  * [quartersAgoEnd(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoEnd_N)

### quartersAgoStart(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoStart(Number quarters) code snippet](quartersAgoStart.js)
  * [quartersAgoStart(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoStart_N)

### yearsAgo(Number years)
  * Description: Gets a date and time for a certain number of years ago.
  * [yearsAgo(Number years) code snippet](yearsAgo.js)
  * [yearsAgo(Number years) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yearsAgo_N)

### yesterday()
  * Description: Returns yesterday's time (24 hours ago).
  * [yesterday() code snippet](yesterday.js)
  * [yesterday() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yesterday)

### setDisplayValueInternalWithAlternates
  * [setDisplayValueInternalWithAlternates code snippet](setDisplayValueInternalWithAlternates.js)
  * Description: Sets a date and time value using the internal format (yyyy-MM-dd HH:mm:ss) and the current user's time zone. This method attempts to parse incomplete date and time values.
  * [setDisplayValueInternalWithAlternates() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GDT-setDispValInternalAlt_S?navFilter=setDisplayValueInternalWithAlternates)
Folder Name:

  - ./GlideSystem/date-time
    - # GlideSystem date-time Methods

### beginningOfLastMonth
  
  * [beginningOfLastMonth code snippet](beginningOfLastMonth.js)
  * Description: Returns the date and time for the beginning of last month in GMT.
  * [beginningOfLastMonth() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server/no-namespace/c_GlideSystemScopedAPI#SGSYS-beginningOfLastMonth?navFilter=glidesystem)

### minutesAgoEnd(Number minutes)
  * Description: Returns a date and time for the end of the minute a certain number of minutes ago.
  * [minutesAgoEnd(Number minutes) code snippet](minutesAgoEnd.js)
  * [minutesAgoEnd(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoEnd_N)

### minutesAgoStart(Number minutes)
  * Description: Returns a date and time for the start of the minute a certain number of minutes ago.
  * [minutesAgoStart(Number minutes) code snippet](minutesAgoStart.js)
  * [minutesAgoStart(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoStart_N)

### monthsAgo(Number months)
  * Description: Returns a date and time for a certain number of months ago.
  * [monthsAgo(Number Months) code snippet](monthsAgo.js)
  * [monthsAgo(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgo_N)

### monthsAgoEnd(Number months)
  * Description: Returns a date and time for the last day of the month a certain number of months ago
  * [monthsAgoEnd(Number Months) code snippet](monthsAgoEnd.js)
  * [monthsAgoEnd(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoEnd_N)

### monthsAgoStart(Number months)
  * Description: Returns a date and time for the start of the month a certain number of months ago.
  * [monthsAgoStart(Number Months) code snippet](monthsAgoStart.js)
  * [monthsAgoStart(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoStart_N)

### quartersAgo(Number quarters)
  * Description: Returns a date and time for a certain number of quarters ago.
  * [quartersAgo(Number quarters) code snippet](quartersAgo.js)
  * [quartersAgo(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgo_N)

### quartersAgoEnd(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoEnd(Number quarters) code snippet](quartersAgoEnd.js)
  * [quartersAgoEnd(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoEnd_N)

### quartersAgoStart(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoStart(Number quarters) code snippet](quartersAgoStart.js)
  * [quartersAgoStart(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoStart_N)

### yearsAgo(Number years)
  * Description: Gets a date and time for a certain number of years ago.
  * [yearsAgo(Number years) code snippet](yearsAgo.js)
  * [yearsAgo(Number years) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yearsAgo_N)

### yesterday()
  * Description: Returns yesterday's time (24 hours ago).
  * [yesterday() code snippet](yesterday.js)
  * [yesterday() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yesterday)

### setDisplayValueInternalWithAlternates
  * [setDisplayValueInternalWithAlternates code snippet](setDisplayValueInternalWithAlternates.js)
  * Description: Sets a date and time value using the internal format (yyyy-MM-dd HH:mm:ss) and the current user's time zone. This method attempts to parse incomplete date and time values.
  * [setDisplayValueInternalWithAlternates() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GDT-setDispValInternalAlt_S?navFilter=setDisplayValueInternalWithAlternates)
Folder Name:

  - ./GlideSystem/date-time
    - # GlideSystem date-time Methods

### beginningOfLastMonth
  
  * [beginningOfLastMonth code snippet](beginningOfLastMonth.js)
  * Description: Returns the date and time for the beginning of last month in GMT.
  * [beginningOfLastMonth() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server/no-namespace/c_GlideSystemScopedAPI#SGSYS-beginningOfLastMonth?navFilter=glidesystem)

### minutesAgoEnd(Number minutes)
  * Description: Returns a date and time for the end of the minute a certain number of minutes ago.
  * [minutesAgoEnd(Number minutes) code snippet](minutesAgoEnd.js)
  * [minutesAgoEnd(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoEnd_N)

### minutesAgoStart(Number minutes)
  * Description: Returns a date and time for the start of the minute a certain number of minutes ago.
  * [minutesAgoStart(Number minutes) code snippet](minutesAgoStart.js)
  * [minutesAgoStart(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoStart_N)

### monthsAgo(Number months)
  * Description: Returns a date and time for a certain number of months ago.
  * [monthsAgo(Number Months) code snippet](monthsAgo.js)
  * [monthsAgo(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgo_N)

### monthsAgoEnd(Number months)
  * Description: Returns a date and time for the last day of the month a certain number of months ago
  * [monthsAgoEnd(Number Months) code snippet](monthsAgoEnd.js)
  * [monthsAgoEnd(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoEnd_N)

### monthsAgoStart(Number months)
  * Description: Returns a date and time for the start of the month a certain number of months ago.
  * [monthsAgoStart(Number Months) code snippet](monthsAgoStart.js)
  * [monthsAgoStart(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoStart_N)

### quartersAgo(Number quarters)
  * Description: Returns a date and time for a certain number of quarters ago.
  * [quartersAgo(Number quarters) code snippet](quartersAgo.js)
  * [quartersAgo(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgo_N)

### quartersAgoEnd(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoEnd(Number quarters) code snippet](quartersAgoEnd.js)
  * [quartersAgoEnd(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoEnd_N)

### quartersAgoStart(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoStart(Number quarters) code snippet](quartersAgoStart.js)
  * [quartersAgoStart(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoStart_N)

### yearsAgo(Number years)
  * Description: Gets a date and time for a certain number of years ago.
  * [yearsAgo(Number years) code snippet](yearsAgo.js)
  * [yearsAgo(Number years) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yearsAgo_N)

### yesterday()
  * Description: Returns yesterday's time (24 hours ago).
  * [yesterday() code snippet](yesterday.js)
  * [yesterday() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yesterday)

### setDisplayValueInternalWithAlternates
  * [setDisplayValueInternalWithAlternates code snippet](setDisplayValueInternalWithAlternates.js)
  * Description: Sets a date and time value using the internal format (yyyy-MM-dd HH:mm:ss) and the current user's time zone. This method attempts to parse incomplete date and time values.
  * [setDisplayValueInternalWithAlternates() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GDT-setDispValInternalAlt_S?navFilter=setDisplayValueInternalWithAlternates)
Folder Name:

  - ./GlideSystem/date-time
    - # GlideSystem date-time Methods

### beginningOfLastMonth
  
  * [beginningOfLastMonth code snippet](beginningOfLastMonth.js)
  * Description: Returns the date and time for the beginning of last month in GMT.
  * [beginningOfLastMonth() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server/no-namespace/c_GlideSystemScopedAPI#SGSYS-beginningOfLastMonth?navFilter=glidesystem)

### minutesAgoEnd(Number minutes)
  * Description: Returns a date and time for the end of the minute a certain number of minutes ago.
  * [minutesAgoEnd(Number minutes) code snippet](minutesAgoEnd.js)
  * [minutesAgoEnd(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoEnd_N)

### minutesAgoStart(Number minutes)
  * Description: Returns a date and time for the start of the minute a certain number of minutes ago.
  * [minutesAgoStart(Number minutes) code snippet](minutesAgoStart.js)
  * [minutesAgoStart(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoStart_N)

### monthsAgo(Number months)
  * Description: Returns a date and time for a certain number of months ago.
  * [monthsAgo(Number Months) code snippet](monthsAgo.js)
  * [monthsAgo(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgo_N)

### monthsAgoEnd(Number months)
  * Description: Returns a date and time for the last day of the month a certain number of months ago
  * [monthsAgoEnd(Number Months) code snippet](monthsAgoEnd.js)
  * [monthsAgoEnd(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoEnd_N)

### monthsAgoStart(Number months)
  * Description: Returns a date and time for the start of the month a certain number of months ago.
  * [monthsAgoStart(Number Months) code snippet](monthsAgoStart.js)
  * [monthsAgoStart(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoStart_N)

### quartersAgo(Number quarters)
  * Description: Returns a date and time for a certain number of quarters ago.
  * [quartersAgo(Number quarters) code snippet](quartersAgo.js)
  * [quartersAgo(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgo_N)

### quartersAgoEnd(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoEnd(Number quarters) code snippet](quartersAgoEnd.js)
  * [quartersAgoEnd(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoEnd_N)

### quartersAgoStart(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoStart(Number quarters) code snippet](quartersAgoStart.js)
  * [quartersAgoStart(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoStart_N)

### yearsAgo(Number years)
  * Description: Gets a date and time for a certain number of years ago.
  * [yearsAgo(Number years) code snippet](yearsAgo.js)
  * [yearsAgo(Number years) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yearsAgo_N)

### yesterday()
  * Description: Returns yesterday's time (24 hours ago).
  * [yesterday() code snippet](yesterday.js)
  * [yesterday() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yesterday)

### setDisplayValueInternalWithAlternates
  * [setDisplayValueInternalWithAlternates code snippet](setDisplayValueInternalWithAlternates.js)
  * Description: Sets a date and time value using the internal format (yyyy-MM-dd HH:mm:ss) and the current user's time zone. This method attempts to parse incomplete date and time values.
  * [setDisplayValueInternalWithAlternates() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GDT-setDispValInternalAlt_S?navFilter=setDisplayValueInternalWithAlternates)
Folder Name:

  - ./GlideSystem/date-time
    - # GlideSystem date-time Methods

### beginningOfLastMonth
  
  * [beginningOfLastMonth code snippet](beginningOfLastMonth.js)
  * Description: Returns the date and time for the beginning of last month in GMT.
  * [beginningOfLastMonth() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server/no-namespace/c_GlideSystemScopedAPI#SGSYS-beginningOfLastMonth?navFilter=glidesystem)

### minutesAgoEnd(Number minutes)
  * Description: Returns a date and time for the end of the minute a certain number of minutes ago.
  * [minutesAgoEnd(Number minutes) code snippet](minutesAgoEnd.js)
  * [minutesAgoEnd(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoEnd_N)

### minutesAgoStart(Number minutes)
  * Description: Returns a date and time for the start of the minute a certain number of minutes ago.
  * [minutesAgoStart(Number minutes) code snippet](minutesAgoStart.js)
  * [minutesAgoStart(Number minutes) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-minutesAgoStart_N)

### monthsAgo(Number months)
  * Description: Returns a date and time for a certain number of months ago.
  * [monthsAgo(Number Months) code snippet](monthsAgo.js)
  * [monthsAgo(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgo_N)

### monthsAgoEnd(Number months)
  * Description: Returns a date and time for the last day of the month a certain number of months ago
  * [monthsAgoEnd(Number Months) code snippet](monthsAgoEnd.js)
  * [monthsAgoEnd(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoEnd_N)

### monthsAgoStart(Number months)
  * Description: Returns a date and time for the start of the month a certain number of months ago.
  * [monthsAgoStart(Number Months) code snippet](monthsAgoStart.js)
  * [monthsAgoStart(Number Months) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-monthsAgoStart_N)

### quartersAgo(Number quarters)
  * Description: Returns a date and time for a certain number of quarters ago.
  * [quartersAgo(Number quarters) code snippet](quartersAgo.js)
  * [quartersAgo(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgo_N)

### quartersAgoEnd(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoEnd(Number quarters) code snippet](quartersAgoEnd.js)
  * [quartersAgoEnd(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoEnd_N)

### quartersAgoStart(Number quarters)
  * Description: Returns a date and time for the last day of the quarter, for a specified number of quarters ago.
  * [quartersAgoStart(Number quarters) code snippet](quartersAgoStart.js)
  * [quartersAgoStart(Number quarters) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-quartersAgoStart_N)

### yearsAgo(Number years)
  * Description: Gets a date and time for a certain number of years ago.
  * [yearsAgo(Number years) code snippet](yearsAgo.js)
  * [yearsAgo(Number years) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yearsAgo_N)

### yesterday()
  * Description: Returns yesterday's time (24 hours ago).
  * [yesterday() code snippet](yesterday.js)
  * [yesterday() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-yesterday)

### setDisplayValueInternalWithAlternates
  * [setDisplayValueInternalWithAlternates code snippet](setDisplayValueInternalWithAlternates.js)
  * Description: Sets a date and time value using the internal format (yyyy-MM-dd HH:mm:ss) and the current user's time zone. This method attempts to parse incomplete date and time values.
  * [setDisplayValueInternalWithAlternates() API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GDT-setDispValInternalAlt_S?navFilter=setDisplayValueInternalWithAlternates)
Folder Name:

  - ./GlideSystem/hasRoleExactly
    - # Server-side version of the hasRoleExactly

Determines whether the current user has the specified role.

This feature only exists on the client-side but can be useful on the server-side also.
Folder Name:

  - ./GlideSystem/Table
    - # GlideSystem Table Methods

### tableExists(String tableName)
  * Determines if a database table exists.
  * [tableExists(String tableName) code snippet](tableExists.js)
  * [tableExists(String tableName) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-tableExists_S)

### truncateTable(String tableName)
  * Deletes all records in a table. ***UNDOCUMENTED
Folder Name:

  - ./GlideSystem/Table
    - # GlideSystem Table Methods

### tableExists(String tableName)
  * Determines if a database table exists.
  * [tableExists(String tableName) code snippet](tableExists.js)
  * [tableExists(String tableName) API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_GlideSystemAPI#r_GS-tableExists_S)

### truncateTable(String tableName)
  * Deletes all records in a table. ***UNDOCUMENTED
Folder Name:

  - ./GlideSystem/Impersonate
    - GlideSystem (referred as "gs") provides a way to find information about the current session.
Using the getSession() method of the scoped GlideSystem API.

This gives the example on how to impersonate a user using the impersonate method in the code.
Folder Name:

  - ./UI Pages/Fetch Table(Incident) fields in UI Page
    - Fetch Incident fields(or any table fields) in a UI page via UI Action trigger

Steps
1) Create a UI action and create a function.
2) Add the UI action script provided in the Script section.
3) This code helps to render a pop up window of 600x600 dimentions for the UI page and passes the current sys id to UI page.
4) Make sure to add the code in the UI Page : <g:evaluate var="jvar_sysId" expression="RP.getWindowProperties().get('sysparm_sys_id')" />
5) Create a UI Page and add the HTML Code provided.
6) Trigger the UI Action from the Incident form and it should render the ui page with the incident fields data.
7) Add additional static or dynamic data as per the requirement.
Folder Name:

  - ./UI Pages/Dynamic program status overview
    - This is a super basic set of ui page and dynamic content block that can be added to a dashboard to allow users to select program records that will then load additional information, such as overall health and executive summary, into a content block.

Addition to-dos:
 1. The formatting is quite basic - you'll definitely need to apply some styles as per the instance design or customer preferences.
 2. Link to the program status report to allow for another layer of detail to be accessible
 3. Improve how users can interact with the program list

See attached image for example of what this looks like.
Folder Name:

  - ./UI Pages/Export UI pages to word docx
    - This code allows you to export the contents of a UI page into a word document

Steps
1. Create a body and contents in the html part of the UI Page
2. Create a button and name it as 'Export to word' and call the function.
3. Now, paste the js code in the client script section of the ui page.
4. Click on try it and the contents of the html body will be exported as a word upon clicking on the 'export to word' button.
Folder Name:

  - ./UI Pages/Custom Alert using UI Page
    - This script helps you to create custom popup easily and attached the screenshot for the reference, have a look.
Folder Name:

  - ./UI Pages/Custom Alert using UI Page
    - This script helps you to create custom popup easily and attached the screenshot for the reference, have a look.
Folder Name:

  - ./UI Pages/EDM DocUnifiedSearch
    - EDM ( Employee document management) which is part of HRSD product doesn’t allow query of employee documents based on different parameters e.g employee id, document type, employee and HR Case.
Current OOB implementation just allows users to query employee documents with list view filters.This results is slow performance and users get security constraints  error based on OOB ACLs which is not intuitive for most users.

Most of the organizations will have thousands of employee documents imported from different sources e.g Workday, Sharepoint and any type of sources.
During EDM implementation, most of the time we will have to import employee documents from these sources and OOB employee document table will contain thousands of documents.
Also, after cut off from these sources is done, ServiceNow EDM table becomes every growing table since all future employee documents will be stored in this table.

I created UI page which allows users to search employee documents based on employee, employee ID, document type and HR case.
This results is performance improvement as well as better UX for end users to search employee documents.

Note : Please make sure that you have com.sn_employee_document_management plugin active on your instance before using code for this UI page.
Folder Name:

  - ./UI Pages/EDM DocUnifiedSearch
    - EDM ( Employee document management) which is part of HRSD product doesn’t allow query of employee documents based on different parameters e.g employee id, document type, employee and HR Case.
Current OOB implementation just allows users to query employee documents with list view filters.This results is slow performance and users get security constraints  error based on OOB ACLs which is not intuitive for most users.

Most of the organizations will have thousands of employee documents imported from different sources e.g Workday, Sharepoint and any type of sources.
During EDM implementation, most of the time we will have to import employee documents from these sources and OOB employee document table will contain thousands of documents.
Also, after cut off from these sources is done, ServiceNow EDM table becomes every growing table since all future employee documents will be stored in this table.

I created UI page which allows users to search employee documents based on employee, employee ID, document type and HR case.
This results is performance improvement as well as better UX for end users to search employee documents.

Note : Please make sure that you have com.sn_employee_document_management plugin active on your instance before using code for this UI page.
Folder Name:

  - ./UI Actions/Open Record in Alternate Instance/Scripted REST API/sys_ws_operation
    - 
Folder Name:

  - ./UI Actions/Open Record in Alternate Instance/Script Includes
    - 
!! The switch statement in CrossInstanceHelper.js will need to be reconfigured to match instance names, and RESTMessage naming.
Folder Name:

  - ./UI Actions/Open Record in Alternate Instance/UI Action
    - 
Folder Name:

  - ./UI Actions/View in Portal Page
    - 
Folder Name:

  - ./UI Actions/Display a 2-choice confirmation dialog
    - # Display a 2-choice confirmation dialog
When you press the button on the Form screen, a two-choice dialog is displayed.

Click the Complete button to execute Serverside processing.

## Please set the following values.
* UI Action 
  * Name: Example Dialog
  * Table: incident (anything) 
  * Action name: example_dialog
  * Client: ture
  * Form button: ture
  * Onclick: onClickExampleDialog()
  * Script

```javascript
function onClickExampleDialog() {
    var dialogClass = typeof GlideModal != 'undefined' ? GlideModal : GlideDialogWindow;
    var dialog = new dialogClass('glide_modal_confirm');
    dialog.setTitle('Dialog title');
    dialog.setPreference("focusTrap", true); // Restrict focus from moving out of Dialog
    dialog.setPreference('body', 'Approve this change?');
    dialog.setPreference('buttonLabelCancel', 'Cancel'); // Cancel button label
    dialog.setPreference('buttonLabelComplete', 'Complete'); // Complete button label
    dialog.setPreference('buttonClassComplete', 'btn btn-destructive'); // Complete button CSS
    dialog.setPreference('onPromptComplete', dialogComplete.bind(this)); // Complete button function
    dialog.setPreference('onPromptCancel', dialogCancel.bind(this)); // Cancel button function
    dialog.render();
    return true;
}

// Complete button function
function dialogComplete() {
    //Press Submit Button and call UIAction(Server side 'example_dialog') again.
    gsftSubmit(null, g_form.getFormElement(), 'example_dialog');
}
// Cancel button function
function dialogCancel() {
    //alert('Dialog Cancel');
}

//Judge Server side
if (typeof window == 'undefined') {
    serversideTask();
}
// Server side function
function serversideTask() {
    current.update();
    gs.info('Serverside Task');
    action.setRedirectURL(current);
}
```
Folder Name:

  - ./UI Actions/Add Show Workflow Related link
    - There are many cases where,we would have workflows on custom tables or non task tables , where we would like to see the "Show Workflow" Related Link for ease of accessibility to the workflow.
The shared code will help show this related link on any rable record that has a workflow associated with it.

Below has to be set for this to work on UI action form:

•	Table: Select the table that you would like this UI action to be available on (preferably table with workflows)

•	Onclick : showWorkflow()

•	Active : True

•	Show Update : True

•	Client : True

•	Form Link : True

•	Condition : new global.Workflow().hasWorkflow(current)
Folder Name:

  - ./UI Actions/Create Update Set on DEV
    - 
Folder Name:

  - ./UI Actions/Create story
    - 
Folder Name:

  - ./UI Actions/Call Subflow
    - # Call Subflow from UI Action

This UI Action enables calling a subflow from ServiceNow Flow Designer using the FlowAPI.

### Instruction

The call can either be done synchronously or asynchronously, depending on the requirement. 
```javascript
//Synchronous Call: 
sn_fd.FlowAPI.getRunner().subflow('global.subflow_name').inForeground().withInputs(inputs).run();
//Asynchronous Call: 
sn_fd.FlowAPI.getRunner().subflow('global.subflow_name').inBackground().withInputs(inputs).run();
```

The API call requires the subflow internal name and scope. The internal name is shown as a second column in the subflow overview in ServiceNow Flow Designer, while the scope is shown in the third column. In the above example the subflow internal name is **subflow_name** and it was created in the **global** scope.

### Benefits
- Enable Citizen Developers to create complex UI Actions with low code Flow Designer capabilities instead of scripting
- Run complex server side UI Actions asynchronously via Flow Designer for better user experience (avoids long loading times in the current user session)
- Re-use already created subflows and actions as well as provided spokes in UI actions
Folder Name:

  - ./UI Actions/Create incident task and relate to incident
    - This UI Action loads a modal for to create a new incident task that is linked to the incident that you generated it from.

Suggested values:
Name: Create Incident Task
Table: Incident
Client: true
List v2: true
Form Link: true

Onclick: createIncidentTask()
Condition: current.state != 7
Folder Name:

  - ./UI Actions/Try Catalog item in Portal view
    - 
Folder Name:

  - ./UI Actions/Mark Records Inactive - List Action
    - Above two scripts will help you to select records in list view and mark them inactive. You can create your UI action(list action) on any table and then you should be able to
mark the records as inactive by calling the reusable script include. Process is pretty simple as shown below:
1. Create a List action - list banner button or list choice.
2. Check the client checkbox. Use the script and do any necessary modifications.
3. Keep your script include ready with the function to make records inactive and done.

You can even modify the scrip include to change other fields too based on your requirements. And you do not need to pass any table name also. This is complete generic.
Folder Name:

  - ./UI Actions/Mark Records Inactive - List Action
    - Above two scripts will help you to select records in list view and mark them inactive. You can create your UI action(list action) on any table and then you should be able to
mark the records as inactive by calling the reusable script include. Process is pretty simple as shown below:
1. Create a List action - list banner button or list choice.
2. Check the client checkbox. Use the script and do any necessary modifications.
3. Keep your script include ready with the function to make records inactive and done.

You can even modify the scrip include to change other fields too based on your requirements. And you do not need to pass any table name also. This is complete generic.
Folder Name:

  - ./UI Actions/Go to Agent Workspace Home Page
    - 
Folder Name:

  - ./UI Actions/Copy incident details and create a child incident
    - # Copy incident details and create a child incident

Use case : A button on the header of incident form to copy details(fields) of current incident and create a child incident with those copied details.

Solution : Added a code snippet for UI action script that copies few fields of current incident and creates a child for the current incident with those details.
Folder Name:

  - ./UI Actions/Copy Variable Set
    - This UI action will help create a copy of the Variable set, including the Catalog Client Script, Catalog UI actions and Variable.

Below Configurations need to be performed on the UI action form on creation

Table : Variable Set
Active: True
Show Update : True
Client : True
Action name : copyQuestionSet
On Click : clientConfirm()
Folder Name:

  - ./UI Actions/GlideModalForm - Open New Record and Pass Query
    - This is an example of using the GlideModalForm API to open a brand new record on a specific table, passing along query parameters to it to assist with loading filling out the form

Within the UI Action settings it's recommended to ensure:
- Active is true
- Either show insert and/or show update is true
- Client is true
- Your appropriate List v2 or V3 compatible checkbox is true
- Onclick contains your function name that matches the function within your Script field -- the code related to this snipped would be: **functionName()**
- Set true to however you wish to display this UI Action to the user; whether that's via Form button, Form context menu, Form link, etc.
Folder Name:

  - ./UI Actions/Clone incident on Agent Workspace
    - Agent can use this UI Action on incident form to clone/copy any existing incident.

This UI Action will create a copy of incident once agent confirm the action.

Caller field will not be copeied to newly created incident, only basic information of ticket like Company, Short Description, Category, Sub-Category 

Create an UI Action with below field values:

Name - Clone Incident

Action Name - clone_incident

Table - Incident

Client - checked (true)

Onclick - cloneIncident();

Workspace Form Button - checked (true)

Script - use clone_incident.js

Workspace Client script - use workspace_client_script.js
Folder Name:

  - ./UI Actions/Clone incident on Agent Workspace
    - Agent can use this UI Action on incident form to clone/copy any existing incident.

This UI Action will create a copy of incident once agent confirm the action.

Caller field will not be copeied to newly created incident, only basic information of ticket like Company, Short Description, Category, Sub-Category 

Create an UI Action with below field values:

Name - Clone Incident

Action Name - clone_incident

Table - Incident

Client - checked (true)

Onclick - cloneIncident();

Workspace Form Button - checked (true)

Script - use clone_incident.js

Workspace Client script - use workspace_client_script.js
Folder Name:

  - ./UI Actions/Create Incident from Record - Open in both Platform and Workspace
    - Script that can be used in the Script section of a UI Action to create an Incident, or any record type, from another record and will open the record that was just created. 
This script will work both in Platform UI and Workspace UI, as long as one of the Workspace Form/Menu buttons are checked. This reduced the need to create a script
for both Platform and Workspace within one UI Action.  For more information: https://www.ashleysn.com/post/action-opengliderecord
Folder Name:

  - ./UI Actions/Show Today Emails Logs
    - # Show Today Emails Logs

The UI Action simplifies the debugging of ServiceNow notifications by redirecting you from the notification definition to the email log list view with the predefined filter.

Setting:
- Name: Show Today Emails Logs
- Table: sysevent_email_action
- Show insert: false
- Show update: true
- Client: true
- Form link: true
- Onclick: openEmailLogList()
- Condition: new GlideRecord('sys_email_log').canRead()
Folder Name:

  - ./UI Actions/Force to Update Set
    - # Introduction

Manually Add a Record to an Update Set

1. Check to make sure the current table isn’t already recording updates
2. Push the current record into the currently-selected update set
3. Reload the form and add an info. message indicating the addition

# Settings
Name: Force to Update Set
Table: Wherever you need it!
Action name: force_update
Form link: True
Condition: gs.hasRole(‘admin’)
Script: 
//Commit any changes to the record
current.update();

//Check to make sure the table isn't synchronized already
var tbl = current.getTableName();
if(tbl.startsWith('wf_') || tbl.startsWith('sys_ui_') || tbl == 'sys_choice' || current.getED().getBooleanAttribute('update_synch') || current.getED().getBooleanAttribute('update_synch_custom')){
   gs.addErrorMessage('Updates are already being recorded for this table.');
   action.setRedirectURL(current); 
}
else{
   //Push the update into the current update set
   var um = new GlideUpdateManager2();
   um.saveRecord(current);

   //Query for the current update set to display info message
   var setID = gs.getPreference('sys_update_set');
   var us = new GlideRecord('sys_update_set');
   us.get(setID);

   //Display info message and reload the form
   gs.addInfoMessage('Record included in <a href="sys_update_set.do?sys_id=' + setID + '">' + us.name + '</a> update set.');
   action.setRedirectURL(current);
}
Folder Name:

  - ./ECMASCript 2021
    - ## What?

Prior to the Tokyo Release, ServiceNow's serverside JavaScript utilized ECMAScript 5. "ECMAScript" is basically the version of JavaScript. Newer versions have come out since then (7+ years ago!) and thus, we have been missing out on some helpful functionality.

Client-side scripting is run in your web browser so usually any client script you've made on ServiceNow could utilize the newest JavaScript features, but any script running on the server was limiteded to ES5.

ServiceNow has denoted our version of JavaScript as ECMAScript 2021, which encompasses the feature roll-up of ECMAScript 6 to ECMAScript 12. To see the full documentation of changes, you can see the release notes here: [JavaScript engine feature support](https://docs.servicenow.com/bundle/tokyo-application-development/page/script/JavaScript-engine-upgrade/reference/javascript-engine-feature-support.html). This page has all the new features that are supported, not supported, and disallowed.

## How?

To utilize ECMASCript 2021 on your app, just follow these simple steps:

1. Make sure your instance is upgraded to Tokyo (get a Personal Developer instance [here](https://developer.servicenow.com/))
2. Create a new app via your preferred method (eg. Studio or App Engine Studio)
3. Open the sys_app page for your app<br>![openrecord.png](openrecord.png)
4. Under "Design and Runtime" change "JavaSCript Mode" to `ECMAScript 2021 (ES12)`<br>![javascriptmode.png](javascriptmode.png)
5. Save your record. That's it!

## Looking forward

- The new features are available on scoped apps only for now but we've been told that Global scope support is on the roadmap.
- If you switch existing apps to the new engine, we do recommend that you test for functionality and ensure that existing scripts are running correctly.

## Features!

And here are all the scripts that came from the show. **The scripts are all formatted as if they are running in a `Before Update Business Rule` to demonstrate that it works server side**:

### const

This was actually available previously but would display an error to you when using it, despite allowing you to save. Almost everything else related to ECMAScript 6 and up would not allow you to save your record at all.

`const` is a way to declare and initialize a variable that will never change its value. A great way to ensure a variable that is not meant to change never does (your script will throw an error).

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	const y = 100;
	current.work_notes = x + y;

})(current, previous);
```

### let

What's the difference between `var` and `let`?

#### Scoping rules

The main difference is scoping rules. Variables declared by var keyword are scoped to the immediate function body (hence the function scope) while let variables are scoped to the immediate enclosing block denoted by { } (hence the block scope).

#### Hoisting

While variables declared with var keyword are hoisted (initialized with undefined before the code is run) which means they are accessible in their enclosing scope even before they are declared

#### Creating global object property

At the top level, let, unlike var, does not create a property on the global object

#### Redeclaration

In strict mode, var will let you re-declare the same variable in the same scope while let raises a SyntaxError.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	let y = 200;
	current.work_notes = x + y;

})(current, previous);
```

### arrow functions

How many times have we googled "how to do ____ in JavaScript?" and the top result was a StackOverflow answer that utilized arrow functions? Arrow functions are a compact alternative to traditional function expressions. Combined with other new features, there are so many use-cases for arrow functions (like quickly reordering arrays of objects!).

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	function addDescriptions(x, y){
		return x + '\n' + y;
	}
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	let addDescriptions = (x, y) => x + '\n'+ y; //one line!
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);
```

### for/of

A different kind of for/in to add to your arsenal.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	var work_notes = [];
	for (var inc in incidents){
		work_notes.push(incidents[inc]);
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	let work_notes = [];
	for (let inc of incidents){
		work_notes.push(inc); //note that no index reference is needed
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### map

The Map object holds key-value pairs and remembers the original insertion order of the keys. Any value (both objects and primitive values) may be used as either a key or a value.

Object is similar to Map—both let you set keys to values, retrieve those values, delete keys, and detect whether something is stored at a key. For this reason (and because there were no built-in alternatives), Object has been used as Map historically.

However, there are important differences that make Map preferable in some cases:

- Accidental Keys (objects initialize with prototype)
- Key types (previously just strings or symbols, now can be functions, objects, any primitive)
- Key Order (simplified to order of entry insertion)
- Size (inherent size property)
- Iteration (objects aren't inherently iterable)
- Performance (additions and removals are more performative)
- Serialization and parsing (object wins in this case)

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	const incidents = new Map();

	const keyString = 'a string';
	const keyObj = {};
	const keyFunc = function() {};
	
	inc_gr.next();
	incidents.set(keyString, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyObj, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyFunc, inc_gr.getValue('short_description'));

	let work_notes = [];
	work_notes.push('map size: ' + incidents.size);
	work_notes.push(incidents.get(keyString));
	work_notes.push(incidents.get(keyObj));
	work_notes.push(incidents.get(keyFunc)); //Finding an a value by providing a function!
	work_notes.push(incidents.get('a string'));

	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### set

The Set object lets you store unique values of any type, whether primitive values or object references. Faster, and forces uniqueness of values.

```javascript
const mySet1 = new Set()

mySet1.add(1)           // Set [ 1 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add('some text') // Set [ 1, 5, 'some text' ]
const o = {a: 1, b: 2}
mySet1.add(o)

mySet1.add({a: 1, b: 2})   // o is referencing a different object, so this is okay

mySet1.has(1)              // true
mySet1.has(3)              // false, since 3 has not been added to the set
mySet1.has(5)              // true
mySet1.has(Math.sqrt(25))  // true
mySet1.has('Some Text'.toLowerCase()) // true
mySet1.has(o)       // true

mySet1.size         // 5

mySet1.delete(5)    // removes 5 from the set
mySet1.has(5)       // false, 5 has been removed

mySet1.size         // 4, since we just removed one value

mySet1.add(5)       // Set [1, 'some text', {...}, {...}, 5] - a previously deleted item will be added as a new item, it will not retain its original position before deletion

console.log(mySet1)
// logs Set(5) [ 1, "some text", {…}, {…}, 5 ] in Firefox
// logs Set(5) { 1, "some text", {…}, {…}, 5 } in Chrome
```

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	let incidents = new Set();
	
	while (inc_gr.next()){
		incidents.add(inc_gr.getValue('short_description'));
	}
	
	current.work_notes = incidents.has(inc_gr.getValue('short_description')) + '\n' + incidents.values().next().value + '\n' + incidents.size;
	
})(current, previous);
```

### symbol

Symbol is a built-in object whose constructor returns a symbol primitive — also called a Symbol value or just a Symbol — that's guaranteed to be unique. Symbols are often used to add unique property keys to an object that won't collide with keys any other code might add to the object, and which are hidden from any mechanisms other code will typically use to access the object. That enables a form of weak encapsulation, or a weak form of information hiding.

Every Symbol() call is guaranteed to return a unique Symbol. Every Symbol.for("key") call will always return the same Symbol for a given value of "key". When Symbol.for("key") is called, if a Symbol with the given key can be found in the global Symbol registry, that Symbol is returned. Otherwise, a new Symbol is created, added to the global Symbol registry under the given key, and returned.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var incidents = [];
	let incident = {
		number: current.number,
		short_description: current.short_description
	};
	
	incidents.push(incident);
	incidents.push(incident);
	
	var incidents2 = [];
	incidents2.push(Symbol(incident));
	incidents2.push(Symbol(incident));
	
	current.work_notes = (incidents[0] == incidents[1]) + '\n' + (incidents2[0] == incidents2[1]); //Notice how the first one is true and the second is false, despite all four items being the "same"
	
})(current, previous);
```

### default params

Instead of having to check for included parameters in a function's body, we can do it directly in the parameters now.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	function add (x, y){
		if (y == null) y = 'nothing to see here';
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	function add (x, y = 'nothing to see here'){
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);
```

### spread

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	let incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}

	function sum(x, y, z) {
		return x + '\n' + y + '\n' + z;
	}
	
	const incidents_obj = { ...incidents}; //the array's items are "spread" out as parameters
	
	current.work_notes = sum(...incidents) + '\n' + JSON.stringify(incidents_obj);

})(current, previous);
```

### template strings/literals

I love this one because it makes it so much easier to copy and paste multi-line strings into my code. I use this a lot on AdventOfCode challenges!

```javascript
(function executeRule(current, previous /*null when async*/) {

	let x = `hello
	world
	lchh loves you`;
	
	current.work_notes = x; //goodbye \n

})(current, previous);
```

Another way that these are helpful are for templates (Thanks Chris Helming for the suggestion):

```javascript
(function executeRule(current, previous /*null when async*/) {

	const a = 5; 
	const b = 10; 
	current.work_notes = `Fifteen is ${a + b} and not ${2 * a + b}.`;

})(current, previous);
```

### destructuring

Okay, so destructuring is a LOT more than this but here is just an example.

```javascript
const x = [1, 2, 3, 4, 5];
const [y, z] = x;
// y: 1
// z: 2

const obj = { a: 1, b: 2 };
const { a, b } = obj;
// is equivalent to:
// const a = obj.a;
// const b = obj.b;
```

### class

Hoisting differences (functions and classes are both hoisted and declared but classes are not initialized)

```javascript
class Rectangle {
  constructor(height, width) {
    this.name = 'Rectangle';
    this.height = height;
    this.width = width;
  }
}

class FilledRectangle extends Rectangle {
  constructor(height, width, color) {
    super(height, width);
    this.name = 'Filled rectangle';
    this.color = color;
  }
}
```

### And more

That's not all! Go check it out in the docs!

### ES Sources

- https://betterprogramming.pub/difference-between-regular-functions-and-arrow-functions-f65639aba256
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/
Folder Name:

  - ./ECMASCript 2021
    - ## What?

Prior to the Tokyo Release, ServiceNow's serverside JavaScript utilized ECMAScript 5. "ECMAScript" is basically the version of JavaScript. Newer versions have come out since then (7+ years ago!) and thus, we have been missing out on some helpful functionality.

Client-side scripting is run in your web browser so usually any client script you've made on ServiceNow could utilize the newest JavaScript features, but any script running on the server was limiteded to ES5.

ServiceNow has denoted our version of JavaScript as ECMAScript 2021, which encompasses the feature roll-up of ECMAScript 6 to ECMAScript 12. To see the full documentation of changes, you can see the release notes here: [JavaScript engine feature support](https://docs.servicenow.com/bundle/tokyo-application-development/page/script/JavaScript-engine-upgrade/reference/javascript-engine-feature-support.html). This page has all the new features that are supported, not supported, and disallowed.

## How?

To utilize ECMASCript 2021 on your app, just follow these simple steps:

1. Make sure your instance is upgraded to Tokyo (get a Personal Developer instance [here](https://developer.servicenow.com/))
2. Create a new app via your preferred method (eg. Studio or App Engine Studio)
3. Open the sys_app page for your app<br>![openrecord.png](openrecord.png)
4. Under "Design and Runtime" change "JavaSCript Mode" to `ECMAScript 2021 (ES12)`<br>![javascriptmode.png](javascriptmode.png)
5. Save your record. That's it!

## Looking forward

- The new features are available on scoped apps only for now but we've been told that Global scope support is on the roadmap.
- If you switch existing apps to the new engine, we do recommend that you test for functionality and ensure that existing scripts are running correctly.

## Features!

And here are all the scripts that came from the show. **The scripts are all formatted as if they are running in a `Before Update Business Rule` to demonstrate that it works server side**:

### const

This was actually available previously but would display an error to you when using it, despite allowing you to save. Almost everything else related to ECMAScript 6 and up would not allow you to save your record at all.

`const` is a way to declare and initialize a variable that will never change its value. A great way to ensure a variable that is not meant to change never does (your script will throw an error).

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	const y = 100;
	current.work_notes = x + y;

})(current, previous);
```

### let

What's the difference between `var` and `let`?

#### Scoping rules

The main difference is scoping rules. Variables declared by var keyword are scoped to the immediate function body (hence the function scope) while let variables are scoped to the immediate enclosing block denoted by { } (hence the block scope).

#### Hoisting

While variables declared with var keyword are hoisted (initialized with undefined before the code is run) which means they are accessible in their enclosing scope even before they are declared

#### Creating global object property

At the top level, let, unlike var, does not create a property on the global object

#### Redeclaration

In strict mode, var will let you re-declare the same variable in the same scope while let raises a SyntaxError.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	let y = 200;
	current.work_notes = x + y;

})(current, previous);
```

### arrow functions

How many times have we googled "how to do ____ in JavaScript?" and the top result was a StackOverflow answer that utilized arrow functions? Arrow functions are a compact alternative to traditional function expressions. Combined with other new features, there are so many use-cases for arrow functions (like quickly reordering arrays of objects!).

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	function addDescriptions(x, y){
		return x + '\n' + y;
	}
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	let addDescriptions = (x, y) => x + '\n'+ y; //one line!
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);
```

### for/of

A different kind of for/in to add to your arsenal.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	var work_notes = [];
	for (var inc in incidents){
		work_notes.push(incidents[inc]);
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	let work_notes = [];
	for (let inc of incidents){
		work_notes.push(inc); //note that no index reference is needed
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### map

The Map object holds key-value pairs and remembers the original insertion order of the keys. Any value (both objects and primitive values) may be used as either a key or a value.

Object is similar to Map—both let you set keys to values, retrieve those values, delete keys, and detect whether something is stored at a key. For this reason (and because there were no built-in alternatives), Object has been used as Map historically.

However, there are important differences that make Map preferable in some cases:

- Accidental Keys (objects initialize with prototype)
- Key types (previously just strings or symbols, now can be functions, objects, any primitive)
- Key Order (simplified to order of entry insertion)
- Size (inherent size property)
- Iteration (objects aren't inherently iterable)
- Performance (additions and removals are more performative)
- Serialization and parsing (object wins in this case)

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	const incidents = new Map();

	const keyString = 'a string';
	const keyObj = {};
	const keyFunc = function() {};
	
	inc_gr.next();
	incidents.set(keyString, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyObj, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyFunc, inc_gr.getValue('short_description'));

	let work_notes = [];
	work_notes.push('map size: ' + incidents.size);
	work_notes.push(incidents.get(keyString));
	work_notes.push(incidents.get(keyObj));
	work_notes.push(incidents.get(keyFunc)); //Finding an a value by providing a function!
	work_notes.push(incidents.get('a string'));

	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### set

The Set object lets you store unique values of any type, whether primitive values or object references. Faster, and forces uniqueness of values.

```javascript
const mySet1 = new Set()

mySet1.add(1)           // Set [ 1 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add('some text') // Set [ 1, 5, 'some text' ]
const o = {a: 1, b: 2}
mySet1.add(o)

mySet1.add({a: 1, b: 2})   // o is referencing a different object, so this is okay

mySet1.has(1)              // true
mySet1.has(3)              // false, since 3 has not been added to the set
mySet1.has(5)              // true
mySet1.has(Math.sqrt(25))  // true
mySet1.has('Some Text'.toLowerCase()) // true
mySet1.has(o)       // true

mySet1.size         // 5

mySet1.delete(5)    // removes 5 from the set
mySet1.has(5)       // false, 5 has been removed

mySet1.size         // 4, since we just removed one value

mySet1.add(5)       // Set [1, 'some text', {...}, {...}, 5] - a previously deleted item will be added as a new item, it will not retain its original position before deletion

console.log(mySet1)
// logs Set(5) [ 1, "some text", {…}, {…}, 5 ] in Firefox
// logs Set(5) { 1, "some text", {…}, {…}, 5 } in Chrome
```

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	let incidents = new Set();
	
	while (inc_gr.next()){
		incidents.add(inc_gr.getValue('short_description'));
	}
	
	current.work_notes = incidents.has(inc_gr.getValue('short_description')) + '\n' + incidents.values().next().value + '\n' + incidents.size;
	
})(current, previous);
```

### symbol

Symbol is a built-in object whose constructor returns a symbol primitive — also called a Symbol value or just a Symbol — that's guaranteed to be unique. Symbols are often used to add unique property keys to an object that won't collide with keys any other code might add to the object, and which are hidden from any mechanisms other code will typically use to access the object. That enables a form of weak encapsulation, or a weak form of information hiding.

Every Symbol() call is guaranteed to return a unique Symbol. Every Symbol.for("key") call will always return the same Symbol for a given value of "key". When Symbol.for("key") is called, if a Symbol with the given key can be found in the global Symbol registry, that Symbol is returned. Otherwise, a new Symbol is created, added to the global Symbol registry under the given key, and returned.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var incidents = [];
	let incident = {
		number: current.number,
		short_description: current.short_description
	};
	
	incidents.push(incident);
	incidents.push(incident);
	
	var incidents2 = [];
	incidents2.push(Symbol(incident));
	incidents2.push(Symbol(incident));
	
	current.work_notes = (incidents[0] == incidents[1]) + '\n' + (incidents2[0] == incidents2[1]); //Notice how the first one is true and the second is false, despite all four items being the "same"
	
})(current, previous);
```

### default params

Instead of having to check for included parameters in a function's body, we can do it directly in the parameters now.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	function add (x, y){
		if (y == null) y = 'nothing to see here';
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	function add (x, y = 'nothing to see here'){
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);
```

### spread

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	let incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}

	function sum(x, y, z) {
		return x + '\n' + y + '\n' + z;
	}
	
	const incidents_obj = { ...incidents}; //the array's items are "spread" out as parameters
	
	current.work_notes = sum(...incidents) + '\n' + JSON.stringify(incidents_obj);

})(current, previous);
```

### template strings/literals

I love this one because it makes it so much easier to copy and paste multi-line strings into my code. I use this a lot on AdventOfCode challenges!

```javascript
(function executeRule(current, previous /*null when async*/) {

	let x = `hello
	world
	lchh loves you`;
	
	current.work_notes = x; //goodbye \n

})(current, previous);
```

Another way that these are helpful are for templates (Thanks Chris Helming for the suggestion):

```javascript
(function executeRule(current, previous /*null when async*/) {

	const a = 5; 
	const b = 10; 
	current.work_notes = `Fifteen is ${a + b} and not ${2 * a + b}.`;

})(current, previous);
```

### destructuring

Okay, so destructuring is a LOT more than this but here is just an example.

```javascript
const x = [1, 2, 3, 4, 5];
const [y, z] = x;
// y: 1
// z: 2

const obj = { a: 1, b: 2 };
const { a, b } = obj;
// is equivalent to:
// const a = obj.a;
// const b = obj.b;
```

### class

Hoisting differences (functions and classes are both hoisted and declared but classes are not initialized)

```javascript
class Rectangle {
  constructor(height, width) {
    this.name = 'Rectangle';
    this.height = height;
    this.width = width;
  }
}

class FilledRectangle extends Rectangle {
  constructor(height, width, color) {
    super(height, width);
    this.name = 'Filled rectangle';
    this.color = color;
  }
}
```

### And more

That's not all! Go check it out in the docs!

### ES Sources

- https://betterprogramming.pub/difference-between-regular-functions-and-arrow-functions-f65639aba256
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/
Folder Name:

  - ./ECMASCript 2021
    - ## What?

Prior to the Tokyo Release, ServiceNow's serverside JavaScript utilized ECMAScript 5. "ECMAScript" is basically the version of JavaScript. Newer versions have come out since then (7+ years ago!) and thus, we have been missing out on some helpful functionality.

Client-side scripting is run in your web browser so usually any client script you've made on ServiceNow could utilize the newest JavaScript features, but any script running on the server was limiteded to ES5.

ServiceNow has denoted our version of JavaScript as ECMAScript 2021, which encompasses the feature roll-up of ECMAScript 6 to ECMAScript 12. To see the full documentation of changes, you can see the release notes here: [JavaScript engine feature support](https://docs.servicenow.com/bundle/tokyo-application-development/page/script/JavaScript-engine-upgrade/reference/javascript-engine-feature-support.html). This page has all the new features that are supported, not supported, and disallowed.

## How?

To utilize ECMASCript 2021 on your app, just follow these simple steps:

1. Make sure your instance is upgraded to Tokyo (get a Personal Developer instance [here](https://developer.servicenow.com/))
2. Create a new app via your preferred method (eg. Studio or App Engine Studio)
3. Open the sys_app page for your app<br>![openrecord.png](openrecord.png)
4. Under "Design and Runtime" change "JavaSCript Mode" to `ECMAScript 2021 (ES12)`<br>![javascriptmode.png](javascriptmode.png)
5. Save your record. That's it!

## Looking forward

- The new features are available on scoped apps only for now but we've been told that Global scope support is on the roadmap.
- If you switch existing apps to the new engine, we do recommend that you test for functionality and ensure that existing scripts are running correctly.

## Features!

And here are all the scripts that came from the show. **The scripts are all formatted as if they are running in a `Before Update Business Rule` to demonstrate that it works server side**:

### const

This was actually available previously but would display an error to you when using it, despite allowing you to save. Almost everything else related to ECMAScript 6 and up would not allow you to save your record at all.

`const` is a way to declare and initialize a variable that will never change its value. A great way to ensure a variable that is not meant to change never does (your script will throw an error).

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	const y = 100;
	current.work_notes = x + y;

})(current, previous);
```

### let

What's the difference between `var` and `let`?

#### Scoping rules

The main difference is scoping rules. Variables declared by var keyword are scoped to the immediate function body (hence the function scope) while let variables are scoped to the immediate enclosing block denoted by { } (hence the block scope).

#### Hoisting

While variables declared with var keyword are hoisted (initialized with undefined before the code is run) which means they are accessible in their enclosing scope even before they are declared

#### Creating global object property

At the top level, let, unlike var, does not create a property on the global object

#### Redeclaration

In strict mode, var will let you re-declare the same variable in the same scope while let raises a SyntaxError.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	let y = 200;
	current.work_notes = x + y;

})(current, previous);
```

### arrow functions

How many times have we googled "how to do ____ in JavaScript?" and the top result was a StackOverflow answer that utilized arrow functions? Arrow functions are a compact alternative to traditional function expressions. Combined with other new features, there are so many use-cases for arrow functions (like quickly reordering arrays of objects!).

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	function addDescriptions(x, y){
		return x + '\n' + y;
	}
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	let addDescriptions = (x, y) => x + '\n'+ y; //one line!
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);
```

### for/of

A different kind of for/in to add to your arsenal.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	var work_notes = [];
	for (var inc in incidents){
		work_notes.push(incidents[inc]);
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	let work_notes = [];
	for (let inc of incidents){
		work_notes.push(inc); //note that no index reference is needed
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### map

The Map object holds key-value pairs and remembers the original insertion order of the keys. Any value (both objects and primitive values) may be used as either a key or a value.

Object is similar to Map—both let you set keys to values, retrieve those values, delete keys, and detect whether something is stored at a key. For this reason (and because there were no built-in alternatives), Object has been used as Map historically.

However, there are important differences that make Map preferable in some cases:

- Accidental Keys (objects initialize with prototype)
- Key types (previously just strings or symbols, now can be functions, objects, any primitive)
- Key Order (simplified to order of entry insertion)
- Size (inherent size property)
- Iteration (objects aren't inherently iterable)
- Performance (additions and removals are more performative)
- Serialization and parsing (object wins in this case)

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	const incidents = new Map();

	const keyString = 'a string';
	const keyObj = {};
	const keyFunc = function() {};
	
	inc_gr.next();
	incidents.set(keyString, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyObj, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyFunc, inc_gr.getValue('short_description'));

	let work_notes = [];
	work_notes.push('map size: ' + incidents.size);
	work_notes.push(incidents.get(keyString));
	work_notes.push(incidents.get(keyObj));
	work_notes.push(incidents.get(keyFunc)); //Finding an a value by providing a function!
	work_notes.push(incidents.get('a string'));

	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### set

The Set object lets you store unique values of any type, whether primitive values or object references. Faster, and forces uniqueness of values.

```javascript
const mySet1 = new Set()

mySet1.add(1)           // Set [ 1 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add('some text') // Set [ 1, 5, 'some text' ]
const o = {a: 1, b: 2}
mySet1.add(o)

mySet1.add({a: 1, b: 2})   // o is referencing a different object, so this is okay

mySet1.has(1)              // true
mySet1.has(3)              // false, since 3 has not been added to the set
mySet1.has(5)              // true
mySet1.has(Math.sqrt(25))  // true
mySet1.has('Some Text'.toLowerCase()) // true
mySet1.has(o)       // true

mySet1.size         // 5

mySet1.delete(5)    // removes 5 from the set
mySet1.has(5)       // false, 5 has been removed

mySet1.size         // 4, since we just removed one value

mySet1.add(5)       // Set [1, 'some text', {...}, {...}, 5] - a previously deleted item will be added as a new item, it will not retain its original position before deletion

console.log(mySet1)
// logs Set(5) [ 1, "some text", {…}, {…}, 5 ] in Firefox
// logs Set(5) { 1, "some text", {…}, {…}, 5 } in Chrome
```

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	let incidents = new Set();
	
	while (inc_gr.next()){
		incidents.add(inc_gr.getValue('short_description'));
	}
	
	current.work_notes = incidents.has(inc_gr.getValue('short_description')) + '\n' + incidents.values().next().value + '\n' + incidents.size;
	
})(current, previous);
```

### symbol

Symbol is a built-in object whose constructor returns a symbol primitive — also called a Symbol value or just a Symbol — that's guaranteed to be unique. Symbols are often used to add unique property keys to an object that won't collide with keys any other code might add to the object, and which are hidden from any mechanisms other code will typically use to access the object. That enables a form of weak encapsulation, or a weak form of information hiding.

Every Symbol() call is guaranteed to return a unique Symbol. Every Symbol.for("key") call will always return the same Symbol for a given value of "key". When Symbol.for("key") is called, if a Symbol with the given key can be found in the global Symbol registry, that Symbol is returned. Otherwise, a new Symbol is created, added to the global Symbol registry under the given key, and returned.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var incidents = [];
	let incident = {
		number: current.number,
		short_description: current.short_description
	};
	
	incidents.push(incident);
	incidents.push(incident);
	
	var incidents2 = [];
	incidents2.push(Symbol(incident));
	incidents2.push(Symbol(incident));
	
	current.work_notes = (incidents[0] == incidents[1]) + '\n' + (incidents2[0] == incidents2[1]); //Notice how the first one is true and the second is false, despite all four items being the "same"
	
})(current, previous);
```

### default params

Instead of having to check for included parameters in a function's body, we can do it directly in the parameters now.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	function add (x, y){
		if (y == null) y = 'nothing to see here';
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	function add (x, y = 'nothing to see here'){
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);
```

### spread

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	let incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}

	function sum(x, y, z) {
		return x + '\n' + y + '\n' + z;
	}
	
	const incidents_obj = { ...incidents}; //the array's items are "spread" out as parameters
	
	current.work_notes = sum(...incidents) + '\n' + JSON.stringify(incidents_obj);

})(current, previous);
```

### template strings/literals

I love this one because it makes it so much easier to copy and paste multi-line strings into my code. I use this a lot on AdventOfCode challenges!

```javascript
(function executeRule(current, previous /*null when async*/) {

	let x = `hello
	world
	lchh loves you`;
	
	current.work_notes = x; //goodbye \n

})(current, previous);
```

Another way that these are helpful are for templates (Thanks Chris Helming for the suggestion):

```javascript
(function executeRule(current, previous /*null when async*/) {

	const a = 5; 
	const b = 10; 
	current.work_notes = `Fifteen is ${a + b} and not ${2 * a + b}.`;

})(current, previous);
```

### destructuring

Okay, so destructuring is a LOT more than this but here is just an example.

```javascript
const x = [1, 2, 3, 4, 5];
const [y, z] = x;
// y: 1
// z: 2

const obj = { a: 1, b: 2 };
const { a, b } = obj;
// is equivalent to:
// const a = obj.a;
// const b = obj.b;
```

### class

Hoisting differences (functions and classes are both hoisted and declared but classes are not initialized)

```javascript
class Rectangle {
  constructor(height, width) {
    this.name = 'Rectangle';
    this.height = height;
    this.width = width;
  }
}

class FilledRectangle extends Rectangle {
  constructor(height, width, color) {
    super(height, width);
    this.name = 'Filled rectangle';
    this.color = color;
  }
}
```

### And more

That's not all! Go check it out in the docs!

### ES Sources

- https://betterprogramming.pub/difference-between-regular-functions-and-arrow-functions-f65639aba256
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/
Folder Name:

  - ./ECMASCript 2021
    - ## What?

Prior to the Tokyo Release, ServiceNow's serverside JavaScript utilized ECMAScript 5. "ECMAScript" is basically the version of JavaScript. Newer versions have come out since then (7+ years ago!) and thus, we have been missing out on some helpful functionality.

Client-side scripting is run in your web browser so usually any client script you've made on ServiceNow could utilize the newest JavaScript features, but any script running on the server was limiteded to ES5.

ServiceNow has denoted our version of JavaScript as ECMAScript 2021, which encompasses the feature roll-up of ECMAScript 6 to ECMAScript 12. To see the full documentation of changes, you can see the release notes here: [JavaScript engine feature support](https://docs.servicenow.com/bundle/tokyo-application-development/page/script/JavaScript-engine-upgrade/reference/javascript-engine-feature-support.html). This page has all the new features that are supported, not supported, and disallowed.

## How?

To utilize ECMASCript 2021 on your app, just follow these simple steps:

1. Make sure your instance is upgraded to Tokyo (get a Personal Developer instance [here](https://developer.servicenow.com/))
2. Create a new app via your preferred method (eg. Studio or App Engine Studio)
3. Open the sys_app page for your app<br>![openrecord.png](openrecord.png)
4. Under "Design and Runtime" change "JavaSCript Mode" to `ECMAScript 2021 (ES12)`<br>![javascriptmode.png](javascriptmode.png)
5. Save your record. That's it!

## Looking forward

- The new features are available on scoped apps only for now but we've been told that Global scope support is on the roadmap.
- If you switch existing apps to the new engine, we do recommend that you test for functionality and ensure that existing scripts are running correctly.

## Features!

And here are all the scripts that came from the show. **The scripts are all formatted as if they are running in a `Before Update Business Rule` to demonstrate that it works server side**:

### const

This was actually available previously but would display an error to you when using it, despite allowing you to save. Almost everything else related to ECMAScript 6 and up would not allow you to save your record at all.

`const` is a way to declare and initialize a variable that will never change its value. A great way to ensure a variable that is not meant to change never does (your script will throw an error).

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	const y = 100;
	current.work_notes = x + y;

})(current, previous);
```

### let

What's the difference between `var` and `let`?

#### Scoping rules

The main difference is scoping rules. Variables declared by var keyword are scoped to the immediate function body (hence the function scope) while let variables are scoped to the immediate enclosing block denoted by { } (hence the block scope).

#### Hoisting

While variables declared with var keyword are hoisted (initialized with undefined before the code is run) which means they are accessible in their enclosing scope even before they are declared

#### Creating global object property

At the top level, let, unlike var, does not create a property on the global object

#### Redeclaration

In strict mode, var will let you re-declare the same variable in the same scope while let raises a SyntaxError.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	let y = 200;
	current.work_notes = x + y;

})(current, previous);
```

### arrow functions

How many times have we googled "how to do ____ in JavaScript?" and the top result was a StackOverflow answer that utilized arrow functions? Arrow functions are a compact alternative to traditional function expressions. Combined with other new features, there are so many use-cases for arrow functions (like quickly reordering arrays of objects!).

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	function addDescriptions(x, y){
		return x + '\n' + y;
	}
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	let addDescriptions = (x, y) => x + '\n'+ y; //one line!
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);
```

### for/of

A different kind of for/in to add to your arsenal.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	var work_notes = [];
	for (var inc in incidents){
		work_notes.push(incidents[inc]);
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	let work_notes = [];
	for (let inc of incidents){
		work_notes.push(inc); //note that no index reference is needed
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### map

The Map object holds key-value pairs and remembers the original insertion order of the keys. Any value (both objects and primitive values) may be used as either a key or a value.

Object is similar to Map—both let you set keys to values, retrieve those values, delete keys, and detect whether something is stored at a key. For this reason (and because there were no built-in alternatives), Object has been used as Map historically.

However, there are important differences that make Map preferable in some cases:

- Accidental Keys (objects initialize with prototype)
- Key types (previously just strings or symbols, now can be functions, objects, any primitive)
- Key Order (simplified to order of entry insertion)
- Size (inherent size property)
- Iteration (objects aren't inherently iterable)
- Performance (additions and removals are more performative)
- Serialization and parsing (object wins in this case)

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	const incidents = new Map();

	const keyString = 'a string';
	const keyObj = {};
	const keyFunc = function() {};
	
	inc_gr.next();
	incidents.set(keyString, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyObj, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyFunc, inc_gr.getValue('short_description'));

	let work_notes = [];
	work_notes.push('map size: ' + incidents.size);
	work_notes.push(incidents.get(keyString));
	work_notes.push(incidents.get(keyObj));
	work_notes.push(incidents.get(keyFunc)); //Finding an a value by providing a function!
	work_notes.push(incidents.get('a string'));

	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### set

The Set object lets you store unique values of any type, whether primitive values or object references. Faster, and forces uniqueness of values.

```javascript
const mySet1 = new Set()

mySet1.add(1)           // Set [ 1 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add('some text') // Set [ 1, 5, 'some text' ]
const o = {a: 1, b: 2}
mySet1.add(o)

mySet1.add({a: 1, b: 2})   // o is referencing a different object, so this is okay

mySet1.has(1)              // true
mySet1.has(3)              // false, since 3 has not been added to the set
mySet1.has(5)              // true
mySet1.has(Math.sqrt(25))  // true
mySet1.has('Some Text'.toLowerCase()) // true
mySet1.has(o)       // true

mySet1.size         // 5

mySet1.delete(5)    // removes 5 from the set
mySet1.has(5)       // false, 5 has been removed

mySet1.size         // 4, since we just removed one value

mySet1.add(5)       // Set [1, 'some text', {...}, {...}, 5] - a previously deleted item will be added as a new item, it will not retain its original position before deletion

console.log(mySet1)
// logs Set(5) [ 1, "some text", {…}, {…}, 5 ] in Firefox
// logs Set(5) { 1, "some text", {…}, {…}, 5 } in Chrome
```

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	let incidents = new Set();
	
	while (inc_gr.next()){
		incidents.add(inc_gr.getValue('short_description'));
	}
	
	current.work_notes = incidents.has(inc_gr.getValue('short_description')) + '\n' + incidents.values().next().value + '\n' + incidents.size;
	
})(current, previous);
```

### symbol

Symbol is a built-in object whose constructor returns a symbol primitive — also called a Symbol value or just a Symbol — that's guaranteed to be unique. Symbols are often used to add unique property keys to an object that won't collide with keys any other code might add to the object, and which are hidden from any mechanisms other code will typically use to access the object. That enables a form of weak encapsulation, or a weak form of information hiding.

Every Symbol() call is guaranteed to return a unique Symbol. Every Symbol.for("key") call will always return the same Symbol for a given value of "key". When Symbol.for("key") is called, if a Symbol with the given key can be found in the global Symbol registry, that Symbol is returned. Otherwise, a new Symbol is created, added to the global Symbol registry under the given key, and returned.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var incidents = [];
	let incident = {
		number: current.number,
		short_description: current.short_description
	};
	
	incidents.push(incident);
	incidents.push(incident);
	
	var incidents2 = [];
	incidents2.push(Symbol(incident));
	incidents2.push(Symbol(incident));
	
	current.work_notes = (incidents[0] == incidents[1]) + '\n' + (incidents2[0] == incidents2[1]); //Notice how the first one is true and the second is false, despite all four items being the "same"
	
})(current, previous);
```

### default params

Instead of having to check for included parameters in a function's body, we can do it directly in the parameters now.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	function add (x, y){
		if (y == null) y = 'nothing to see here';
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	function add (x, y = 'nothing to see here'){
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);
```

### spread

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	let incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}

	function sum(x, y, z) {
		return x + '\n' + y + '\n' + z;
	}
	
	const incidents_obj = { ...incidents}; //the array's items are "spread" out as parameters
	
	current.work_notes = sum(...incidents) + '\n' + JSON.stringify(incidents_obj);

})(current, previous);
```

### template strings/literals

I love this one because it makes it so much easier to copy and paste multi-line strings into my code. I use this a lot on AdventOfCode challenges!

```javascript
(function executeRule(current, previous /*null when async*/) {

	let x = `hello
	world
	lchh loves you`;
	
	current.work_notes = x; //goodbye \n

})(current, previous);
```

Another way that these are helpful are for templates (Thanks Chris Helming for the suggestion):

```javascript
(function executeRule(current, previous /*null when async*/) {

	const a = 5; 
	const b = 10; 
	current.work_notes = `Fifteen is ${a + b} and not ${2 * a + b}.`;

})(current, previous);
```

### destructuring

Okay, so destructuring is a LOT more than this but here is just an example.

```javascript
const x = [1, 2, 3, 4, 5];
const [y, z] = x;
// y: 1
// z: 2

const obj = { a: 1, b: 2 };
const { a, b } = obj;
// is equivalent to:
// const a = obj.a;
// const b = obj.b;
```

### class

Hoisting differences (functions and classes are both hoisted and declared but classes are not initialized)

```javascript
class Rectangle {
  constructor(height, width) {
    this.name = 'Rectangle';
    this.height = height;
    this.width = width;
  }
}

class FilledRectangle extends Rectangle {
  constructor(height, width, color) {
    super(height, width);
    this.name = 'Filled rectangle';
    this.color = color;
  }
}
```

### And more

That's not all! Go check it out in the docs!

### ES Sources

- https://betterprogramming.pub/difference-between-regular-functions-and-arrow-functions-f65639aba256
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/
Folder Name:

  - ./ECMASCript 2021
    - ## What?

Prior to the Tokyo Release, ServiceNow's serverside JavaScript utilized ECMAScript 5. "ECMAScript" is basically the version of JavaScript. Newer versions have come out since then (7+ years ago!) and thus, we have been missing out on some helpful functionality.

Client-side scripting is run in your web browser so usually any client script you've made on ServiceNow could utilize the newest JavaScript features, but any script running on the server was limiteded to ES5.

ServiceNow has denoted our version of JavaScript as ECMAScript 2021, which encompasses the feature roll-up of ECMAScript 6 to ECMAScript 12. To see the full documentation of changes, you can see the release notes here: [JavaScript engine feature support](https://docs.servicenow.com/bundle/tokyo-application-development/page/script/JavaScript-engine-upgrade/reference/javascript-engine-feature-support.html). This page has all the new features that are supported, not supported, and disallowed.

## How?

To utilize ECMASCript 2021 on your app, just follow these simple steps:

1. Make sure your instance is upgraded to Tokyo (get a Personal Developer instance [here](https://developer.servicenow.com/))
2. Create a new app via your preferred method (eg. Studio or App Engine Studio)
3. Open the sys_app page for your app<br>![openrecord.png](openrecord.png)
4. Under "Design and Runtime" change "JavaSCript Mode" to `ECMAScript 2021 (ES12)`<br>![javascriptmode.png](javascriptmode.png)
5. Save your record. That's it!

## Looking forward

- The new features are available on scoped apps only for now but we've been told that Global scope support is on the roadmap.
- If you switch existing apps to the new engine, we do recommend that you test for functionality and ensure that existing scripts are running correctly.

## Features!

And here are all the scripts that came from the show. **The scripts are all formatted as if they are running in a `Before Update Business Rule` to demonstrate that it works server side**:

### const

This was actually available previously but would display an error to you when using it, despite allowing you to save. Almost everything else related to ECMAScript 6 and up would not allow you to save your record at all.

`const` is a way to declare and initialize a variable that will never change its value. A great way to ensure a variable that is not meant to change never does (your script will throw an error).

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	const y = 100;
	current.work_notes = x + y;

})(current, previous);
```

### let

What's the difference between `var` and `let`?

#### Scoping rules

The main difference is scoping rules. Variables declared by var keyword are scoped to the immediate function body (hence the function scope) while let variables are scoped to the immediate enclosing block denoted by { } (hence the block scope).

#### Hoisting

While variables declared with var keyword are hoisted (initialized with undefined before the code is run) which means they are accessible in their enclosing scope even before they are declared

#### Creating global object property

At the top level, let, unlike var, does not create a property on the global object

#### Redeclaration

In strict mode, var will let you re-declare the same variable in the same scope while let raises a SyntaxError.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	let y = 200;
	current.work_notes = x + y;

})(current, previous);
```

### arrow functions

How many times have we googled "how to do ____ in JavaScript?" and the top result was a StackOverflow answer that utilized arrow functions? Arrow functions are a compact alternative to traditional function expressions. Combined with other new features, there are so many use-cases for arrow functions (like quickly reordering arrays of objects!).

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	function addDescriptions(x, y){
		return x + '\n' + y;
	}
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	let addDescriptions = (x, y) => x + '\n'+ y; //one line!
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);
```

### for/of

A different kind of for/in to add to your arsenal.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	var work_notes = [];
	for (var inc in incidents){
		work_notes.push(incidents[inc]);
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	let work_notes = [];
	for (let inc of incidents){
		work_notes.push(inc); //note that no index reference is needed
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### map

The Map object holds key-value pairs and remembers the original insertion order of the keys. Any value (both objects and primitive values) may be used as either a key or a value.

Object is similar to Map—both let you set keys to values, retrieve those values, delete keys, and detect whether something is stored at a key. For this reason (and because there were no built-in alternatives), Object has been used as Map historically.

However, there are important differences that make Map preferable in some cases:

- Accidental Keys (objects initialize with prototype)
- Key types (previously just strings or symbols, now can be functions, objects, any primitive)
- Key Order (simplified to order of entry insertion)
- Size (inherent size property)
- Iteration (objects aren't inherently iterable)
- Performance (additions and removals are more performative)
- Serialization and parsing (object wins in this case)

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	const incidents = new Map();

	const keyString = 'a string';
	const keyObj = {};
	const keyFunc = function() {};
	
	inc_gr.next();
	incidents.set(keyString, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyObj, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyFunc, inc_gr.getValue('short_description'));

	let work_notes = [];
	work_notes.push('map size: ' + incidents.size);
	work_notes.push(incidents.get(keyString));
	work_notes.push(incidents.get(keyObj));
	work_notes.push(incidents.get(keyFunc)); //Finding an a value by providing a function!
	work_notes.push(incidents.get('a string'));

	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### set

The Set object lets you store unique values of any type, whether primitive values or object references. Faster, and forces uniqueness of values.

```javascript
const mySet1 = new Set()

mySet1.add(1)           // Set [ 1 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add('some text') // Set [ 1, 5, 'some text' ]
const o = {a: 1, b: 2}
mySet1.add(o)

mySet1.add({a: 1, b: 2})   // o is referencing a different object, so this is okay

mySet1.has(1)              // true
mySet1.has(3)              // false, since 3 has not been added to the set
mySet1.has(5)              // true
mySet1.has(Math.sqrt(25))  // true
mySet1.has('Some Text'.toLowerCase()) // true
mySet1.has(o)       // true

mySet1.size         // 5

mySet1.delete(5)    // removes 5 from the set
mySet1.has(5)       // false, 5 has been removed

mySet1.size         // 4, since we just removed one value

mySet1.add(5)       // Set [1, 'some text', {...}, {...}, 5] - a previously deleted item will be added as a new item, it will not retain its original position before deletion

console.log(mySet1)
// logs Set(5) [ 1, "some text", {…}, {…}, 5 ] in Firefox
// logs Set(5) { 1, "some text", {…}, {…}, 5 } in Chrome
```

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	let incidents = new Set();
	
	while (inc_gr.next()){
		incidents.add(inc_gr.getValue('short_description'));
	}
	
	current.work_notes = incidents.has(inc_gr.getValue('short_description')) + '\n' + incidents.values().next().value + '\n' + incidents.size;
	
})(current, previous);
```

### symbol

Symbol is a built-in object whose constructor returns a symbol primitive — also called a Symbol value or just a Symbol — that's guaranteed to be unique. Symbols are often used to add unique property keys to an object that won't collide with keys any other code might add to the object, and which are hidden from any mechanisms other code will typically use to access the object. That enables a form of weak encapsulation, or a weak form of information hiding.

Every Symbol() call is guaranteed to return a unique Symbol. Every Symbol.for("key") call will always return the same Symbol for a given value of "key". When Symbol.for("key") is called, if a Symbol with the given key can be found in the global Symbol registry, that Symbol is returned. Otherwise, a new Symbol is created, added to the global Symbol registry under the given key, and returned.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var incidents = [];
	let incident = {
		number: current.number,
		short_description: current.short_description
	};
	
	incidents.push(incident);
	incidents.push(incident);
	
	var incidents2 = [];
	incidents2.push(Symbol(incident));
	incidents2.push(Symbol(incident));
	
	current.work_notes = (incidents[0] == incidents[1]) + '\n' + (incidents2[0] == incidents2[1]); //Notice how the first one is true and the second is false, despite all four items being the "same"
	
})(current, previous);
```

### default params

Instead of having to check for included parameters in a function's body, we can do it directly in the parameters now.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	function add (x, y){
		if (y == null) y = 'nothing to see here';
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	function add (x, y = 'nothing to see here'){
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);
```

### spread

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	let incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}

	function sum(x, y, z) {
		return x + '\n' + y + '\n' + z;
	}
	
	const incidents_obj = { ...incidents}; //the array's items are "spread" out as parameters
	
	current.work_notes = sum(...incidents) + '\n' + JSON.stringify(incidents_obj);

})(current, previous);
```

### template strings/literals

I love this one because it makes it so much easier to copy and paste multi-line strings into my code. I use this a lot on AdventOfCode challenges!

```javascript
(function executeRule(current, previous /*null when async*/) {

	let x = `hello
	world
	lchh loves you`;
	
	current.work_notes = x; //goodbye \n

})(current, previous);
```

Another way that these are helpful are for templates (Thanks Chris Helming for the suggestion):

```javascript
(function executeRule(current, previous /*null when async*/) {

	const a = 5; 
	const b = 10; 
	current.work_notes = `Fifteen is ${a + b} and not ${2 * a + b}.`;

})(current, previous);
```

### destructuring

Okay, so destructuring is a LOT more than this but here is just an example.

```javascript
const x = [1, 2, 3, 4, 5];
const [y, z] = x;
// y: 1
// z: 2

const obj = { a: 1, b: 2 };
const { a, b } = obj;
// is equivalent to:
// const a = obj.a;
// const b = obj.b;
```

### class

Hoisting differences (functions and classes are both hoisted and declared but classes are not initialized)

```javascript
class Rectangle {
  constructor(height, width) {
    this.name = 'Rectangle';
    this.height = height;
    this.width = width;
  }
}

class FilledRectangle extends Rectangle {
  constructor(height, width, color) {
    super(height, width);
    this.name = 'Filled rectangle';
    this.color = color;
  }
}
```

### And more

That's not all! Go check it out in the docs!

### ES Sources

- https://betterprogramming.pub/difference-between-regular-functions-and-arrow-functions-f65639aba256
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/
Folder Name:

  - ./ECMASCript 2021
    - ## What?

Prior to the Tokyo Release, ServiceNow's serverside JavaScript utilized ECMAScript 5. "ECMAScript" is basically the version of JavaScript. Newer versions have come out since then (7+ years ago!) and thus, we have been missing out on some helpful functionality.

Client-side scripting is run in your web browser so usually any client script you've made on ServiceNow could utilize the newest JavaScript features, but any script running on the server was limiteded to ES5.

ServiceNow has denoted our version of JavaScript as ECMAScript 2021, which encompasses the feature roll-up of ECMAScript 6 to ECMAScript 12. To see the full documentation of changes, you can see the release notes here: [JavaScript engine feature support](https://docs.servicenow.com/bundle/tokyo-application-development/page/script/JavaScript-engine-upgrade/reference/javascript-engine-feature-support.html). This page has all the new features that are supported, not supported, and disallowed.

## How?

To utilize ECMASCript 2021 on your app, just follow these simple steps:

1. Make sure your instance is upgraded to Tokyo (get a Personal Developer instance [here](https://developer.servicenow.com/))
2. Create a new app via your preferred method (eg. Studio or App Engine Studio)
3. Open the sys_app page for your app<br>![openrecord.png](openrecord.png)
4. Under "Design and Runtime" change "JavaSCript Mode" to `ECMAScript 2021 (ES12)`<br>![javascriptmode.png](javascriptmode.png)
5. Save your record. That's it!

## Looking forward

- The new features are available on scoped apps only for now but we've been told that Global scope support is on the roadmap.
- If you switch existing apps to the new engine, we do recommend that you test for functionality and ensure that existing scripts are running correctly.

## Features!

And here are all the scripts that came from the show. **The scripts are all formatted as if they are running in a `Before Update Business Rule` to demonstrate that it works server side**:

### const

This was actually available previously but would display an error to you when using it, despite allowing you to save. Almost everything else related to ECMAScript 6 and up would not allow you to save your record at all.

`const` is a way to declare and initialize a variable that will never change its value. A great way to ensure a variable that is not meant to change never does (your script will throw an error).

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	const y = 100;
	current.work_notes = x + y;

})(current, previous);
```

### let

What's the difference between `var` and `let`?

#### Scoping rules

The main difference is scoping rules. Variables declared by var keyword are scoped to the immediate function body (hence the function scope) while let variables are scoped to the immediate enclosing block denoted by { } (hence the block scope).

#### Hoisting

While variables declared with var keyword are hoisted (initialized with undefined before the code is run) which means they are accessible in their enclosing scope even before they are declared

#### Creating global object property

At the top level, let, unlike var, does not create a property on the global object

#### Redeclaration

In strict mode, var will let you re-declare the same variable in the same scope while let raises a SyntaxError.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	let y = 200;
	current.work_notes = x + y;

})(current, previous);
```

### arrow functions

How many times have we googled "how to do ____ in JavaScript?" and the top result was a StackOverflow answer that utilized arrow functions? Arrow functions are a compact alternative to traditional function expressions. Combined with other new features, there are so many use-cases for arrow functions (like quickly reordering arrays of objects!).

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	function addDescriptions(x, y){
		return x + '\n' + y;
	}
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	let addDescriptions = (x, y) => x + '\n'+ y; //one line!
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);
```

### for/of

A different kind of for/in to add to your arsenal.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	var work_notes = [];
	for (var inc in incidents){
		work_notes.push(incidents[inc]);
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	let work_notes = [];
	for (let inc of incidents){
		work_notes.push(inc); //note that no index reference is needed
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### map

The Map object holds key-value pairs and remembers the original insertion order of the keys. Any value (both objects and primitive values) may be used as either a key or a value.

Object is similar to Map—both let you set keys to values, retrieve those values, delete keys, and detect whether something is stored at a key. For this reason (and because there were no built-in alternatives), Object has been used as Map historically.

However, there are important differences that make Map preferable in some cases:

- Accidental Keys (objects initialize with prototype)
- Key types (previously just strings or symbols, now can be functions, objects, any primitive)
- Key Order (simplified to order of entry insertion)
- Size (inherent size property)
- Iteration (objects aren't inherently iterable)
- Performance (additions and removals are more performative)
- Serialization and parsing (object wins in this case)

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	const incidents = new Map();

	const keyString = 'a string';
	const keyObj = {};
	const keyFunc = function() {};
	
	inc_gr.next();
	incidents.set(keyString, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyObj, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyFunc, inc_gr.getValue('short_description'));

	let work_notes = [];
	work_notes.push('map size: ' + incidents.size);
	work_notes.push(incidents.get(keyString));
	work_notes.push(incidents.get(keyObj));
	work_notes.push(incidents.get(keyFunc)); //Finding an a value by providing a function!
	work_notes.push(incidents.get('a string'));

	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### set

The Set object lets you store unique values of any type, whether primitive values or object references. Faster, and forces uniqueness of values.

```javascript
const mySet1 = new Set()

mySet1.add(1)           // Set [ 1 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add('some text') // Set [ 1, 5, 'some text' ]
const o = {a: 1, b: 2}
mySet1.add(o)

mySet1.add({a: 1, b: 2})   // o is referencing a different object, so this is okay

mySet1.has(1)              // true
mySet1.has(3)              // false, since 3 has not been added to the set
mySet1.has(5)              // true
mySet1.has(Math.sqrt(25))  // true
mySet1.has('Some Text'.toLowerCase()) // true
mySet1.has(o)       // true

mySet1.size         // 5

mySet1.delete(5)    // removes 5 from the set
mySet1.has(5)       // false, 5 has been removed

mySet1.size         // 4, since we just removed one value

mySet1.add(5)       // Set [1, 'some text', {...}, {...}, 5] - a previously deleted item will be added as a new item, it will not retain its original position before deletion

console.log(mySet1)
// logs Set(5) [ 1, "some text", {…}, {…}, 5 ] in Firefox
// logs Set(5) { 1, "some text", {…}, {…}, 5 } in Chrome
```

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	let incidents = new Set();
	
	while (inc_gr.next()){
		incidents.add(inc_gr.getValue('short_description'));
	}
	
	current.work_notes = incidents.has(inc_gr.getValue('short_description')) + '\n' + incidents.values().next().value + '\n' + incidents.size;
	
})(current, previous);
```

### symbol

Symbol is a built-in object whose constructor returns a symbol primitive — also called a Symbol value or just a Symbol — that's guaranteed to be unique. Symbols are often used to add unique property keys to an object that won't collide with keys any other code might add to the object, and which are hidden from any mechanisms other code will typically use to access the object. That enables a form of weak encapsulation, or a weak form of information hiding.

Every Symbol() call is guaranteed to return a unique Symbol. Every Symbol.for("key") call will always return the same Symbol for a given value of "key". When Symbol.for("key") is called, if a Symbol with the given key can be found in the global Symbol registry, that Symbol is returned. Otherwise, a new Symbol is created, added to the global Symbol registry under the given key, and returned.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var incidents = [];
	let incident = {
		number: current.number,
		short_description: current.short_description
	};
	
	incidents.push(incident);
	incidents.push(incident);
	
	var incidents2 = [];
	incidents2.push(Symbol(incident));
	incidents2.push(Symbol(incident));
	
	current.work_notes = (incidents[0] == incidents[1]) + '\n' + (incidents2[0] == incidents2[1]); //Notice how the first one is true and the second is false, despite all four items being the "same"
	
})(current, previous);
```

### default params

Instead of having to check for included parameters in a function's body, we can do it directly in the parameters now.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	function add (x, y){
		if (y == null) y = 'nothing to see here';
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	function add (x, y = 'nothing to see here'){
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);
```

### spread

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	let incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}

	function sum(x, y, z) {
		return x + '\n' + y + '\n' + z;
	}
	
	const incidents_obj = { ...incidents}; //the array's items are "spread" out as parameters
	
	current.work_notes = sum(...incidents) + '\n' + JSON.stringify(incidents_obj);

})(current, previous);
```

### template strings/literals

I love this one because it makes it so much easier to copy and paste multi-line strings into my code. I use this a lot on AdventOfCode challenges!

```javascript
(function executeRule(current, previous /*null when async*/) {

	let x = `hello
	world
	lchh loves you`;
	
	current.work_notes = x; //goodbye \n

})(current, previous);
```

Another way that these are helpful are for templates (Thanks Chris Helming for the suggestion):

```javascript
(function executeRule(current, previous /*null when async*/) {

	const a = 5; 
	const b = 10; 
	current.work_notes = `Fifteen is ${a + b} and not ${2 * a + b}.`;

})(current, previous);
```

### destructuring

Okay, so destructuring is a LOT more than this but here is just an example.

```javascript
const x = [1, 2, 3, 4, 5];
const [y, z] = x;
// y: 1
// z: 2

const obj = { a: 1, b: 2 };
const { a, b } = obj;
// is equivalent to:
// const a = obj.a;
// const b = obj.b;
```

### class

Hoisting differences (functions and classes are both hoisted and declared but classes are not initialized)

```javascript
class Rectangle {
  constructor(height, width) {
    this.name = 'Rectangle';
    this.height = height;
    this.width = width;
  }
}

class FilledRectangle extends Rectangle {
  constructor(height, width, color) {
    super(height, width);
    this.name = 'Filled rectangle';
    this.color = color;
  }
}
```

### And more

That's not all! Go check it out in the docs!

### ES Sources

- https://betterprogramming.pub/difference-between-regular-functions-and-arrow-functions-f65639aba256
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/
Folder Name:

  - ./ECMASCript 2021
    - ## What?

Prior to the Tokyo Release, ServiceNow's serverside JavaScript utilized ECMAScript 5. "ECMAScript" is basically the version of JavaScript. Newer versions have come out since then (7+ years ago!) and thus, we have been missing out on some helpful functionality.

Client-side scripting is run in your web browser so usually any client script you've made on ServiceNow could utilize the newest JavaScript features, but any script running on the server was limiteded to ES5.

ServiceNow has denoted our version of JavaScript as ECMAScript 2021, which encompasses the feature roll-up of ECMAScript 6 to ECMAScript 12. To see the full documentation of changes, you can see the release notes here: [JavaScript engine feature support](https://docs.servicenow.com/bundle/tokyo-application-development/page/script/JavaScript-engine-upgrade/reference/javascript-engine-feature-support.html). This page has all the new features that are supported, not supported, and disallowed.

## How?

To utilize ECMASCript 2021 on your app, just follow these simple steps:

1. Make sure your instance is upgraded to Tokyo (get a Personal Developer instance [here](https://developer.servicenow.com/))
2. Create a new app via your preferred method (eg. Studio or App Engine Studio)
3. Open the sys_app page for your app<br>![openrecord.png](openrecord.png)
4. Under "Design and Runtime" change "JavaSCript Mode" to `ECMAScript 2021 (ES12)`<br>![javascriptmode.png](javascriptmode.png)
5. Save your record. That's it!

## Looking forward

- The new features are available on scoped apps only for now but we've been told that Global scope support is on the roadmap.
- If you switch existing apps to the new engine, we do recommend that you test for functionality and ensure that existing scripts are running correctly.

## Features!

And here are all the scripts that came from the show. **The scripts are all formatted as if they are running in a `Before Update Business Rule` to demonstrate that it works server side**:

### const

This was actually available previously but would display an error to you when using it, despite allowing you to save. Almost everything else related to ECMAScript 6 and up would not allow you to save your record at all.

`const` is a way to declare and initialize a variable that will never change its value. A great way to ensure a variable that is not meant to change never does (your script will throw an error).

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	const y = 100;
	current.work_notes = x + y;

})(current, previous);
```

### let

What's the difference between `var` and `let`?

#### Scoping rules

The main difference is scoping rules. Variables declared by var keyword are scoped to the immediate function body (hence the function scope) while let variables are scoped to the immediate enclosing block denoted by { } (hence the block scope).

#### Hoisting

While variables declared with var keyword are hoisted (initialized with undefined before the code is run) which means they are accessible in their enclosing scope even before they are declared

#### Creating global object property

At the top level, let, unlike var, does not create a property on the global object

#### Redeclaration

In strict mode, var will let you re-declare the same variable in the same scope while let raises a SyntaxError.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	let y = 200;
	current.work_notes = x + y;

})(current, previous);
```

### arrow functions

How many times have we googled "how to do ____ in JavaScript?" and the top result was a StackOverflow answer that utilized arrow functions? Arrow functions are a compact alternative to traditional function expressions. Combined with other new features, there are so many use-cases for arrow functions (like quickly reordering arrays of objects!).

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	function addDescriptions(x, y){
		return x + '\n' + y;
	}
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	let addDescriptions = (x, y) => x + '\n'+ y; //one line!
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);
```

### for/of

A different kind of for/in to add to your arsenal.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	var work_notes = [];
	for (var inc in incidents){
		work_notes.push(incidents[inc]);
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	let work_notes = [];
	for (let inc of incidents){
		work_notes.push(inc); //note that no index reference is needed
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### map

The Map object holds key-value pairs and remembers the original insertion order of the keys. Any value (both objects and primitive values) may be used as either a key or a value.

Object is similar to Map—both let you set keys to values, retrieve those values, delete keys, and detect whether something is stored at a key. For this reason (and because there were no built-in alternatives), Object has been used as Map historically.

However, there are important differences that make Map preferable in some cases:

- Accidental Keys (objects initialize with prototype)
- Key types (previously just strings or symbols, now can be functions, objects, any primitive)
- Key Order (simplified to order of entry insertion)
- Size (inherent size property)
- Iteration (objects aren't inherently iterable)
- Performance (additions and removals are more performative)
- Serialization and parsing (object wins in this case)

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	const incidents = new Map();

	const keyString = 'a string';
	const keyObj = {};
	const keyFunc = function() {};
	
	inc_gr.next();
	incidents.set(keyString, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyObj, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyFunc, inc_gr.getValue('short_description'));

	let work_notes = [];
	work_notes.push('map size: ' + incidents.size);
	work_notes.push(incidents.get(keyString));
	work_notes.push(incidents.get(keyObj));
	work_notes.push(incidents.get(keyFunc)); //Finding an a value by providing a function!
	work_notes.push(incidents.get('a string'));

	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### set

The Set object lets you store unique values of any type, whether primitive values or object references. Faster, and forces uniqueness of values.

```javascript
const mySet1 = new Set()

mySet1.add(1)           // Set [ 1 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add('some text') // Set [ 1, 5, 'some text' ]
const o = {a: 1, b: 2}
mySet1.add(o)

mySet1.add({a: 1, b: 2})   // o is referencing a different object, so this is okay

mySet1.has(1)              // true
mySet1.has(3)              // false, since 3 has not been added to the set
mySet1.has(5)              // true
mySet1.has(Math.sqrt(25))  // true
mySet1.has('Some Text'.toLowerCase()) // true
mySet1.has(o)       // true

mySet1.size         // 5

mySet1.delete(5)    // removes 5 from the set
mySet1.has(5)       // false, 5 has been removed

mySet1.size         // 4, since we just removed one value

mySet1.add(5)       // Set [1, 'some text', {...}, {...}, 5] - a previously deleted item will be added as a new item, it will not retain its original position before deletion

console.log(mySet1)
// logs Set(5) [ 1, "some text", {…}, {…}, 5 ] in Firefox
// logs Set(5) { 1, "some text", {…}, {…}, 5 } in Chrome
```

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	let incidents = new Set();
	
	while (inc_gr.next()){
		incidents.add(inc_gr.getValue('short_description'));
	}
	
	current.work_notes = incidents.has(inc_gr.getValue('short_description')) + '\n' + incidents.values().next().value + '\n' + incidents.size;
	
})(current, previous);
```

### symbol

Symbol is a built-in object whose constructor returns a symbol primitive — also called a Symbol value or just a Symbol — that's guaranteed to be unique. Symbols are often used to add unique property keys to an object that won't collide with keys any other code might add to the object, and which are hidden from any mechanisms other code will typically use to access the object. That enables a form of weak encapsulation, or a weak form of information hiding.

Every Symbol() call is guaranteed to return a unique Symbol. Every Symbol.for("key") call will always return the same Symbol for a given value of "key". When Symbol.for("key") is called, if a Symbol with the given key can be found in the global Symbol registry, that Symbol is returned. Otherwise, a new Symbol is created, added to the global Symbol registry under the given key, and returned.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var incidents = [];
	let incident = {
		number: current.number,
		short_description: current.short_description
	};
	
	incidents.push(incident);
	incidents.push(incident);
	
	var incidents2 = [];
	incidents2.push(Symbol(incident));
	incidents2.push(Symbol(incident));
	
	current.work_notes = (incidents[0] == incidents[1]) + '\n' + (incidents2[0] == incidents2[1]); //Notice how the first one is true and the second is false, despite all four items being the "same"
	
})(current, previous);
```

### default params

Instead of having to check for included parameters in a function's body, we can do it directly in the parameters now.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	function add (x, y){
		if (y == null) y = 'nothing to see here';
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	function add (x, y = 'nothing to see here'){
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);
```

### spread

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	let incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}

	function sum(x, y, z) {
		return x + '\n' + y + '\n' + z;
	}
	
	const incidents_obj = { ...incidents}; //the array's items are "spread" out as parameters
	
	current.work_notes = sum(...incidents) + '\n' + JSON.stringify(incidents_obj);

})(current, previous);
```

### template strings/literals

I love this one because it makes it so much easier to copy and paste multi-line strings into my code. I use this a lot on AdventOfCode challenges!

```javascript
(function executeRule(current, previous /*null when async*/) {

	let x = `hello
	world
	lchh loves you`;
	
	current.work_notes = x; //goodbye \n

})(current, previous);
```

Another way that these are helpful are for templates (Thanks Chris Helming for the suggestion):

```javascript
(function executeRule(current, previous /*null when async*/) {

	const a = 5; 
	const b = 10; 
	current.work_notes = `Fifteen is ${a + b} and not ${2 * a + b}.`;

})(current, previous);
```

### destructuring

Okay, so destructuring is a LOT more than this but here is just an example.

```javascript
const x = [1, 2, 3, 4, 5];
const [y, z] = x;
// y: 1
// z: 2

const obj = { a: 1, b: 2 };
const { a, b } = obj;
// is equivalent to:
// const a = obj.a;
// const b = obj.b;
```

### class

Hoisting differences (functions and classes are both hoisted and declared but classes are not initialized)

```javascript
class Rectangle {
  constructor(height, width) {
    this.name = 'Rectangle';
    this.height = height;
    this.width = width;
  }
}

class FilledRectangle extends Rectangle {
  constructor(height, width, color) {
    super(height, width);
    this.name = 'Filled rectangle';
    this.color = color;
  }
}
```

### And more

That's not all! Go check it out in the docs!

### ES Sources

- https://betterprogramming.pub/difference-between-regular-functions-and-arrow-functions-f65639aba256
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/
Folder Name:

  - ./ECMASCript 2021
    - ## What?

Prior to the Tokyo Release, ServiceNow's serverside JavaScript utilized ECMAScript 5. "ECMAScript" is basically the version of JavaScript. Newer versions have come out since then (7+ years ago!) and thus, we have been missing out on some helpful functionality.

Client-side scripting is run in your web browser so usually any client script you've made on ServiceNow could utilize the newest JavaScript features, but any script running on the server was limiteded to ES5.

ServiceNow has denoted our version of JavaScript as ECMAScript 2021, which encompasses the feature roll-up of ECMAScript 6 to ECMAScript 12. To see the full documentation of changes, you can see the release notes here: [JavaScript engine feature support](https://docs.servicenow.com/bundle/tokyo-application-development/page/script/JavaScript-engine-upgrade/reference/javascript-engine-feature-support.html). This page has all the new features that are supported, not supported, and disallowed.

## How?

To utilize ECMASCript 2021 on your app, just follow these simple steps:

1. Make sure your instance is upgraded to Tokyo (get a Personal Developer instance [here](https://developer.servicenow.com/))
2. Create a new app via your preferred method (eg. Studio or App Engine Studio)
3. Open the sys_app page for your app<br>![openrecord.png](openrecord.png)
4. Under "Design and Runtime" change "JavaSCript Mode" to `ECMAScript 2021 (ES12)`<br>![javascriptmode.png](javascriptmode.png)
5. Save your record. That's it!

## Looking forward

- The new features are available on scoped apps only for now but we've been told that Global scope support is on the roadmap.
- If you switch existing apps to the new engine, we do recommend that you test for functionality and ensure that existing scripts are running correctly.

## Features!

And here are all the scripts that came from the show. **The scripts are all formatted as if they are running in a `Before Update Business Rule` to demonstrate that it works server side**:

### const

This was actually available previously but would display an error to you when using it, despite allowing you to save. Almost everything else related to ECMAScript 6 and up would not allow you to save your record at all.

`const` is a way to declare and initialize a variable that will never change its value. A great way to ensure a variable that is not meant to change never does (your script will throw an error).

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	const y = 100;
	current.work_notes = x + y;

})(current, previous);
```

### let

What's the difference between `var` and `let`?

#### Scoping rules

The main difference is scoping rules. Variables declared by var keyword are scoped to the immediate function body (hence the function scope) while let variables are scoped to the immediate enclosing block denoted by { } (hence the block scope).

#### Hoisting

While variables declared with var keyword are hoisted (initialized with undefined before the code is run) which means they are accessible in their enclosing scope even before they are declared

#### Creating global object property

At the top level, let, unlike var, does not create a property on the global object

#### Redeclaration

In strict mode, var will let you re-declare the same variable in the same scope while let raises a SyntaxError.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	let y = 200;
	current.work_notes = x + y;

})(current, previous);
```

### arrow functions

How many times have we googled "how to do ____ in JavaScript?" and the top result was a StackOverflow answer that utilized arrow functions? Arrow functions are a compact alternative to traditional function expressions. Combined with other new features, there are so many use-cases for arrow functions (like quickly reordering arrays of objects!).

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	function addDescriptions(x, y){
		return x + '\n' + y;
	}
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	let addDescriptions = (x, y) => x + '\n'+ y; //one line!
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);
```

### for/of

A different kind of for/in to add to your arsenal.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	var work_notes = [];
	for (var inc in incidents){
		work_notes.push(incidents[inc]);
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	let work_notes = [];
	for (let inc of incidents){
		work_notes.push(inc); //note that no index reference is needed
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### map

The Map object holds key-value pairs and remembers the original insertion order of the keys. Any value (both objects and primitive values) may be used as either a key or a value.

Object is similar to Map—both let you set keys to values, retrieve those values, delete keys, and detect whether something is stored at a key. For this reason (and because there were no built-in alternatives), Object has been used as Map historically.

However, there are important differences that make Map preferable in some cases:

- Accidental Keys (objects initialize with prototype)
- Key types (previously just strings or symbols, now can be functions, objects, any primitive)
- Key Order (simplified to order of entry insertion)
- Size (inherent size property)
- Iteration (objects aren't inherently iterable)
- Performance (additions and removals are more performative)
- Serialization and parsing (object wins in this case)

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	const incidents = new Map();

	const keyString = 'a string';
	const keyObj = {};
	const keyFunc = function() {};
	
	inc_gr.next();
	incidents.set(keyString, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyObj, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyFunc, inc_gr.getValue('short_description'));

	let work_notes = [];
	work_notes.push('map size: ' + incidents.size);
	work_notes.push(incidents.get(keyString));
	work_notes.push(incidents.get(keyObj));
	work_notes.push(incidents.get(keyFunc)); //Finding an a value by providing a function!
	work_notes.push(incidents.get('a string'));

	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### set

The Set object lets you store unique values of any type, whether primitive values or object references. Faster, and forces uniqueness of values.

```javascript
const mySet1 = new Set()

mySet1.add(1)           // Set [ 1 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add('some text') // Set [ 1, 5, 'some text' ]
const o = {a: 1, b: 2}
mySet1.add(o)

mySet1.add({a: 1, b: 2})   // o is referencing a different object, so this is okay

mySet1.has(1)              // true
mySet1.has(3)              // false, since 3 has not been added to the set
mySet1.has(5)              // true
mySet1.has(Math.sqrt(25))  // true
mySet1.has('Some Text'.toLowerCase()) // true
mySet1.has(o)       // true

mySet1.size         // 5

mySet1.delete(5)    // removes 5 from the set
mySet1.has(5)       // false, 5 has been removed

mySet1.size         // 4, since we just removed one value

mySet1.add(5)       // Set [1, 'some text', {...}, {...}, 5] - a previously deleted item will be added as a new item, it will not retain its original position before deletion

console.log(mySet1)
// logs Set(5) [ 1, "some text", {…}, {…}, 5 ] in Firefox
// logs Set(5) { 1, "some text", {…}, {…}, 5 } in Chrome
```

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	let incidents = new Set();
	
	while (inc_gr.next()){
		incidents.add(inc_gr.getValue('short_description'));
	}
	
	current.work_notes = incidents.has(inc_gr.getValue('short_description')) + '\n' + incidents.values().next().value + '\n' + incidents.size;
	
})(current, previous);
```

### symbol

Symbol is a built-in object whose constructor returns a symbol primitive — also called a Symbol value or just a Symbol — that's guaranteed to be unique. Symbols are often used to add unique property keys to an object that won't collide with keys any other code might add to the object, and which are hidden from any mechanisms other code will typically use to access the object. That enables a form of weak encapsulation, or a weak form of information hiding.

Every Symbol() call is guaranteed to return a unique Symbol. Every Symbol.for("key") call will always return the same Symbol for a given value of "key". When Symbol.for("key") is called, if a Symbol with the given key can be found in the global Symbol registry, that Symbol is returned. Otherwise, a new Symbol is created, added to the global Symbol registry under the given key, and returned.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var incidents = [];
	let incident = {
		number: current.number,
		short_description: current.short_description
	};
	
	incidents.push(incident);
	incidents.push(incident);
	
	var incidents2 = [];
	incidents2.push(Symbol(incident));
	incidents2.push(Symbol(incident));
	
	current.work_notes = (incidents[0] == incidents[1]) + '\n' + (incidents2[0] == incidents2[1]); //Notice how the first one is true and the second is false, despite all four items being the "same"
	
})(current, previous);
```

### default params

Instead of having to check for included parameters in a function's body, we can do it directly in the parameters now.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	function add (x, y){
		if (y == null) y = 'nothing to see here';
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	function add (x, y = 'nothing to see here'){
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);
```

### spread

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	let incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}

	function sum(x, y, z) {
		return x + '\n' + y + '\n' + z;
	}
	
	const incidents_obj = { ...incidents}; //the array's items are "spread" out as parameters
	
	current.work_notes = sum(...incidents) + '\n' + JSON.stringify(incidents_obj);

})(current, previous);
```

### template strings/literals

I love this one because it makes it so much easier to copy and paste multi-line strings into my code. I use this a lot on AdventOfCode challenges!

```javascript
(function executeRule(current, previous /*null when async*/) {

	let x = `hello
	world
	lchh loves you`;
	
	current.work_notes = x; //goodbye \n

})(current, previous);
```

Another way that these are helpful are for templates (Thanks Chris Helming for the suggestion):

```javascript
(function executeRule(current, previous /*null when async*/) {

	const a = 5; 
	const b = 10; 
	current.work_notes = `Fifteen is ${a + b} and not ${2 * a + b}.`;

})(current, previous);
```

### destructuring

Okay, so destructuring is a LOT more than this but here is just an example.

```javascript
const x = [1, 2, 3, 4, 5];
const [y, z] = x;
// y: 1
// z: 2

const obj = { a: 1, b: 2 };
const { a, b } = obj;
// is equivalent to:
// const a = obj.a;
// const b = obj.b;
```

### class

Hoisting differences (functions and classes are both hoisted and declared but classes are not initialized)

```javascript
class Rectangle {
  constructor(height, width) {
    this.name = 'Rectangle';
    this.height = height;
    this.width = width;
  }
}

class FilledRectangle extends Rectangle {
  constructor(height, width, color) {
    super(height, width);
    this.name = 'Filled rectangle';
    this.color = color;
  }
}
```

### And more

That's not all! Go check it out in the docs!

### ES Sources

- https://betterprogramming.pub/difference-between-regular-functions-and-arrow-functions-f65639aba256
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/
Folder Name:

  - ./ECMASCript 2021
    - ## What?

Prior to the Tokyo Release, ServiceNow's serverside JavaScript utilized ECMAScript 5. "ECMAScript" is basically the version of JavaScript. Newer versions have come out since then (7+ years ago!) and thus, we have been missing out on some helpful functionality.

Client-side scripting is run in your web browser so usually any client script you've made on ServiceNow could utilize the newest JavaScript features, but any script running on the server was limiteded to ES5.

ServiceNow has denoted our version of JavaScript as ECMAScript 2021, which encompasses the feature roll-up of ECMAScript 6 to ECMAScript 12. To see the full documentation of changes, you can see the release notes here: [JavaScript engine feature support](https://docs.servicenow.com/bundle/tokyo-application-development/page/script/JavaScript-engine-upgrade/reference/javascript-engine-feature-support.html). This page has all the new features that are supported, not supported, and disallowed.

## How?

To utilize ECMASCript 2021 on your app, just follow these simple steps:

1. Make sure your instance is upgraded to Tokyo (get a Personal Developer instance [here](https://developer.servicenow.com/))
2. Create a new app via your preferred method (eg. Studio or App Engine Studio)
3. Open the sys_app page for your app<br>![openrecord.png](openrecord.png)
4. Under "Design and Runtime" change "JavaSCript Mode" to `ECMAScript 2021 (ES12)`<br>![javascriptmode.png](javascriptmode.png)
5. Save your record. That's it!

## Looking forward

- The new features are available on scoped apps only for now but we've been told that Global scope support is on the roadmap.
- If you switch existing apps to the new engine, we do recommend that you test for functionality and ensure that existing scripts are running correctly.

## Features!

And here are all the scripts that came from the show. **The scripts are all formatted as if they are running in a `Before Update Business Rule` to demonstrate that it works server side**:

### const

This was actually available previously but would display an error to you when using it, despite allowing you to save. Almost everything else related to ECMAScript 6 and up would not allow you to save your record at all.

`const` is a way to declare and initialize a variable that will never change its value. A great way to ensure a variable that is not meant to change never does (your script will throw an error).

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	const y = 100;
	current.work_notes = x + y;

})(current, previous);
```

### let

What's the difference between `var` and `let`?

#### Scoping rules

The main difference is scoping rules. Variables declared by var keyword are scoped to the immediate function body (hence the function scope) while let variables are scoped to the immediate enclosing block denoted by { } (hence the block scope).

#### Hoisting

While variables declared with var keyword are hoisted (initialized with undefined before the code is run) which means they are accessible in their enclosing scope even before they are declared

#### Creating global object property

At the top level, let, unlike var, does not create a property on the global object

#### Redeclaration

In strict mode, var will let you re-declare the same variable in the same scope while let raises a SyntaxError.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	let y = 200;
	current.work_notes = x + y;

})(current, previous);
```

### arrow functions

How many times have we googled "how to do ____ in JavaScript?" and the top result was a StackOverflow answer that utilized arrow functions? Arrow functions are a compact alternative to traditional function expressions. Combined with other new features, there are so many use-cases for arrow functions (like quickly reordering arrays of objects!).

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	function addDescriptions(x, y){
		return x + '\n' + y;
	}
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	let addDescriptions = (x, y) => x + '\n'+ y; //one line!
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);
```

### for/of

A different kind of for/in to add to your arsenal.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	var work_notes = [];
	for (var inc in incidents){
		work_notes.push(incidents[inc]);
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	let work_notes = [];
	for (let inc of incidents){
		work_notes.push(inc); //note that no index reference is needed
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### map

The Map object holds key-value pairs and remembers the original insertion order of the keys. Any value (both objects and primitive values) may be used as either a key or a value.

Object is similar to Map—both let you set keys to values, retrieve those values, delete keys, and detect whether something is stored at a key. For this reason (and because there were no built-in alternatives), Object has been used as Map historically.

However, there are important differences that make Map preferable in some cases:

- Accidental Keys (objects initialize with prototype)
- Key types (previously just strings or symbols, now can be functions, objects, any primitive)
- Key Order (simplified to order of entry insertion)
- Size (inherent size property)
- Iteration (objects aren't inherently iterable)
- Performance (additions and removals are more performative)
- Serialization and parsing (object wins in this case)

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	const incidents = new Map();

	const keyString = 'a string';
	const keyObj = {};
	const keyFunc = function() {};
	
	inc_gr.next();
	incidents.set(keyString, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyObj, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyFunc, inc_gr.getValue('short_description'));

	let work_notes = [];
	work_notes.push('map size: ' + incidents.size);
	work_notes.push(incidents.get(keyString));
	work_notes.push(incidents.get(keyObj));
	work_notes.push(incidents.get(keyFunc)); //Finding an a value by providing a function!
	work_notes.push(incidents.get('a string'));

	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### set

The Set object lets you store unique values of any type, whether primitive values or object references. Faster, and forces uniqueness of values.

```javascript
const mySet1 = new Set()

mySet1.add(1)           // Set [ 1 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add('some text') // Set [ 1, 5, 'some text' ]
const o = {a: 1, b: 2}
mySet1.add(o)

mySet1.add({a: 1, b: 2})   // o is referencing a different object, so this is okay

mySet1.has(1)              // true
mySet1.has(3)              // false, since 3 has not been added to the set
mySet1.has(5)              // true
mySet1.has(Math.sqrt(25))  // true
mySet1.has('Some Text'.toLowerCase()) // true
mySet1.has(o)       // true

mySet1.size         // 5

mySet1.delete(5)    // removes 5 from the set
mySet1.has(5)       // false, 5 has been removed

mySet1.size         // 4, since we just removed one value

mySet1.add(5)       // Set [1, 'some text', {...}, {...}, 5] - a previously deleted item will be added as a new item, it will not retain its original position before deletion

console.log(mySet1)
// logs Set(5) [ 1, "some text", {…}, {…}, 5 ] in Firefox
// logs Set(5) { 1, "some text", {…}, {…}, 5 } in Chrome
```

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	let incidents = new Set();
	
	while (inc_gr.next()){
		incidents.add(inc_gr.getValue('short_description'));
	}
	
	current.work_notes = incidents.has(inc_gr.getValue('short_description')) + '\n' + incidents.values().next().value + '\n' + incidents.size;
	
})(current, previous);
```

### symbol

Symbol is a built-in object whose constructor returns a symbol primitive — also called a Symbol value or just a Symbol — that's guaranteed to be unique. Symbols are often used to add unique property keys to an object that won't collide with keys any other code might add to the object, and which are hidden from any mechanisms other code will typically use to access the object. That enables a form of weak encapsulation, or a weak form of information hiding.

Every Symbol() call is guaranteed to return a unique Symbol. Every Symbol.for("key") call will always return the same Symbol for a given value of "key". When Symbol.for("key") is called, if a Symbol with the given key can be found in the global Symbol registry, that Symbol is returned. Otherwise, a new Symbol is created, added to the global Symbol registry under the given key, and returned.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var incidents = [];
	let incident = {
		number: current.number,
		short_description: current.short_description
	};
	
	incidents.push(incident);
	incidents.push(incident);
	
	var incidents2 = [];
	incidents2.push(Symbol(incident));
	incidents2.push(Symbol(incident));
	
	current.work_notes = (incidents[0] == incidents[1]) + '\n' + (incidents2[0] == incidents2[1]); //Notice how the first one is true and the second is false, despite all four items being the "same"
	
})(current, previous);
```

### default params

Instead of having to check for included parameters in a function's body, we can do it directly in the parameters now.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	function add (x, y){
		if (y == null) y = 'nothing to see here';
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	function add (x, y = 'nothing to see here'){
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);
```

### spread

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	let incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}

	function sum(x, y, z) {
		return x + '\n' + y + '\n' + z;
	}
	
	const incidents_obj = { ...incidents}; //the array's items are "spread" out as parameters
	
	current.work_notes = sum(...incidents) + '\n' + JSON.stringify(incidents_obj);

})(current, previous);
```

### template strings/literals

I love this one because it makes it so much easier to copy and paste multi-line strings into my code. I use this a lot on AdventOfCode challenges!

```javascript
(function executeRule(current, previous /*null when async*/) {

	let x = `hello
	world
	lchh loves you`;
	
	current.work_notes = x; //goodbye \n

})(current, previous);
```

Another way that these are helpful are for templates (Thanks Chris Helming for the suggestion):

```javascript
(function executeRule(current, previous /*null when async*/) {

	const a = 5; 
	const b = 10; 
	current.work_notes = `Fifteen is ${a + b} and not ${2 * a + b}.`;

})(current, previous);
```

### destructuring

Okay, so destructuring is a LOT more than this but here is just an example.

```javascript
const x = [1, 2, 3, 4, 5];
const [y, z] = x;
// y: 1
// z: 2

const obj = { a: 1, b: 2 };
const { a, b } = obj;
// is equivalent to:
// const a = obj.a;
// const b = obj.b;
```

### class

Hoisting differences (functions and classes are both hoisted and declared but classes are not initialized)

```javascript
class Rectangle {
  constructor(height, width) {
    this.name = 'Rectangle';
    this.height = height;
    this.width = width;
  }
}

class FilledRectangle extends Rectangle {
  constructor(height, width, color) {
    super(height, width);
    this.name = 'Filled rectangle';
    this.color = color;
  }
}
```

### And more

That's not all! Go check it out in the docs!

### ES Sources

- https://betterprogramming.pub/difference-between-regular-functions-and-arrow-functions-f65639aba256
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/
Folder Name:

  - ./ECMASCript 2021
    - ## What?

Prior to the Tokyo Release, ServiceNow's serverside JavaScript utilized ECMAScript 5. "ECMAScript" is basically the version of JavaScript. Newer versions have come out since then (7+ years ago!) and thus, we have been missing out on some helpful functionality.

Client-side scripting is run in your web browser so usually any client script you've made on ServiceNow could utilize the newest JavaScript features, but any script running on the server was limiteded to ES5.

ServiceNow has denoted our version of JavaScript as ECMAScript 2021, which encompasses the feature roll-up of ECMAScript 6 to ECMAScript 12. To see the full documentation of changes, you can see the release notes here: [JavaScript engine feature support](https://docs.servicenow.com/bundle/tokyo-application-development/page/script/JavaScript-engine-upgrade/reference/javascript-engine-feature-support.html). This page has all the new features that are supported, not supported, and disallowed.

## How?

To utilize ECMASCript 2021 on your app, just follow these simple steps:

1. Make sure your instance is upgraded to Tokyo (get a Personal Developer instance [here](https://developer.servicenow.com/))
2. Create a new app via your preferred method (eg. Studio or App Engine Studio)
3. Open the sys_app page for your app<br>![openrecord.png](openrecord.png)
4. Under "Design and Runtime" change "JavaSCript Mode" to `ECMAScript 2021 (ES12)`<br>![javascriptmode.png](javascriptmode.png)
5. Save your record. That's it!

## Looking forward

- The new features are available on scoped apps only for now but we've been told that Global scope support is on the roadmap.
- If you switch existing apps to the new engine, we do recommend that you test for functionality and ensure that existing scripts are running correctly.

## Features!

And here are all the scripts that came from the show. **The scripts are all formatted as if they are running in a `Before Update Business Rule` to demonstrate that it works server side**:

### const

This was actually available previously but would display an error to you when using it, despite allowing you to save. Almost everything else related to ECMAScript 6 and up would not allow you to save your record at all.

`const` is a way to declare and initialize a variable that will never change its value. A great way to ensure a variable that is not meant to change never does (your script will throw an error).

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	const y = 100;
	current.work_notes = x + y;

})(current, previous);
```

### let

What's the difference between `var` and `let`?

#### Scoping rules

The main difference is scoping rules. Variables declared by var keyword are scoped to the immediate function body (hence the function scope) while let variables are scoped to the immediate enclosing block denoted by { } (hence the block scope).

#### Hoisting

While variables declared with var keyword are hoisted (initialized with undefined before the code is run) which means they are accessible in their enclosing scope even before they are declared

#### Creating global object property

At the top level, let, unlike var, does not create a property on the global object

#### Redeclaration

In strict mode, var will let you re-declare the same variable in the same scope while let raises a SyntaxError.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	let y = 200;
	current.work_notes = x + y;

})(current, previous);
```

### arrow functions

How many times have we googled "how to do ____ in JavaScript?" and the top result was a StackOverflow answer that utilized arrow functions? Arrow functions are a compact alternative to traditional function expressions. Combined with other new features, there are so many use-cases for arrow functions (like quickly reordering arrays of objects!).

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	function addDescriptions(x, y){
		return x + '\n' + y;
	}
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	let addDescriptions = (x, y) => x + '\n'+ y; //one line!
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);
```

### for/of

A different kind of for/in to add to your arsenal.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	var work_notes = [];
	for (var inc in incidents){
		work_notes.push(incidents[inc]);
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	let work_notes = [];
	for (let inc of incidents){
		work_notes.push(inc); //note that no index reference is needed
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### map

The Map object holds key-value pairs and remembers the original insertion order of the keys. Any value (both objects and primitive values) may be used as either a key or a value.

Object is similar to Map—both let you set keys to values, retrieve those values, delete keys, and detect whether something is stored at a key. For this reason (and because there were no built-in alternatives), Object has been used as Map historically.

However, there are important differences that make Map preferable in some cases:

- Accidental Keys (objects initialize with prototype)
- Key types (previously just strings or symbols, now can be functions, objects, any primitive)
- Key Order (simplified to order of entry insertion)
- Size (inherent size property)
- Iteration (objects aren't inherently iterable)
- Performance (additions and removals are more performative)
- Serialization and parsing (object wins in this case)

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	const incidents = new Map();

	const keyString = 'a string';
	const keyObj = {};
	const keyFunc = function() {};
	
	inc_gr.next();
	incidents.set(keyString, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyObj, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyFunc, inc_gr.getValue('short_description'));

	let work_notes = [];
	work_notes.push('map size: ' + incidents.size);
	work_notes.push(incidents.get(keyString));
	work_notes.push(incidents.get(keyObj));
	work_notes.push(incidents.get(keyFunc)); //Finding an a value by providing a function!
	work_notes.push(incidents.get('a string'));

	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### set

The Set object lets you store unique values of any type, whether primitive values or object references. Faster, and forces uniqueness of values.

```javascript
const mySet1 = new Set()

mySet1.add(1)           // Set [ 1 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add('some text') // Set [ 1, 5, 'some text' ]
const o = {a: 1, b: 2}
mySet1.add(o)

mySet1.add({a: 1, b: 2})   // o is referencing a different object, so this is okay

mySet1.has(1)              // true
mySet1.has(3)              // false, since 3 has not been added to the set
mySet1.has(5)              // true
mySet1.has(Math.sqrt(25))  // true
mySet1.has('Some Text'.toLowerCase()) // true
mySet1.has(o)       // true

mySet1.size         // 5

mySet1.delete(5)    // removes 5 from the set
mySet1.has(5)       // false, 5 has been removed

mySet1.size         // 4, since we just removed one value

mySet1.add(5)       // Set [1, 'some text', {...}, {...}, 5] - a previously deleted item will be added as a new item, it will not retain its original position before deletion

console.log(mySet1)
// logs Set(5) [ 1, "some text", {…}, {…}, 5 ] in Firefox
// logs Set(5) { 1, "some text", {…}, {…}, 5 } in Chrome
```

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	let incidents = new Set();
	
	while (inc_gr.next()){
		incidents.add(inc_gr.getValue('short_description'));
	}
	
	current.work_notes = incidents.has(inc_gr.getValue('short_description')) + '\n' + incidents.values().next().value + '\n' + incidents.size;
	
})(current, previous);
```

### symbol

Symbol is a built-in object whose constructor returns a symbol primitive — also called a Symbol value or just a Symbol — that's guaranteed to be unique. Symbols are often used to add unique property keys to an object that won't collide with keys any other code might add to the object, and which are hidden from any mechanisms other code will typically use to access the object. That enables a form of weak encapsulation, or a weak form of information hiding.

Every Symbol() call is guaranteed to return a unique Symbol. Every Symbol.for("key") call will always return the same Symbol for a given value of "key". When Symbol.for("key") is called, if a Symbol with the given key can be found in the global Symbol registry, that Symbol is returned. Otherwise, a new Symbol is created, added to the global Symbol registry under the given key, and returned.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var incidents = [];
	let incident = {
		number: current.number,
		short_description: current.short_description
	};
	
	incidents.push(incident);
	incidents.push(incident);
	
	var incidents2 = [];
	incidents2.push(Symbol(incident));
	incidents2.push(Symbol(incident));
	
	current.work_notes = (incidents[0] == incidents[1]) + '\n' + (incidents2[0] == incidents2[1]); //Notice how the first one is true and the second is false, despite all four items being the "same"
	
})(current, previous);
```

### default params

Instead of having to check for included parameters in a function's body, we can do it directly in the parameters now.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	function add (x, y){
		if (y == null) y = 'nothing to see here';
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	function add (x, y = 'nothing to see here'){
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);
```

### spread

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	let incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}

	function sum(x, y, z) {
		return x + '\n' + y + '\n' + z;
	}
	
	const incidents_obj = { ...incidents}; //the array's items are "spread" out as parameters
	
	current.work_notes = sum(...incidents) + '\n' + JSON.stringify(incidents_obj);

})(current, previous);
```

### template strings/literals

I love this one because it makes it so much easier to copy and paste multi-line strings into my code. I use this a lot on AdventOfCode challenges!

```javascript
(function executeRule(current, previous /*null when async*/) {

	let x = `hello
	world
	lchh loves you`;
	
	current.work_notes = x; //goodbye \n

})(current, previous);
```

Another way that these are helpful are for templates (Thanks Chris Helming for the suggestion):

```javascript
(function executeRule(current, previous /*null when async*/) {

	const a = 5; 
	const b = 10; 
	current.work_notes = `Fifteen is ${a + b} and not ${2 * a + b}.`;

})(current, previous);
```

### destructuring

Okay, so destructuring is a LOT more than this but here is just an example.

```javascript
const x = [1, 2, 3, 4, 5];
const [y, z] = x;
// y: 1
// z: 2

const obj = { a: 1, b: 2 };
const { a, b } = obj;
// is equivalent to:
// const a = obj.a;
// const b = obj.b;
```

### class

Hoisting differences (functions and classes are both hoisted and declared but classes are not initialized)

```javascript
class Rectangle {
  constructor(height, width) {
    this.name = 'Rectangle';
    this.height = height;
    this.width = width;
  }
}

class FilledRectangle extends Rectangle {
  constructor(height, width, color) {
    super(height, width);
    this.name = 'Filled rectangle';
    this.color = color;
  }
}
```

### And more

That's not all! Go check it out in the docs!

### ES Sources

- https://betterprogramming.pub/difference-between-regular-functions-and-arrow-functions-f65639aba256
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/
Folder Name:

  - ./ECMASCript 2021
    - ## What?

Prior to the Tokyo Release, ServiceNow's serverside JavaScript utilized ECMAScript 5. "ECMAScript" is basically the version of JavaScript. Newer versions have come out since then (7+ years ago!) and thus, we have been missing out on some helpful functionality.

Client-side scripting is run in your web browser so usually any client script you've made on ServiceNow could utilize the newest JavaScript features, but any script running on the server was limiteded to ES5.

ServiceNow has denoted our version of JavaScript as ECMAScript 2021, which encompasses the feature roll-up of ECMAScript 6 to ECMAScript 12. To see the full documentation of changes, you can see the release notes here: [JavaScript engine feature support](https://docs.servicenow.com/bundle/tokyo-application-development/page/script/JavaScript-engine-upgrade/reference/javascript-engine-feature-support.html). This page has all the new features that are supported, not supported, and disallowed.

## How?

To utilize ECMASCript 2021 on your app, just follow these simple steps:

1. Make sure your instance is upgraded to Tokyo (get a Personal Developer instance [here](https://developer.servicenow.com/))
2. Create a new app via your preferred method (eg. Studio or App Engine Studio)
3. Open the sys_app page for your app<br>![openrecord.png](openrecord.png)
4. Under "Design and Runtime" change "JavaSCript Mode" to `ECMAScript 2021 (ES12)`<br>![javascriptmode.png](javascriptmode.png)
5. Save your record. That's it!

## Looking forward

- The new features are available on scoped apps only for now but we've been told that Global scope support is on the roadmap.
- If you switch existing apps to the new engine, we do recommend that you test for functionality and ensure that existing scripts are running correctly.

## Features!

And here are all the scripts that came from the show. **The scripts are all formatted as if they are running in a `Before Update Business Rule` to demonstrate that it works server side**:

### const

This was actually available previously but would display an error to you when using it, despite allowing you to save. Almost everything else related to ECMAScript 6 and up would not allow you to save your record at all.

`const` is a way to declare and initialize a variable that will never change its value. A great way to ensure a variable that is not meant to change never does (your script will throw an error).

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	const y = 100;
	current.work_notes = x + y;

})(current, previous);
```

### let

What's the difference between `var` and `let`?

#### Scoping rules

The main difference is scoping rules. Variables declared by var keyword are scoped to the immediate function body (hence the function scope) while let variables are scoped to the immediate enclosing block denoted by { } (hence the block scope).

#### Hoisting

While variables declared with var keyword are hoisted (initialized with undefined before the code is run) which means they are accessible in their enclosing scope even before they are declared

#### Creating global object property

At the top level, let, unlike var, does not create a property on the global object

#### Redeclaration

In strict mode, var will let you re-declare the same variable in the same scope while let raises a SyntaxError.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	let y = 200;
	current.work_notes = x + y;

})(current, previous);
```

### arrow functions

How many times have we googled "how to do ____ in JavaScript?" and the top result was a StackOverflow answer that utilized arrow functions? Arrow functions are a compact alternative to traditional function expressions. Combined with other new features, there are so many use-cases for arrow functions (like quickly reordering arrays of objects!).

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	function addDescriptions(x, y){
		return x + '\n' + y;
	}
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	let addDescriptions = (x, y) => x + '\n'+ y; //one line!
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);
```

### for/of

A different kind of for/in to add to your arsenal.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	var work_notes = [];
	for (var inc in incidents){
		work_notes.push(incidents[inc]);
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	let work_notes = [];
	for (let inc of incidents){
		work_notes.push(inc); //note that no index reference is needed
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### map

The Map object holds key-value pairs and remembers the original insertion order of the keys. Any value (both objects and primitive values) may be used as either a key or a value.

Object is similar to Map—both let you set keys to values, retrieve those values, delete keys, and detect whether something is stored at a key. For this reason (and because there were no built-in alternatives), Object has been used as Map historically.

However, there are important differences that make Map preferable in some cases:

- Accidental Keys (objects initialize with prototype)
- Key types (previously just strings or symbols, now can be functions, objects, any primitive)
- Key Order (simplified to order of entry insertion)
- Size (inherent size property)
- Iteration (objects aren't inherently iterable)
- Performance (additions and removals are more performative)
- Serialization and parsing (object wins in this case)

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	const incidents = new Map();

	const keyString = 'a string';
	const keyObj = {};
	const keyFunc = function() {};
	
	inc_gr.next();
	incidents.set(keyString, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyObj, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyFunc, inc_gr.getValue('short_description'));

	let work_notes = [];
	work_notes.push('map size: ' + incidents.size);
	work_notes.push(incidents.get(keyString));
	work_notes.push(incidents.get(keyObj));
	work_notes.push(incidents.get(keyFunc)); //Finding an a value by providing a function!
	work_notes.push(incidents.get('a string'));

	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### set

The Set object lets you store unique values of any type, whether primitive values or object references. Faster, and forces uniqueness of values.

```javascript
const mySet1 = new Set()

mySet1.add(1)           // Set [ 1 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add('some text') // Set [ 1, 5, 'some text' ]
const o = {a: 1, b: 2}
mySet1.add(o)

mySet1.add({a: 1, b: 2})   // o is referencing a different object, so this is okay

mySet1.has(1)              // true
mySet1.has(3)              // false, since 3 has not been added to the set
mySet1.has(5)              // true
mySet1.has(Math.sqrt(25))  // true
mySet1.has('Some Text'.toLowerCase()) // true
mySet1.has(o)       // true

mySet1.size         // 5

mySet1.delete(5)    // removes 5 from the set
mySet1.has(5)       // false, 5 has been removed

mySet1.size         // 4, since we just removed one value

mySet1.add(5)       // Set [1, 'some text', {...}, {...}, 5] - a previously deleted item will be added as a new item, it will not retain its original position before deletion

console.log(mySet1)
// logs Set(5) [ 1, "some text", {…}, {…}, 5 ] in Firefox
// logs Set(5) { 1, "some text", {…}, {…}, 5 } in Chrome
```

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	let incidents = new Set();
	
	while (inc_gr.next()){
		incidents.add(inc_gr.getValue('short_description'));
	}
	
	current.work_notes = incidents.has(inc_gr.getValue('short_description')) + '\n' + incidents.values().next().value + '\n' + incidents.size;
	
})(current, previous);
```

### symbol

Symbol is a built-in object whose constructor returns a symbol primitive — also called a Symbol value or just a Symbol — that's guaranteed to be unique. Symbols are often used to add unique property keys to an object that won't collide with keys any other code might add to the object, and which are hidden from any mechanisms other code will typically use to access the object. That enables a form of weak encapsulation, or a weak form of information hiding.

Every Symbol() call is guaranteed to return a unique Symbol. Every Symbol.for("key") call will always return the same Symbol for a given value of "key". When Symbol.for("key") is called, if a Symbol with the given key can be found in the global Symbol registry, that Symbol is returned. Otherwise, a new Symbol is created, added to the global Symbol registry under the given key, and returned.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var incidents = [];
	let incident = {
		number: current.number,
		short_description: current.short_description
	};
	
	incidents.push(incident);
	incidents.push(incident);
	
	var incidents2 = [];
	incidents2.push(Symbol(incident));
	incidents2.push(Symbol(incident));
	
	current.work_notes = (incidents[0] == incidents[1]) + '\n' + (incidents2[0] == incidents2[1]); //Notice how the first one is true and the second is false, despite all four items being the "same"
	
})(current, previous);
```

### default params

Instead of having to check for included parameters in a function's body, we can do it directly in the parameters now.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	function add (x, y){
		if (y == null) y = 'nothing to see here';
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	function add (x, y = 'nothing to see here'){
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);
```

### spread

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	let incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}

	function sum(x, y, z) {
		return x + '\n' + y + '\n' + z;
	}
	
	const incidents_obj = { ...incidents}; //the array's items are "spread" out as parameters
	
	current.work_notes = sum(...incidents) + '\n' + JSON.stringify(incidents_obj);

})(current, previous);
```

### template strings/literals

I love this one because it makes it so much easier to copy and paste multi-line strings into my code. I use this a lot on AdventOfCode challenges!

```javascript
(function executeRule(current, previous /*null when async*/) {

	let x = `hello
	world
	lchh loves you`;
	
	current.work_notes = x; //goodbye \n

})(current, previous);
```

Another way that these are helpful are for templates (Thanks Chris Helming for the suggestion):

```javascript
(function executeRule(current, previous /*null when async*/) {

	const a = 5; 
	const b = 10; 
	current.work_notes = `Fifteen is ${a + b} and not ${2 * a + b}.`;

})(current, previous);
```

### destructuring

Okay, so destructuring is a LOT more than this but here is just an example.

```javascript
const x = [1, 2, 3, 4, 5];
const [y, z] = x;
// y: 1
// z: 2

const obj = { a: 1, b: 2 };
const { a, b } = obj;
// is equivalent to:
// const a = obj.a;
// const b = obj.b;
```

### class

Hoisting differences (functions and classes are both hoisted and declared but classes are not initialized)

```javascript
class Rectangle {
  constructor(height, width) {
    this.name = 'Rectangle';
    this.height = height;
    this.width = width;
  }
}

class FilledRectangle extends Rectangle {
  constructor(height, width, color) {
    super(height, width);
    this.name = 'Filled rectangle';
    this.color = color;
  }
}
```

### And more

That's not all! Go check it out in the docs!

### ES Sources

- https://betterprogramming.pub/difference-between-regular-functions-and-arrow-functions-f65639aba256
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/
Folder Name:

  - ./ECMASCript 2021
    - ## What?

Prior to the Tokyo Release, ServiceNow's serverside JavaScript utilized ECMAScript 5. "ECMAScript" is basically the version of JavaScript. Newer versions have come out since then (7+ years ago!) and thus, we have been missing out on some helpful functionality.

Client-side scripting is run in your web browser so usually any client script you've made on ServiceNow could utilize the newest JavaScript features, but any script running on the server was limiteded to ES5.

ServiceNow has denoted our version of JavaScript as ECMAScript 2021, which encompasses the feature roll-up of ECMAScript 6 to ECMAScript 12. To see the full documentation of changes, you can see the release notes here: [JavaScript engine feature support](https://docs.servicenow.com/bundle/tokyo-application-development/page/script/JavaScript-engine-upgrade/reference/javascript-engine-feature-support.html). This page has all the new features that are supported, not supported, and disallowed.

## How?

To utilize ECMASCript 2021 on your app, just follow these simple steps:

1. Make sure your instance is upgraded to Tokyo (get a Personal Developer instance [here](https://developer.servicenow.com/))
2. Create a new app via your preferred method (eg. Studio or App Engine Studio)
3. Open the sys_app page for your app<br>![openrecord.png](openrecord.png)
4. Under "Design and Runtime" change "JavaSCript Mode" to `ECMAScript 2021 (ES12)`<br>![javascriptmode.png](javascriptmode.png)
5. Save your record. That's it!

## Looking forward

- The new features are available on scoped apps only for now but we've been told that Global scope support is on the roadmap.
- If you switch existing apps to the new engine, we do recommend that you test for functionality and ensure that existing scripts are running correctly.

## Features!

And here are all the scripts that came from the show. **The scripts are all formatted as if they are running in a `Before Update Business Rule` to demonstrate that it works server side**:

### const

This was actually available previously but would display an error to you when using it, despite allowing you to save. Almost everything else related to ECMAScript 6 and up would not allow you to save your record at all.

`const` is a way to declare and initialize a variable that will never change its value. A great way to ensure a variable that is not meant to change never does (your script will throw an error).

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	const y = 100;
	current.work_notes = x + y;

})(current, previous);
```

### let

What's the difference between `var` and `let`?

#### Scoping rules

The main difference is scoping rules. Variables declared by var keyword are scoped to the immediate function body (hence the function scope) while let variables are scoped to the immediate enclosing block denoted by { } (hence the block scope).

#### Hoisting

While variables declared with var keyword are hoisted (initialized with undefined before the code is run) which means they are accessible in their enclosing scope even before they are declared

#### Creating global object property

At the top level, let, unlike var, does not create a property on the global object

#### Redeclaration

In strict mode, var will let you re-declare the same variable in the same scope while let raises a SyntaxError.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.query();
	var x = inc_gr.getRowCount();
	
	let y = 200;
	current.work_notes = x + y;

})(current, previous);
```

### arrow functions

How many times have we googled "how to do ____ in JavaScript?" and the top result was a StackOverflow answer that utilized arrow functions? Arrow functions are a compact alternative to traditional function expressions. Combined with other new features, there are so many use-cases for arrow functions (like quickly reordering arrays of objects!).

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	function addDescriptions(x, y){
		return x + '\n' + y;
	}
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var sd = current.short_description;
	var d = current.description;
	
	let addDescriptions = (x, y) => x + '\n'+ y; //one line!
	
	current.work_notes = addDescriptions(sd, d);
	
})(current, previous);
```

### for/of

A different kind of for/in to add to your arsenal.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	var work_notes = [];
	for (var inc in incidents){
		work_notes.push(incidents[inc]);
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(10);
	inc_gr.query();
	var incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}
	let work_notes = [];
	for (let inc of incidents){
		work_notes.push(inc); //note that no index reference is needed
	}
	
	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### map

The Map object holds key-value pairs and remembers the original insertion order of the keys. Any value (both objects and primitive values) may be used as either a key or a value.

Object is similar to Map—both let you set keys to values, retrieve those values, delete keys, and detect whether something is stored at a key. For this reason (and because there were no built-in alternatives), Object has been used as Map historically.

However, there are important differences that make Map preferable in some cases:

- Accidental Keys (objects initialize with prototype)
- Key types (previously just strings or symbols, now can be functions, objects, any primitive)
- Key Order (simplified to order of entry insertion)
- Size (inherent size property)
- Iteration (objects aren't inherently iterable)
- Performance (additions and removals are more performative)
- Serialization and parsing (object wins in this case)

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	const incidents = new Map();

	const keyString = 'a string';
	const keyObj = {};
	const keyFunc = function() {};
	
	inc_gr.next();
	incidents.set(keyString, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyObj, inc_gr.getValue('short_description'));
	
	inc_gr.next();
	incidents.set(keyFunc, inc_gr.getValue('short_description'));

	let work_notes = [];
	work_notes.push('map size: ' + incidents.size);
	work_notes.push(incidents.get(keyString));
	work_notes.push(incidents.get(keyObj));
	work_notes.push(incidents.get(keyFunc)); //Finding an a value by providing a function!
	work_notes.push(incidents.get('a string'));

	current.work_notes = work_notes.join('\n');
	
})(current, previous);
```

### set

The Set object lets you store unique values of any type, whether primitive values or object references. Faster, and forces uniqueness of values.

```javascript
const mySet1 = new Set()

mySet1.add(1)           // Set [ 1 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add(5)           // Set [ 1, 5 ]
mySet1.add('some text') // Set [ 1, 5, 'some text' ]
const o = {a: 1, b: 2}
mySet1.add(o)

mySet1.add({a: 1, b: 2})   // o is referencing a different object, so this is okay

mySet1.has(1)              // true
mySet1.has(3)              // false, since 3 has not been added to the set
mySet1.has(5)              // true
mySet1.has(Math.sqrt(25))  // true
mySet1.has('Some Text'.toLowerCase()) // true
mySet1.has(o)       // true

mySet1.size         // 5

mySet1.delete(5)    // removes 5 from the set
mySet1.has(5)       // false, 5 has been removed

mySet1.size         // 4, since we just removed one value

mySet1.add(5)       // Set [1, 'some text', {...}, {...}, 5] - a previously deleted item will be added as a new item, it will not retain its original position before deletion

console.log(mySet1)
// logs Set(5) [ 1, "some text", {…}, {…}, 5 ] in Firefox
// logs Set(5) { 1, "some text", {…}, {…}, 5 } in Chrome
```

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	
	let incidents = new Set();
	
	while (inc_gr.next()){
		incidents.add(inc_gr.getValue('short_description'));
	}
	
	current.work_notes = incidents.has(inc_gr.getValue('short_description')) + '\n' + incidents.values().next().value + '\n' + incidents.size;
	
})(current, previous);
```

### symbol

Symbol is a built-in object whose constructor returns a symbol primitive — also called a Symbol value or just a Symbol — that's guaranteed to be unique. Symbols are often used to add unique property keys to an object that won't collide with keys any other code might add to the object, and which are hidden from any mechanisms other code will typically use to access the object. That enables a form of weak encapsulation, or a weak form of information hiding.

Every Symbol() call is guaranteed to return a unique Symbol. Every Symbol.for("key") call will always return the same Symbol for a given value of "key". When Symbol.for("key") is called, if a Symbol with the given key can be found in the global Symbol registry, that Symbol is returned. Otherwise, a new Symbol is created, added to the global Symbol registry under the given key, and returned.

```javascript
(function executeRule(current, previous /*null when async*/) {

	var incidents = [];
	let incident = {
		number: current.number,
		short_description: current.short_description
	};
	
	incidents.push(incident);
	incidents.push(incident);
	
	var incidents2 = [];
	incidents2.push(Symbol(incident));
	incidents2.push(Symbol(incident));
	
	current.work_notes = (incidents[0] == incidents[1]) + '\n' + (incidents2[0] == incidents2[1]); //Notice how the first one is true and the second is false, despite all four items being the "same"
	
})(current, previous);
```

### default params

Instead of having to check for included parameters in a function's body, we can do it directly in the parameters now.

```javascript
//before
(function executeRule(current, previous /*null when async*/) {

	function add (x, y){
		if (y == null) y = 'nothing to see here';
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);

//after
(function executeRule(current, previous /*null when async*/) {

	function add (x, y = 'nothing to see here'){
		return x + '\n' + y;
	}
	
	current.work_notes = add(current.short_description);
	
})(current, previous);
```

### spread

```javascript
(function executeRule(current, previous /*null when async*/) {

	var inc_gr = new GlideRecord('incident');
	inc_gr.orderByDesc('number');
	inc_gr.setLimit(3);
	inc_gr.query();
	let incidents = [];
	while (inc_gr.next()){
		incidents.push(inc_gr.getValue('short_description'));
	}

	function sum(x, y, z) {
		return x + '\n' + y + '\n' + z;
	}
	
	const incidents_obj = { ...incidents}; //the array's items are "spread" out as parameters
	
	current.work_notes = sum(...incidents) + '\n' + JSON.stringify(incidents_obj);

})(current, previous);
```

### template strings/literals

I love this one because it makes it so much easier to copy and paste multi-line strings into my code. I use this a lot on AdventOfCode challenges!

```javascript
(function executeRule(current, previous /*null when async*/) {

	let x = `hello
	world
	lchh loves you`;
	
	current.work_notes = x; //goodbye \n

})(current, previous);
```

Another way that these are helpful are for templates (Thanks Chris Helming for the suggestion):

```javascript
(function executeRule(current, previous /*null when async*/) {

	const a = 5; 
	const b = 10; 
	current.work_notes = `Fifteen is ${a + b} and not ${2 * a + b}.`;

})(current, previous);
```

### destructuring

Okay, so destructuring is a LOT more than this but here is just an example.

```javascript
const x = [1, 2, 3, 4, 5];
const [y, z] = x;
// y: 1
// z: 2

const obj = { a: 1, b: 2 };
const { a, b } = obj;
// is equivalent to:
// const a = obj.a;
// const b = obj.b;
```

### class

Hoisting differences (functions and classes are both hoisted and declared but classes are not initialized)

```javascript
class Rectangle {
  constructor(height, width) {
    this.name = 'Rectangle';
    this.height = height;
    this.width = width;
  }
}

class FilledRectangle extends Rectangle {
  constructor(height, width, color) {
    super(height, width);
    this.name = 'Filled rectangle';
    this.color = color;
  }
}
```

### And more

That's not all! Go check it out in the docs!

### ES Sources

- https://betterprogramming.pub/difference-between-regular-functions-and-arrow-functions-f65639aba256
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/
Folder Name:

  - ./UI Scripts/Make OOB Attachment Mandatory
    - # Make out of the box attahcment mandatory onChange of a field in Catalog Item

This scripts makes the out of the box attachments to mandatory on the Service Portal for any Catalog Item.

Usage:

Step #1 - Create the UI Script 
* [Click here for script](setAttachmentMandatory.js)

Step #2 - Include the UI Script in the Portal Theme under JS Includes

Step #3 - Create a Catalog Client Script for the respective Catalog Item where you want to make the OOB attachment mandatory for certain criteria
Folder Name:

  - ./UI Scripts/Restrict URL Hack using UI script
    - 1.Go to System UI >UI Scripts >Create a new UI script and Check the Global field.
2.Below is an example 

Lets say the Original URL opened is:

https://devXXXXX.service-now.com/sys_security_acl.do?sys_id=-1&sys_is_list=true&sys_target=sys_security_acl&sysparm_checked_items=&sysparm_fixed_query=&sysparm_group_sort=&sysparm_list_css=&sysparm_query=name%3dincident%5eoperation%3dread

and we need to monitor "sysparm_fixed_query" parameter in the URL.


![image](https://user-images.githubusercontent.com/42912180/195846361-d51f40ba-cdc0-40e1-8057-b19a0906a9a8.png)
Folder Name:

  - ./UI Scripts/Display number of created records
    - # Display number of created records

Use case / Requirement : When trying to create a new record in a table, Display a message showing number of records already created by him/her in that table.

Solution : Created a UI script to display number of records and call that UI script from an onLoad client script.
Folder Name:

  - ./UI Scripts/Display number of created records
    - # Display number of created records

Use case / Requirement : When trying to create a new record in a table, Display a message showing number of records already created by him/her in that table.

Solution : Created a UI script to display number of records and call that UI script from an onLoad client script.
Folder Name:

  - ./GlideQuery/Get User's Roles from User Name
    - # Get User's Roles from User Name

GlideQuery's can greatly simplify extracting information from queries, especially when dot walking.

This query retrieves a user's roles, and returns an array of objects with the the role's display
value, the role's active status, the user's display value, and the user's email.  Adding more
fields is trivial with this format, and the query stream is very easy to follow.
Folder Name:

  - ./GlideQuery/FlatMap to Nest New Queries
    - # Using FlatMap to Nest Queries

`flatMap` returns a Stream to a parent stream, that cause the parent stream to return the result of the nested Stream.  It is extremely useful for using the results of a query to create and return the results of a new query based on the original's results.

The provided example is slightly contrived, but exhibits this behavior of using the results of a query on one table to create a query on a second table, and then view the output.

It finds uses the `sys_user` table to find the `sys_id` for username = david.miller, then queries the incident table for incidents where the `caller_id` is David Miller's sys_id (from the first query).  The output is the result of the inner query.
Folder Name:

  - ./GlideQuery/Nested WHERE orWHERE GlideQueries
    - # WHERE Clauses with Nested GlideQueries

Creating a query with multiple groupings of AND and OR statements would be impossible to decipher,
so `GlideQuery` forbids them.

An example of this would be the following, where the query system would be unable to tell if this
should be 

`WHERE (caller_id is david.miller AND state is 1) OR (caller_id is beth.anglin)` 

versus

`WHERE (caller_id is david.miller) AND (state is 1 OR caller_id is beth.anglin)` 

```javascript
secondQuery = new GlideQuery('task')
	.where('caller_id.user_name', 'david.miller')
	.where('state', 1)
	.orWhere('caller_id.user_name', 'beth.anglin')
	.select(['sys_id'])
	.toArray(10);
```

Instead, using the equivalent nested GlideQuery in the JavaScript file shows the proper way of nesting
OR WHERE queries.
Folder Name:

  - ./GlideQuery/Remote Table
    - 
Folder Name:

  - ./GlideQuery/Basic Wrappers
    - # GlideQuery

GlideQuery is a wrapper for the GlideRecord and GlideAggregate APIs. The wrapper offers several advantages, including a single point of entry, fail-fast with friendly error messaging, native JavaScript syntax, and more. Here are some functions that implement the basic GlideQuery capabilities to help you get started.

[Product Documentation](https://docs.servicenow.com/bundle/tokyo-application-development/page/app-store/dev_portal/API_reference/GlideQuery/concept/GlideQueryGlobalAPI.html)

[ServiceNow Community Blog Entries](https://developer.servicenow.com/blog.do?p=/tags/glidequery/) 
[Streyda Article](https://www.streyda.eu/post/gliderecordorglidequery)


## Get Records
```javascript
function getRecords( tableName, query, fields ){
	/* Given a table name, encoded query, and array of field names,
	 * Gather the request field attributes of the queried records,
	 * Build an array of JSON objects and return the array.
	 */
	 	
	return new global.GlideQuery.parse( tableName, query )
	.select( fields )
	.reduce( function( arr, rec ){
		arr.push( rec );
		return arr;
	}, [] );
	
}
```

## Insert Records
```javascript
function insertRecords( strTableName, arrValues, boolDisableWorkflow ){
	/* Given a table name, array of objects, where
	 * each object contains the data for a new record,
	 * Insert the new objects into the table as new records.
	 * Optionally, disable workflow
	 */
	 	
	if( boolDisableWorkflow === undefined || boolDisableWorkflow == 'false' ){
		boolDisableWorkflow = false;
	}

	try{
		var gqRecords = new global.GlideQuery( strTableName )
		.disableWorkflow( boolDisableWorkflow )

		arrValues.forEach( function( record ){
			gqRecords.insert( record );
		} );
		
	}
	catch( e ){
	
		gs.error( 
			'An error occurred trying to insert records into ' + strTableName + 
			'\nValues: \n' + JSON.stringify( arrValues, null, 2 ) + 
			'\n\nError: ' + e.name + ': ' + e.message 
		);
		
	}
	
}

```

## Update Records
```javascript
function updateRecords( strTableName, strEncodedQuery, objValues, boolDisableWorkflow ){
	/* Given a table name, an encoded query, and an object of record values,
	 * Update all of the filtered records with the new values.
	 * Optionally, disable workflow
	 */
	 	
	if( boolDisableWorkflow === undefined || boolDisableWorkflow == 'false' ){
		boolDisableWorkflow = false;
	}

	try{

		return new global.GlideQuery.parse( strTableName, strEncodedQuery )
		.disableWorkflow( boolDisableWorkflow )
		.updateMultiple( objValues );
	
	}
	catch( e ){
	
		gs.error( 
			'An error occurred trying to update records in ' + strTableName + 
			'\nQuery: ' + strEncodedQuery + 
			'\nValues: \n' + JSON.stringify( objValues, null, 2 ) + 
			'\n\nError: ' + e.name + ': ' + e.message 
		);
		
	}
	
}

```

## Delete Records
```javascript
function deleteRecords( strTableName, strEncodedQuery, boolDisableWorkflow ){
	/* Given a table name and an encoded query,
	 * Delete all of the filtered records.
	 * Optionally, disable workflow
	 */
	 	
	if( boolDisableWorkflow === undefined || boolDisableWorkflow == 'false' ){
		boolDisableWorkflow = false;
	}

	try{

		return new global.GlideQuery.parse( strTableName, strEncodedQuery )
		.disableWorkflow( boolDisableWorkflow )
		.deleteMultiple();
	
	}
	catch( e ){
	
		gs.error( 
			'An error occurred trying to delete records from ' + strTableName + 
			'\nQuery: ' + strEncodedQuery + 
			'\n\nError: ' + e.name + ': ' + e.message 
		);
		
	}
	
}

```
Folder Name:

  - ./GlideQuery/Basic Wrappers
    - # GlideQuery

GlideQuery is a wrapper for the GlideRecord and GlideAggregate APIs. The wrapper offers several advantages, including a single point of entry, fail-fast with friendly error messaging, native JavaScript syntax, and more. Here are some functions that implement the basic GlideQuery capabilities to help you get started.

[Product Documentation](https://docs.servicenow.com/bundle/tokyo-application-development/page/app-store/dev_portal/API_reference/GlideQuery/concept/GlideQueryGlobalAPI.html)

[ServiceNow Community Blog Entries](https://developer.servicenow.com/blog.do?p=/tags/glidequery/) 
[Streyda Article](https://www.streyda.eu/post/gliderecordorglidequery)


## Get Records
```javascript
function getRecords( tableName, query, fields ){
	/* Given a table name, encoded query, and array of field names,
	 * Gather the request field attributes of the queried records,
	 * Build an array of JSON objects and return the array.
	 */
	 	
	return new global.GlideQuery.parse( tableName, query )
	.select( fields )
	.reduce( function( arr, rec ){
		arr.push( rec );
		return arr;
	}, [] );
	
}
```

## Insert Records
```javascript
function insertRecords( strTableName, arrValues, boolDisableWorkflow ){
	/* Given a table name, array of objects, where
	 * each object contains the data for a new record,
	 * Insert the new objects into the table as new records.
	 * Optionally, disable workflow
	 */
	 	
	if( boolDisableWorkflow === undefined || boolDisableWorkflow == 'false' ){
		boolDisableWorkflow = false;
	}

	try{
		var gqRecords = new global.GlideQuery( strTableName )
		.disableWorkflow( boolDisableWorkflow )

		arrValues.forEach( function( record ){
			gqRecords.insert( record );
		} );
		
	}
	catch( e ){
	
		gs.error( 
			'An error occurred trying to insert records into ' + strTableName + 
			'\nValues: \n' + JSON.stringify( arrValues, null, 2 ) + 
			'\n\nError: ' + e.name + ': ' + e.message 
		);
		
	}
	
}

```

## Update Records
```javascript
function updateRecords( strTableName, strEncodedQuery, objValues, boolDisableWorkflow ){
	/* Given a table name, an encoded query, and an object of record values,
	 * Update all of the filtered records with the new values.
	 * Optionally, disable workflow
	 */
	 	
	if( boolDisableWorkflow === undefined || boolDisableWorkflow == 'false' ){
		boolDisableWorkflow = false;
	}

	try{

		return new global.GlideQuery.parse( strTableName, strEncodedQuery )
		.disableWorkflow( boolDisableWorkflow )
		.updateMultiple( objValues );
	
	}
	catch( e ){
	
		gs.error( 
			'An error occurred trying to update records in ' + strTableName + 
			'\nQuery: ' + strEncodedQuery + 
			'\nValues: \n' + JSON.stringify( objValues, null, 2 ) + 
			'\n\nError: ' + e.name + ': ' + e.message 
		);
		
	}
	
}

```

## Delete Records
```javascript
function deleteRecords( strTableName, strEncodedQuery, boolDisableWorkflow ){
	/* Given a table name and an encoded query,
	 * Delete all of the filtered records.
	 * Optionally, disable workflow
	 */
	 	
	if( boolDisableWorkflow === undefined || boolDisableWorkflow == 'false' ){
		boolDisableWorkflow = false;
	}

	try{

		return new global.GlideQuery.parse( strTableName, strEncodedQuery )
		.disableWorkflow( boolDisableWorkflow )
		.deleteMultiple();
	
	}
	catch( e ){
	
		gs.error( 
			'An error occurred trying to delete records from ' + strTableName + 
			'\nQuery: ' + strEncodedQuery + 
			'\n\nError: ' + e.name + ': ' + e.message 
		);
		
	}
	
}

```
Folder Name:

  - ./GlideQuery/Basic Wrappers
    - # GlideQuery

GlideQuery is a wrapper for the GlideRecord and GlideAggregate APIs. The wrapper offers several advantages, including a single point of entry, fail-fast with friendly error messaging, native JavaScript syntax, and more. Here are some functions that implement the basic GlideQuery capabilities to help you get started.

[Product Documentation](https://docs.servicenow.com/bundle/tokyo-application-development/page/app-store/dev_portal/API_reference/GlideQuery/concept/GlideQueryGlobalAPI.html)

[ServiceNow Community Blog Entries](https://developer.servicenow.com/blog.do?p=/tags/glidequery/) 
[Streyda Article](https://www.streyda.eu/post/gliderecordorglidequery)


## Get Records
```javascript
function getRecords( tableName, query, fields ){
	/* Given a table name, encoded query, and array of field names,
	 * Gather the request field attributes of the queried records,
	 * Build an array of JSON objects and return the array.
	 */
	 	
	return new global.GlideQuery.parse( tableName, query )
	.select( fields )
	.reduce( function( arr, rec ){
		arr.push( rec );
		return arr;
	}, [] );
	
}
```

## Insert Records
```javascript
function insertRecords( strTableName, arrValues, boolDisableWorkflow ){
	/* Given a table name, array of objects, where
	 * each object contains the data for a new record,
	 * Insert the new objects into the table as new records.
	 * Optionally, disable workflow
	 */
	 	
	if( boolDisableWorkflow === undefined || boolDisableWorkflow == 'false' ){
		boolDisableWorkflow = false;
	}

	try{
		var gqRecords = new global.GlideQuery( strTableName )
		.disableWorkflow( boolDisableWorkflow )

		arrValues.forEach( function( record ){
			gqRecords.insert( record );
		} );
		
	}
	catch( e ){
	
		gs.error( 
			'An error occurred trying to insert records into ' + strTableName + 
			'\nValues: \n' + JSON.stringify( arrValues, null, 2 ) + 
			'\n\nError: ' + e.name + ': ' + e.message 
		);
		
	}
	
}

```

## Update Records
```javascript
function updateRecords( strTableName, strEncodedQuery, objValues, boolDisableWorkflow ){
	/* Given a table name, an encoded query, and an object of record values,
	 * Update all of the filtered records with the new values.
	 * Optionally, disable workflow
	 */
	 	
	if( boolDisableWorkflow === undefined || boolDisableWorkflow == 'false' ){
		boolDisableWorkflow = false;
	}

	try{

		return new global.GlideQuery.parse( strTableName, strEncodedQuery )
		.disableWorkflow( boolDisableWorkflow )
		.updateMultiple( objValues );
	
	}
	catch( e ){
	
		gs.error( 
			'An error occurred trying to update records in ' + strTableName + 
			'\nQuery: ' + strEncodedQuery + 
			'\nValues: \n' + JSON.stringify( objValues, null, 2 ) + 
			'\n\nError: ' + e.name + ': ' + e.message 
		);
		
	}
	
}

```

## Delete Records
```javascript
function deleteRecords( strTableName, strEncodedQuery, boolDisableWorkflow ){
	/* Given a table name and an encoded query,
	 * Delete all of the filtered records.
	 * Optionally, disable workflow
	 */
	 	
	if( boolDisableWorkflow === undefined || boolDisableWorkflow == 'false' ){
		boolDisableWorkflow = false;
	}

	try{

		return new global.GlideQuery.parse( strTableName, strEncodedQuery )
		.disableWorkflow( boolDisableWorkflow )
		.deleteMultiple();
	
	}
	catch( e ){
	
		gs.error( 
			'An error occurred trying to delete records from ' + strTableName + 
			'\nQuery: ' + strEncodedQuery + 
			'\n\nError: ' + e.name + ': ' + e.message 
		);
		
	}
	
}

```
Folder Name:

  - ./GlideQuery/Basic Wrappers
    - # GlideQuery

GlideQuery is a wrapper for the GlideRecord and GlideAggregate APIs. The wrapper offers several advantages, including a single point of entry, fail-fast with friendly error messaging, native JavaScript syntax, and more. Here are some functions that implement the basic GlideQuery capabilities to help you get started.

[Product Documentation](https://docs.servicenow.com/bundle/tokyo-application-development/page/app-store/dev_portal/API_reference/GlideQuery/concept/GlideQueryGlobalAPI.html)

[ServiceNow Community Blog Entries](https://developer.servicenow.com/blog.do?p=/tags/glidequery/) 
[Streyda Article](https://www.streyda.eu/post/gliderecordorglidequery)


## Get Records
```javascript
function getRecords( tableName, query, fields ){
	/* Given a table name, encoded query, and array of field names,
	 * Gather the request field attributes of the queried records,
	 * Build an array of JSON objects and return the array.
	 */
	 	
	return new global.GlideQuery.parse( tableName, query )
	.select( fields )
	.reduce( function( arr, rec ){
		arr.push( rec );
		return arr;
	}, [] );
	
}
```

## Insert Records
```javascript
function insertRecords( strTableName, arrValues, boolDisableWorkflow ){
	/* Given a table name, array of objects, where
	 * each object contains the data for a new record,
	 * Insert the new objects into the table as new records.
	 * Optionally, disable workflow
	 */
	 	
	if( boolDisableWorkflow === undefined || boolDisableWorkflow == 'false' ){
		boolDisableWorkflow = false;
	}

	try{
		var gqRecords = new global.GlideQuery( strTableName )
		.disableWorkflow( boolDisableWorkflow )

		arrValues.forEach( function( record ){
			gqRecords.insert( record );
		} );
		
	}
	catch( e ){
	
		gs.error( 
			'An error occurred trying to insert records into ' + strTableName + 
			'\nValues: \n' + JSON.stringify( arrValues, null, 2 ) + 
			'\n\nError: ' + e.name + ': ' + e.message 
		);
		
	}
	
}

```

## Update Records
```javascript
function updateRecords( strTableName, strEncodedQuery, objValues, boolDisableWorkflow ){
	/* Given a table name, an encoded query, and an object of record values,
	 * Update all of the filtered records with the new values.
	 * Optionally, disable workflow
	 */
	 	
	if( boolDisableWorkflow === undefined || boolDisableWorkflow == 'false' ){
		boolDisableWorkflow = false;
	}

	try{

		return new global.GlideQuery.parse( strTableName, strEncodedQuery )
		.disableWorkflow( boolDisableWorkflow )
		.updateMultiple( objValues );
	
	}
	catch( e ){
	
		gs.error( 
			'An error occurred trying to update records in ' + strTableName + 
			'\nQuery: ' + strEncodedQuery + 
			'\nValues: \n' + JSON.stringify( objValues, null, 2 ) + 
			'\n\nError: ' + e.name + ': ' + e.message 
		);
		
	}
	
}

```

## Delete Records
```javascript
function deleteRecords( strTableName, strEncodedQuery, boolDisableWorkflow ){
	/* Given a table name and an encoded query,
	 * Delete all of the filtered records.
	 * Optionally, disable workflow
	 */
	 	
	if( boolDisableWorkflow === undefined || boolDisableWorkflow == 'false' ){
		boolDisableWorkflow = false;
	}

	try{

		return new global.GlideQuery.parse( strTableName, strEncodedQuery )
		.disableWorkflow( boolDisableWorkflow )
		.deleteMultiple();
	
	}
	catch( e ){
	
		gs.error( 
			'An error occurred trying to delete records from ' + strTableName + 
			'\nQuery: ' + strEncodedQuery + 
			'\n\nError: ' + e.name + ': ' + e.message 
		);
		
	}
	
}

```
Folder Name:

  - ./GlideHTTPRequest
    - GlideHTTPRequest API is used to work on Glide HTTP Request and Response.

API Documentation Link for "PARIS" release : https://developer.servicenow.com/dev.do#!/reference/api/paris/server_legacy/GlideHTTPRequestAPI

Please update the variable details in the script to check it.
Folder Name:

  - ./Mail Scripts/Call UI Message or System Property in Notification Mail Script
    - Here is the syntax to call your UI Message or System property into Notification Mail script.
Folder Name:

  - ./Mail Scripts/Call Script Include in Notification Mail Script
    - Here is the syntax to call your Script Include from a Global or Scoped application into Notification Mail script.
Folder Name:

  - ./Mail Scripts/Open Survey In Portal
    - 1)create a notification on "Assessment Instance" table</br>
2)when record is created and state is ready to take trigger notification to assigned to </br>
3)use this mail script to get the url to survey in the email that takes them to the portal</br>
Folder Name:

  - ./Mail Scripts/Add Checklist
    - 
Folder Name:

  - ./Mail Scripts/Print variables to mail
    - Script block to be used within a Notification Email Script or as a standalone one.
It prints all variables + answers of a catalog produced record to the email body, along with the short description of the task on top (please check script).
Folder Name:

  - ./Mail Scripts/Add a link which opens ticket in Service Portal
    - Use this script to add a link in email notification which opens the ticket in Service Portal 
Folder Name:

  - ./Mail Scripts/Add HTML Table for Requested Item Variables
    - Use this snippet to create an HTML file of requested item variables.  Will exclude variables that are not needed (empty/undefined)
Folder Name:

  - ./Mail Scripts/HTML Table Creation from ServiceNow Table
    - This mail script uses a GlideRecord object to get values from a ServiceNow table and then format that information into an HTML table in a notification.

Replace "example_table" with your desired table.

Change the style tags to fit your desired results, like background-color, etc.
Folder Name:

  - ./Regular Expressions/AllowAnyLanguage
    - Allow Any Language Character Remove Special Characters, Can be used to verify valid names. Sorry Elon Musk's First born.
Folder Name:

  - ./Regular Expressions/Format mobile into Australian mobile format
    - # Format phone into Australian mobile Format

Use this script to format a phone number from +61433394881 style to 0433 394 881 style.
Folder Name:

  - ./Regular Expressions/Negative RegExp for Condition Builder
    - # Negative regular expressions for Condition Builder

## What problem does it solve?

Certain condition builders (not all, unfortunately) come with a __matches regex__ operator. This is very handy to filter records based on complex rules applied to strings.

Unfortunately, there is no __does not match regex__ operator and I would have needed this on several occasions.

## Solution

The solution is to use a negative regular expression by leveraging the **?!** operator (called _Negative Lookahead_). So one needs to find the proper regex for what it should match, and then invert it with a Negative Lookahead.

For example, the following regex matches a well formed MAC address:
```
^(([A-Fa-f0-9]{2}[:-]){5}[A-Fa-f0-9]{2}).*$
```

Whereas this one matches anything that does NOT match a well formed MAC address:
```
^(?!(([A-Fa-f0-9]{2}[:-]){5}[A-Fa-f0-9]{2})$).*$
```

The script in this example shows how to use this, but it's really in a condition builder that it will be useful. As matter of fact, a script can always reverse the logic (but the condition builder cannot). The script identifies all the entries in an array that do NOT have a well formed MAC address: note that it does not use a __false__ logic in the _if_, proving that the regex does revert the logic.
Folder Name:

  - ./Regular Expressions/Check if number has 10 digits
    - Script is used to check if the number has 10 digts( you can update the digit count in the code based on the need.
Folder Name:

  - ./Regular Expressions/Remove Extra Spaces
    - 
Folder Name:

  - ./Regular Expressions/Remove newline and carriage return
    - Will accept a string and remove all newline (\n) and carriage return (\r) characters
Folder Name:

  - ./Regular Expressions/Encode spaces for URLs
    - convert spaces to %20 for creating dynamic urls
Folder Name:

  - ./Regular Expressions/Poland country code
    - **Regular Expressions**

 Regular Expressions, which allows checking for Poland nine-digit Country code. Poland format starts with +48 and is followed by nine digits.

**Example effect of execution**

![Execution](ScreenShot_1.PNG)
Folder Name:

  - ./Regular Expressions/IP Address Validation
    - This regex validates for ip address(ipv4) based on the input.

Following are the valid IP address examples:

192.168.1.1

127.0.0.1

0.0.0.0

255.255.255.255

256.256.256.256

999.999.999.999

1.2.3

1.2.3.4
Folder Name:

  - ./Regular Expressions/Allow Characters + - ) ( for Phone numbers
    - ### Allows Characters +, -, (, ) for entering Phone Numbers

Allows characters useful for adding phone numbers in various formats like (+1) - 123 - 456 - 789, +1-978-654-362, (123) (567) (897) etc.
One can add more functionality to it, by controlling the number of digits added etc.
Folder Name:

  - ./Regular Expressions/Match URL's from ServiceNow domain
    - **Regular Expressions**

Regular Expressions, which allows checking if URL belongs to ServiceNow domain. It is verifying all starting prefix like 'https://', 'http://' or just 'www' which belongs to servicenow.com.

You can easily change that regex to different domain, by changing 'servicenow' text in regSN variable.

**Example effect of execution**

 ![Execution](ScreenShot_1.PNG)
Folder Name:

  - ./Regular Expressions/Find Emoji
    - # Detect emoji in string

Use this script to detect if string contains emoji
Folder Name:

  - ./CMDB/CMDB record count
    - 
Folder Name:

  - ./CMDB/IRE Queridentify
    - 
Folder Name:

  - ./CMDB/Mandatory Field Analysis
    - 
Folder Name:

  - ./CMDB/CSDM Maturity Report
    - 
Folder Name:

  - ./CMDB/IRE Errors
    - 
Folder Name:

  - ./GraphQL/Sample group query
    - 
Folder Name:

  - ./GraphQL/Sample group query
    - 
Folder Name:

  - ./GraphQL/Sample users query
    - 
Folder Name:

  - ./GraphQL/Sample users query
    - 
Folder Name:

  - ./GraphQL/Sample users query
    - 
Folder Name:

  - ./Script Includes/Get Reference Display Value
    - # Get Reference Choice Display Value

This scripts gets the display value of the selected reference value. 

> Method: getChoiceDisplayValue(question, value)

-   @param {String} table: name of the referenced table.
-   @param {String} value: Value of that reference field
Folder Name:

  - ./Script Includes/Testing Script Include Using Jasmine
    - # Testing Script Include Using ATF and Jasmine

Step 1.
Create a new Script Include based on Sample Calculator Script.js

Step 2.
Create a sample ATF Test

Step 3. Add a Test Step by clicking "Add Test Step". Update the content of the "Test Script" field based on content of the Sample Jasmine Script.js

Step 4. Run the test
Folder Name:

  - ./Script Includes/Testing Script Include Using Jasmine
    - # Testing Script Include Using ATF and Jasmine

Step 1.
Create a new Script Include based on Sample Calculator Script.js

Step 2.
Create a sample ATF Test

Step 3. Add a Test Step by clicking "Add Test Step". Update the content of the "Test Script" field based on content of the Sample Jasmine Script.js

Step 4. Run the test
Folder Name:

  - ./Script Includes/Get Group Members
    - # Get Group Members by Id

A Script utils containing utility functions, to get the group members sys ids
Folder Name:

  - ./Script Includes/Create Multiple RITMS from MRVS
    - # Create Multiple RITMS from MRVS
Use this script to submit multiple Requested Items with data being populated from the MRVS.
Match the variables names in the Obj to the respective Catalog Item variable names and the MRVS variables to the variable names for the MRVS
Folder Name:

  - ./Script Includes/PerformanceAnalyticsUtils
    - # Performance Analytics Utils

A Script Include to gather methods for handling Performance Analytics subjects. Typical use case is to be invoked by PA Scripts (for custom aggregation or breakdown mappings).

## getCmdbClassTableNames

Returns sys_id's of all the tables (sys_db_object) starting -and including- a start class. This is very useful to build a PA Breakdown on CMDB Classes. This method is fast as it uses the sys_class_path field to query sys_db_object.

This is a replacement for SNC.CMDBUtil.getAllChildrenOfAsCommaList() that I did not manage to invoke from Breakdown Source record Condition Builder (was getting an illegal access error because of the SNC scope).

I understand this also could be in an CMDBUtil Script Include, but I found very useful for building a PA Breakdown Source.
Folder Name:

  - ./Script Includes/Excel Parser
    - Server side Excel parser utility leveraging the GlideExcelParser API.

Pass in the sys_id of an Excel attachment and get back an array of objects, with every row in the sheet being an element in the array.
Folder Name:

  - ./Script Includes/GlideDateTimeUtils
    - 
Folder Name:

  - ./Script Includes/BackfillAssignmentGroup
    - # BackFillAssignmentGroup

This script include is an advanced reference qualifier for the Assignment group field. It restricts the Assignment group choices to only relevant groups of which the current Assigned to user is a member.

## Current Configuration

The script include filters for groups with the OOTB **type** of "itil" assigned to them (generally considered fulfiller groups). As such, it's ideal for use on the base Task and its extended tables (Incident, Problem, Change). Note that the **type** field is a list and the values should be queried by sys_id. It would be simple to modify the script to constrain the field to different roles or other attribute.

## Use

1. Create a script include called **BackfillAssignmentGroup**.
2. Set **Accessible from** to **This application scope only**.
3. Add description **Links assignment group field to assigned to field so that only the groups of which the assigned to is a member will be displayed for selection.** or write your own.
4. Paste the entire contents of the script file into the **Script** field.
5. Save.

Configure the dictionary entry of the assignment_group field on Task table.

1. Type **task.list** into the navigator and press **Enter**.
2. Right-click any column name and select **Configure>Table**.
3. Select **Advanced View** under **Related Links** if not already.
4. Under the **Reference Specification** tab, set **Use reference qualifier** to **Advanced**.
5. In the **Reference qual** field, enter: **javascript:new BackfillAssignmentGroup().BackfillAssignmentGroup()**
6. Save
Folder Name:

  - ./Script Includes/Table List Copy Context Options
    - # Add "Copy Field Name, Value, Display Value" to context menu for list records

Add context menu options allowing for admins to be able to right click a record's field in the list view and choose "Copy Field Name", "Copy Field Value", and "Copy Field Display Value" to quickly get the column variable name and values to their clipboard.

## Setting up

- Create a script include and copy the .js file. Set it as `Client callable = true`
- Create sys_ui_context_menu (Context Menu) records, one each for:
    - Copy Field Value
    - Copy Field Name
    - Copy Field Display Value

## Context Menu records configuration

- Table: Global [global]
- Menu: List row
- Type: Action
- Name: Copy Field Value
- Order: Use 51, 52, and 53
- Acive: True
- Run onShow script: False
- Condition: `gs.hasRightsTo("ui/context_menu.copy_sysid/read", null)`
- Action Script: see .js files in this folder for each one
Folder Name:

  - ./Script Includes/Table List Copy Context Options
    - # Add "Copy Field Name, Value, Display Value" to context menu for list records

Add context menu options allowing for admins to be able to right click a record's field in the list view and choose "Copy Field Name", "Copy Field Value", and "Copy Field Display Value" to quickly get the column variable name and values to their clipboard.

## Setting up

- Create a script include and copy the .js file. Set it as `Client callable = true`
- Create sys_ui_context_menu (Context Menu) records, one each for:
    - Copy Field Value
    - Copy Field Name
    - Copy Field Display Value

## Context Menu records configuration

- Table: Global [global]
- Menu: List row
- Type: Action
- Name: Copy Field Value
- Order: Use 51, 52, and 53
- Acive: True
- Run onShow script: False
- Condition: `gs.hasRightsTo("ui/context_menu.copy_sysid/read", null)`
- Action Script: see .js files in this folder for each one
Folder Name:

  - ./Script Includes/Table List Copy Context Options
    - # Add "Copy Field Name, Value, Display Value" to context menu for list records

Add context menu options allowing for admins to be able to right click a record's field in the list view and choose "Copy Field Name", "Copy Field Value", and "Copy Field Display Value" to quickly get the column variable name and values to their clipboard.

## Setting up

- Create a script include and copy the .js file. Set it as `Client callable = true`
- Create sys_ui_context_menu (Context Menu) records, one each for:
    - Copy Field Value
    - Copy Field Name
    - Copy Field Display Value

## Context Menu records configuration

- Table: Global [global]
- Menu: List row
- Type: Action
- Name: Copy Field Value
- Order: Use 51, 52, and 53
- Acive: True
- Run onShow script: False
- Condition: `gs.hasRightsTo("ui/context_menu.copy_sysid/read", null)`
- Action Script: see .js files in this folder for each one
Folder Name:

  - ./Script Includes/Table List Copy Context Options
    - # Add "Copy Field Name, Value, Display Value" to context menu for list records

Add context menu options allowing for admins to be able to right click a record's field in the list view and choose "Copy Field Name", "Copy Field Value", and "Copy Field Display Value" to quickly get the column variable name and values to their clipboard.

## Setting up

- Create a script include and copy the .js file. Set it as `Client callable = true`
- Create sys_ui_context_menu (Context Menu) records, one each for:
    - Copy Field Value
    - Copy Field Name
    - Copy Field Display Value

## Context Menu records configuration

- Table: Global [global]
- Menu: List row
- Type: Action
- Name: Copy Field Value
- Order: Use 51, 52, and 53
- Acive: True
- Run onShow script: False
- Condition: `gs.hasRightsTo("ui/context_menu.copy_sysid/read", null)`
- Action Script: see .js files in this folder for each one
Folder Name:

  - ./Script Includes/Logger
    - # ArtifactRank

Logger script include that helps you to specify the environments that you want create log records without commenting
your logging lines in your code. The logger will check if it is one of the sub-prod environments that you have specified
and log the line otherwise just ignore it. This means you just configure the logger once and then you don't have to
comment or remove your logging code at all!

## Usage

```javascript
var logger = new SubProdLogger(); // This will log for the default environments that is configured e.g. 'test', "uat", 'stage', 'qa', 'dev'. If you have other environment that you want to log for then register it in the line 35 if the SubProdLogger.js file i.e add new values here: this._subProdKeywords = ['test', "uat", 'stage', 'qa', 'dev'];

logger.warn('This is a warning.');
```
Folder Name:

  - ./Script Includes/StripHTML
    - # StripHTML
Script Include that removes all HTML from a specific string.

It doesn't use the typical `Class.create`, instead it is a simple javascript function.
Check out this blog post for more info about the "Function Pattern": https://codecreative.io/blog/interface-design-patterns-function-pattern/

## Example Script
```javascript
var someHTML = "<span><b>Eaque pariatur nemo facere accusantium non enim.</b></span>";
var plainText = StripHTML(someHTML);
gs.debug(plainText);
```
Folder Name:

  - ./Script Includes/Auto Execute Import Set on File Attachment
    - # Auto Execute Import Set on File Attachment
You have to create a data source and a transform map first. After that you can use Flow Designer with the trigger condition Attachment is added to the data source. Once the flow triggers, it will call the action which in turn will trigger the Script Include to create an Import Set and Transform Map.
Folder Name:

  - ./Script Includes/Auto Execute Import Set on File Attachment
    - # Auto Execute Import Set on File Attachment
You have to create a data source and a transform map first. After that you can use Flow Designer with the trigger condition Attachment is added to the data source. Once the flow triggers, it will call the action which in turn will trigger the Script Include to create an Import Set and Transform Map.
Folder Name:

  - ./Script Includes/KBArticleExpPDF
    - This utility contains a script include which generates PDF export of knowledge article  and this script include handles all HTML formatting of Knowledge article as well.
Also, this utility will handle any images attached in KB article body.

Sample Script to call this Script Include:

new PolicyPDFHelper().getPDFBase64('b10db60e2fc738101d84d2172799b69c','landscape');

// First paramter is sys_id of KB article from kb_knowledge record
// Second Parameter is PDF Export Mode. Accepted inputs are landscape or portrait.
Folder Name:

  - ./Script Includes/StarterPack
    - Also available on Share here: https://developer.servicenow.com/connect.do#!/share/contents/6592535_script_include_starter_pack?t=PRODUCT_DETAILS

and related to [CCB1193-K21 Script Includes: What are they and why should I care?](https://events.servicenow.com/widget/servicenow/knowledge2021/library/session/1612301555107001YVuE#1617832086855001eNVb)
Folder Name:

  - ./Script Includes/StarterPack
    - Also available on Share here: https://developer.servicenow.com/connect.do#!/share/contents/6592535_script_include_starter_pack?t=PRODUCT_DETAILS

and related to [CCB1193-K21 Script Includes: What are they and why should I care?](https://events.servicenow.com/widget/servicenow/knowledge2021/library/session/1612301555107001YVuE#1617832086855001eNVb)
Folder Name:

  - ./Script Includes/StarterPack
    - Also available on Share here: https://developer.servicenow.com/connect.do#!/share/contents/6592535_script_include_starter_pack?t=PRODUCT_DETAILS

and related to [CCB1193-K21 Script Includes: What are they and why should I care?](https://events.servicenow.com/widget/servicenow/knowledge2021/library/session/1612301555107001YVuE#1617832086855001eNVb)
Folder Name:

  - ./Script Includes/StarterPack
    - Also available on Share here: https://developer.servicenow.com/connect.do#!/share/contents/6592535_script_include_starter_pack?t=PRODUCT_DETAILS

and related to [CCB1193-K21 Script Includes: What are they and why should I care?](https://events.servicenow.com/widget/servicenow/knowledge2021/library/session/1612301555107001YVuE#1617832086855001eNVb)
Folder Name:

  - ./Script Includes/StarterPack
    - Also available on Share here: https://developer.servicenow.com/connect.do#!/share/contents/6592535_script_include_starter_pack?t=PRODUCT_DETAILS

and related to [CCB1193-K21 Script Includes: What are they and why should I care?](https://events.servicenow.com/widget/servicenow/knowledge2021/library/session/1612301555107001YVuE#1617832086855001eNVb)
Folder Name:

  - ./Script Includes/StarterPack
    - Also available on Share here: https://developer.servicenow.com/connect.do#!/share/contents/6592535_script_include_starter_pack?t=PRODUCT_DETAILS

and related to [CCB1193-K21 Script Includes: What are they and why should I care?](https://events.servicenow.com/widget/servicenow/knowledge2021/library/session/1612301555107001YVuE#1617832086855001eNVb)
Folder Name:

  - ./Script Includes/GlideRecord to JSON
    - # GlideRecord to JSON object converter
* Description: This script include (gr2obj) converts GlideRecord to a JSON object
* Sample Usage: 
```javascript
var gr = new GlideRecord('incident');
// Get an incident record
gr.get('96cef4561b3530108b59a8e5604bcb74');
// Call the script include
var obj = gr2obj(gr);
// Stringify the object and display
gs.info(JSON.stringify(obj));
```
* Sample Output:
```json
{"active":"true","activity_due":"","additional_assignee_list":null,"approval":"not requested","approval_history":"","approval_set":"","assigned_to":null,"assignment_group":null,"business_duration":"","business_service":null,"business_stc":null,"calendar_duration":"","calendar_stc":null,"caller_id":"System Administrator","category":"inquiry","caused_by":null,"child_incidents":"0","close_code":null,"close_notes":null,"closed_at":"","closed_by":null,"cmdb_ci":null,"comments":"","comments_and_work_notes":"","company":null,"contact_type":null,"contract":null,"correlation_display":null,"correlation_id":null,"delivery_plan":null,"delivery_task":null,"description":null,"due_date":"","escalation":"0","expected_start":"","follow_up":"","group_list":null,"hold_reason":null,"impact":"3","incident_state":"2","knowledge":"false","location":null,"made_sla":"true","notify":"1","number":"INC0010007","opened_at":"2021-08-08 03:42:27","opened_by":"System Administrator","order":null,"parent":null,"parent_incident":null,"priority":"5","problem_id":null,"reassignment_count":"0","rejection_goto":null,"reopen_count":"0","reopened_by":null,"reopened_time":"","resolved_at":"","resolved_by":null,"rfc":null,"route_reason":null,"service_offering":null,"severity":"3","short_description":"test2","sla_due":"","state":"2","subcategory":null,"sys_class_name":"incident","sys_created_by":"admin","sys_created_on":"2021-08-08 03:42:56","sys_domain":"global","sys_domain_path":"/","sys_id":"96cef4561b3530108b59a8e5604bcb74","sys_mod_count":"1","sys_tags":"","sys_updated_by":"admin","sys_updated_on":"2021-09-27 16:35:00","task_effective_number":"INC0010007","time_worked":"","u_requested_for":"Abel Tuter","universal_request":null,"upon_approval":"proceed","upon_reject":"cancel","urgency":"3","user_input":"","variables":null,"watch_list":null,"wf_activity":null,"work_end":"","work_notes":"","work_notes_list":null,"work_start":""}
```
Folder Name:

  - ./Script Includes/Slack JSON Block Factory
    - This Script Includes provides simple factories (Slacktory) to create Slack JSON blocks, that can be sent in payloads. 
Documentation for syntax is inline in the code.

The factories will always return the created or modified block [Object].
Folder Name:

  - ./Script Includes/Delete Multiple Records Async
    - 
Folder Name:

  - ./Script Includes/ManagerRecursiveUtil
    - Many teams have a  use case to build reports for executives that shows data related all groups underneath them, such as problem tickets assigned to their reports. 

The script include return a list of group sys_ids that roll up to the given leader. 

This is  client callable script includes and there is a limit the maximum amount of reporting depth, such as 7 users for performance reaasons.
Folder Name:

  - ./Script Includes/API Model Template for New Application
    - # Application Baseline Pattern

Use this Script Include to extend into your new API model and provide a set of re-usable and extendable methods to enhance your application design

Create the new Script Include in your SN instance in the relevant scope, using the matching filename
Then change the name and ensure all references are updated

You can re-use and extend this pattern based on any object and centralise code in the core API base
Folder Name:

  - ./Script Includes/API Model Template for New Application
    - # Application Baseline Pattern

Use this Script Include to extend into your new API model and provide a set of re-usable and extendable methods to enhance your application design

Create the new Script Include in your SN instance in the relevant scope, using the matching filename
Then change the name and ensure all references are updated

You can re-use and extend this pattern based on any object and centralise code in the core API base
Folder Name:

  - ./Script Includes/API Model Template for New Application
    - # Application Baseline Pattern

Use this Script Include to extend into your new API model and provide a set of re-usable and extendable methods to enhance your application design

Create the new Script Include in your SN instance in the relevant scope, using the matching filename
Then change the name and ensure all references are updated

You can re-use and extend this pattern based on any object and centralise code in the core API base
Folder Name:

  - ./Script Includes/API Model Template for New Application
    - # Application Baseline Pattern

Use this Script Include to extend into your new API model and provide a set of re-usable and extendable methods to enhance your application design

Create the new Script Include in your SN instance in the relevant scope, using the matching filename
Then change the name and ensure all references are updated

You can re-use and extend this pattern based on any object and centralise code in the core API base
Folder Name:

  - ./Script Includes/API Model Template for New Application
    - # Application Baseline Pattern

Use this Script Include to extend into your new API model and provide a set of re-usable and extendable methods to enhance your application design

Create the new Script Include in your SN instance in the relevant scope, using the matching filename
Then change the name and ensure all references are updated

You can re-use and extend this pattern based on any object and centralise code in the core API base
Folder Name:

  - ./Script Includes/API Model Template for New Application
    - # Application Baseline Pattern

Use this Script Include to extend into your new API model and provide a set of re-usable and extendable methods to enhance your application design

Create the new Script Include in your SN instance in the relevant scope, using the matching filename
Then change the name and ensure all references are updated

You can re-use and extend this pattern based on any object and centralise code in the core API base
Folder Name:

  - ./Script Includes/API Model Template for New Application
    - # Application Baseline Pattern

Use this Script Include to extend into your new API model and provide a set of re-usable and extendable methods to enhance your application design

Create the new Script Include in your SN instance in the relevant scope, using the matching filename
Then change the name and ensure all references are updated

You can re-use and extend this pattern based on any object and centralise code in the core API base
Folder Name:

  - ./Script Includes/API Model Template for New Application
    - # Application Baseline Pattern

Use this Script Include to extend into your new API model and provide a set of re-usable and extendable methods to enhance your application design

Create the new Script Include in your SN instance in the relevant scope, using the matching filename
Then change the name and ensure all references are updated

You can re-use and extend this pattern based on any object and centralise code in the core API base
Folder Name:

  - ./Script Includes/API Model Template for New Application
    - # Application Baseline Pattern

Use this Script Include to extend into your new API model and provide a set of re-usable and extendable methods to enhance your application design

Create the new Script Include in your SN instance in the relevant scope, using the matching filename
Then change the name and ensure all references are updated

You can re-use and extend this pattern based on any object and centralise code in the core API base
Folder Name:

  - ./Script Includes/API Model Template for New Application
    - # Application Baseline Pattern

Use this Script Include to extend into your new API model and provide a set of re-usable and extendable methods to enhance your application design

Create the new Script Include in your SN instance in the relevant scope, using the matching filename
Then change the name and ensure all references are updated

You can re-use and extend this pattern based on any object and centralise code in the core API base
Folder Name:

  - ./Script Includes/API Model Template for New Application
    - # Application Baseline Pattern

Use this Script Include to extend into your new API model and provide a set of re-usable and extendable methods to enhance your application design

Create the new Script Include in your SN instance in the relevant scope, using the matching filename
Then change the name and ensure all references are updated

You can re-use and extend this pattern based on any object and centralise code in the core API base
Folder Name:

  - ./Script Includes/API Model Template for New Application
    - # Application Baseline Pattern

Use this Script Include to extend into your new API model and provide a set of re-usable and extendable methods to enhance your application design

Create the new Script Include in your SN instance in the relevant scope, using the matching filename
Then change the name and ensure all references are updated

You can re-use and extend this pattern based on any object and centralise code in the core API base
Folder Name:

  - ./Script Includes/Client and Server Callable Script Include
    - # Client and Server Callable Script Include

Example of a script include that can be called via both client and server.
Folder Name:

  - ./Script Includes/TableUtils Extension
    - 
Folder Name:

  - ./Script Includes/Match URL with a String
    - # Match URL with a String using Regex

This script gets the url using the referer method and matches the substring in the url.
Folder Name:

  - ./Script Includes/Dynamic Dropdown List
    - 
Folder Name:

  - ./Script Includes/Dynamic Dropdown List
    - 
Folder Name:

  - ./Script Includes/JSONtoYAML
    - Hi Everyone,

This code is to convert JSON object into Yaml format.

To use this please pass the JSON object as below to this function as shown below

var conYaml = global.SCRIPTINCLUDENAME ('JSON OBJECT');

conYaml will hold the converted Yaml.

**Inputs**:
{ hello: 'world', hello2: [ 'hello', 'world' ] }

**Outputs**:
---
hello: world
hello2:
- hello
- world
Folder Name:

  - ./Script Includes/customArrayUtil
    - Convert input array to JSON 

Make a function call like

var arrayObj = ['name','John','age','30'];

var outputObj = new customArrayUtil().arrToJSON(arrayObj, true);

output would be a JSON Object like {"name":"John","Age":"32"}
Folder Name:

  - ./Script Includes/Hybrid Script Include for AJAX or Server Side Parameters
    - This example shows how one could code a script include that might be called in two different scenarios. One being a client AJAX call, and the other being a server side call, from another script include perhaps.

Example usage:
Client script AJAX call:

        var ajax = new GlideAjax('example_hybrid_parameters');
        ajax.addParam('sysparm_name', 'exampleHybrid');
        ajax.addParam('sysparm_parm1', parm1);
        ajax.addParam('sysparm_parm2', parm2);
        ajax.addParam('sysparm_parm3', parm3);
        ajax.addParam('sysparm_parm4', parm4);
        ajax.getXMLAnswer(exampleResponse);

    Call from server side script:

        var pr = new example_hybrid_parameters();
        result = pr.checkPrereq(parm1, parm2, parm3, parm4);
        return result;
Folder Name:

  - ./Script Includes/attachments
    - 
Folder Name:

  - ./Script Includes/Excel Attachment Via script
    - 
Folder Name:

  - ./Script Includes/Role Checker Util
    - # Script incude with 4 functions to check if users have a certain role.
Should work server side as well as client side with the right prameters (with some caviats for the 4th function).
Pay attention to the defined sysparm names in the script if used on client side.

## hasRoleID
Checks if a user has a given role based on user and role sys_id passed in
Returns a boolean value of true or false depending on whether or not the user has the role
* @param1 - roleID: must be the sys_id of the role to check
* @param2 -userID: must be the sys_id of the user to check
* @returns: true/false

## hasRoleEmail
Checks if a user has a given role based on sys_id of role and email address of user passed in
Only makes sense if user has an account in ServiceNow, otherwise it won't have a role anyway :)
Returns a boolean value of true or false depending on whether or not the user has the role
* @param1 - roleID: must be the sys_id of the role to check
* @param2 - email: must be an email address in string format
* @returns: true/false

## checkArray
Checks if an array of users have a given role based on the role's name (note: not sys_id!)
* @param1 - roleName: must be the name of the role to check as string
* @param2 - array: must be an array that contains sys_ids, email addresses or a combination of both
* @returns: - a comma separated list (stringified array) of names (can be changed) of those users who have the provided role. You can remove stringification to return an array (for server side scripts).

## checkArrayGetObjects
Checks if an array of users have a given role based on the role's name
* @roleName: must be name of the role to check as string
* @array: must be an array that contains sys_ids, email addresses or a combination of both.
* @returns: an array of objects with some details of the users who have the provided role. You can extend the object per your requirements, by default it returns sys_id, name and email.

NOTE: if you want to use this function in GlideAjax, you should stringify the array here, and convert it back (if you want) on the client side!
Folder Name:

  - ./Script Includes/Check User Has Role
    - # User Has Role

This script checks whether the user has a role or not.
This script takes two arguments

Argument #1: userId - userId of the record for which you need to validate the roles exists
Argument #2: roleId - roleId is the sys_id of the role that we need to check whether exists against the provided userId
Folder Name:

  - ./Script Includes/Get Field Label in Specific Language
    - # Get Field Label in Specific Language

This Script Include enables retrieving the label of a certain table field in any given language. 
Often in multi-language instances, the label of a field must be accessed via a script (e.g. to add it to the HTML of an email or add it to another fields like the description or work notes). Instead of retrieving the value each time individually this script include can be re-used (e.g. by multiple Business Rules or Mail Scripts). 

### Instruction

Call the Script Include via the following example code from any server-side script (e.g. Business Rule, Mail Script or Flow Action). If you want, you can also make the Script Include client callable and make it available to Client Scripts. Make sure to provide the correct table name, field name and language in your function call. Be aware, that in some cases the field may be located on a parent table. In this case, you would have to provide the parent table name to the script. 

```javascript
var util =new LanguageUtils();
gs.log(util.getLabel("incident", "category", "de"));
```


### Benefits
- If no label in the provided language can be found, the default English label is returned
- Re-use this Script Include and call it from different types of scripts (e.g. Business Rule, Mail Script or Flow Action)
Folder Name:

  - ./Script Includes/Get Choice Display Value
    - # Get Selected Choice Display Value

This scripts gets the display value of the selected choice. 

> Method: getChoiceDisplayValue(question, value)

-   @param {String} question: Name of the question that needs to be queried
-   @param {String} value: Value of that question
Folder Name:

  - ./Script Includes/VariableHelper
    - ## Variable Helper

 Working with variables in ServiceNow is no fun sometimes, especially [Multi Row Variable Sets](https://docs.servicenow.com/bundle/paris-application-development/page/script/server-scripting/concept/c_ScriptableServiceCatalogVariables.html#d2332110e207).  For that reason I created a helper Script Include to make my life easier.  

 There are 4 parameters that can be passed as an object when instantiating the Script Include or after with setter functions.  All default to false;


 * <b>useDisplayValue</b>:  This will return the display value of all variables instead of value
 * <b>expandRef</b>      :  This will return any reference field as an object. 
 * <b>useLabel</b>       :  Variable/Field Labels will be used instead of name.
 * <b>debug</b>          :  Enable additional logging


### Example

```
var helperOptions = {
  "useLabel": true,
  "useDisplayValue": true ,
  "expandRef": false
};
var varHelper = new variableHelper(helperOptions); 
varHelper.setDebug(true); //example of using setter function

var myVariables = varHelper.getVariables(myGlideRecordObject); //Get an object containing all variables
var myMRVS = varHelper.getMRVS(myGlideRecordObject.variables[mrvsName]); //Get a specific MRVS as an array of objects
  
```
Folder Name:

  - ./Script Includes/CatalogUtils
    - # CatalogUtils
This Script Include is a helper class for dealing with Service Catalog Items
and Requested Items.
## getCatalogVariables()
Returns all variables of a given RITM as stringified array of JSON objects. 
This method thus corresponds to the "Get Catalog Variables" action in a flow and 
it can be used both server-side and client-side.

A single JSON object has the following properties:

**Note:**\
Variable types with no values (e.g. containers) are excluded.

### Example for server-side call
```javascript
var grRITM = new GlideRecord('sc_req_item');

if (grRITM.get('485ae5bf2fc930105bd5d0e62799b662')) {
    var jsonVariables = JSON.parse((new CatalogUtils()).getVariables(grRITM));
}
```
### Example for client-side call
```javascript
var gaCatalogUtils = new GlideAjax('CatalogUtils');
	
gaCatalogUtils.addParam('sysparm_name', 'getVariables');
gaCatalogUtils.addParam('sysparm_ritm_sys_id', '485ae5bf2fc930105bd5d0e62799b662');

gaCatalogUtils.getXMLAnswer(function(strAnswer) {
	var jsonVariables = JSON.parse(strAnswer);
});

var jsonVariables = JSON.parse(gaCatalogUtils.getAnswer() || "");
```
### Example of returned values
```javascript
[
  {
    "strType": "8",
    "strName": "issued_by_name",
    "strQuestionText": "Issued by",
    "strValue": "62826bf03710200044e0bfc8bcbe5df1",
    "strDisplayValue": "Abel Tuter"
  },
  {
    "strType": "6",
    "strName": "issued_by_phone",
    "strQuestionText": "Phone",
    "strValue": "170",
    "strDisplayValue": "170"
  }
]
```
Folder Name:

  - ./Script Includes/ConversationUtils
    - 
Folder Name:

  - ./Script Includes/Records Calculator
    - 
Folder Name:

  - ./Script Includes/CSV Parser
    - # Script Include: CSVParser

A script includes that parses concatenated CSV string and returns and array of the JSON objects for each row of the CSV data.

## Example usage

```
var csv = "John, Doe, 33\nJane, Doe, 32\nJack, Doe, 11\nJosh, Doe, 13"  // Your CSV data
var delimiter = ","
var headers = ["first_name", "last_name", "age"] // Your CSV data headers
var result = parser.parse(csv, headers, delimiter);
```
Folder Name:

  - ./Script Includes/getGlideRecordObject
    - 
Folder Name:

  - ./Script Includes/Standard Change Creator
    - This Script Includes provides a way to create a Standard Change, that will be auto-populated with certain fields.

Usage and list of required variables, as well as documentation and commets are inline in the code.
Folder Name:

  - ./Script Includes/UserCriteriaUtil
    - # UserCriteriaUtil
This Script Include helps to evaluate if a certain UserCriteria did match with a User.

It doesn't use the typical `Class.create`, instead it is a simple javascript function.
Check out this blog post for more info about the "Function Pattern": https://codecreative.io/blog/interface-design-patterns-function-pattern/

## Example Script
```javascript
var myUserCriteriaSysId = gs.getProperty("<my_user_criteria_sys_id>");
//Will match against the current user
UserCriteriaUtil().match(myUserCriteriaSysId);
//Will match against a specific user
UserCriteriaUtil("<user_sys_id>").match(myUserCriteriaSysId);
```
Folder Name:

  - ./Script Includes/UserUtil
    - # UserUtil

A collection of scripts related to some esoteric user functions.

## userMemberOf();

The conceit of this function was to filter a list of assets assigned to the _members_ of a specific group. Returns the sys_ids of the group members. The argument passed in should be the display name of the group.

### Example

On a list, in the condition builder, choose **assigned_to.sys_id** (or whatever sys_user field you need), select **is one of** for the operator and enter
`javascript: new userUtil().userMemberOf("Service Desk")` in the **assigned_to** field.

Example Image
![userMemberOf example](userMemberOf.png)

## isManager();

Returns true or false if the passed in user has direct reports or not. Useful in ACLs, User Criteria, and various access/UI checks.

### Example

`var manager_check = new userUtil().isManager(gs.getUser()); `gs.info(manager_check);

> False

## getUserAssets()

Returns a comma-separated list of sys_ids for assets belonging to the user. Can be used to retrieve a user's current assets in a workflow for fulfillment activity.

### Example

`var util = new userUtil();`  
`assets = util.getUserAssets(gs.getUserID());`

> 3a3bf7421bdf9c50470a4267cc4bcb35,5e6930081b8f8c94470a4267cc4bcbaa
Folder Name:

  - ./Script Includes/regexCheckerScript
    - Script Include to check regex 

This script include can be used in a report or any other script/BR/Action to check if a particular type of text or a field matches the required regex. 
Returns the sys_id of the records that match the regex. You can select your desired table, query and field, also update the required regex in the script. 

Thankyou.
Folder Name:

  - ./Script Includes/NotificationUtil
    - # NotificationUtil

Quickly format all MRVS variables into a table of your current record into a notification mail scripts by using the NotificationUtil script include.

## Usage

Mail script
```javascript
(function runMailScript(/* GlideRecord */ current, /* TemplatePrinter */ template,
          /* Optional EmailOutbound */ email, /* Optional GlideRecord */ email_action,
          /* Optional GlideRecord */ event) {
              template.print(new notificationUtil().formatMRVS(current))
})(current, template, email, email_action, event);
```
Folder Name:

  - ./Script Includes/HTMLUtils
    - # Creates an HTML Table from an object

@param  {String} [title] - Title above table
@param  {Object} [table] - Object with headers attribute and row multi dimension array
@returns {String} HTML Table

### Example
```js
var table = {
header:['col1','col2'],
rows:[['row1col1','row1col2'],
        ['row2col1','row2col2']]
}

var hU = new HTMLUtils();
hU.createHTMLTable("Test",table);
```
### Output
```html
<p style='margin: 10px 0px 10px;'><b>Test</b></p><table class='template_TBL table'><tbody><tr><td>col1</td><td>col2</td></tr><tr><td>row1col1</td><td>row1col2</td></tr><tr><td>row2col1</td><td>row2col2</td></tr></tbody></table>
```
Folder Name:

  - ./Script Includes/Merge Array
    - 	 @name mergeArray
	 @description Compare two arrays of objects, provide add/remove/edit based on the difference of the two arrays
	 @param  {Object} [originalArray] - Array of objects is the base of comparison
	 @param  {Object} [modifiedArray] - Array of objects compared against original to determin add/remove/edit
	 @param  {String} [uniqueProperty] - Which object property to coalesce typically sys_id
	 @param  {String} [compareProperty] - Which object property to compare
	 @returns {Object} Array of objects with included 'action' property indicating add/remove/edit
   
   This is something I wrote when comparing JSON objects from MRVS that were leveraged on a catalog item to maintain CMDB relationships, however, doesn't have to be limited to that.
Folder Name:

  - ./Script Includes/UnloadXml
    - # Unload XML
With this script include you can export a GlideRecord Query to XML which can be imported via the "Import XML" functionality.

```javascript
var exportedXmlStr = UnloadXml("incident", "active=true");
```
Folder Name:

  - ./Script Includes/Public Script Include search
    - # Find public Script Includes

The snippet helps to find public Script Includes (can be executed by a non-logged-in user) and check their security later manually.

Such Script Include can be called from a public page (e.g. login.do page) in the browser console.
Folder Name:

  - ./Script Includes/Retrieve Last Comment by Ticket
    - # Retrieve Last Comment By Ticket

This script returns the last comment that has been added on a ticket by the record id.
The function 'retrieveLastCommentByTicket' requires two arguments

    Argument #1: sys_id - this is the sys_id of the record from which you need to pick the last comment
    Argument #2: tableName - this is the table name of the record
Folder Name:

  - ./Script Includes/Generate QR Code and attach to RITM
    - # Create QR Code
This sample script uses a free QR Code API and does a REST call to the server and returns the QR code as image. Then attaches
the QR code into Requested Item record.

In the script, replace the Requested Item sys_id with sys_id of your record. Change the text to the text you want to appear in the QR Code.
Folder Name:

  - ./Script Includes/Collect Field Values from Any One Table Record
    - 
Folder Name:

  - ./Script Includes/Scheduled Recursion
    - # Scheduled Recursion

To take action on a large number of records in a table, a single script may time out before the actions are completed. This is especially true for deletes. To avoid timing out the script, this solution will enable the action to be scheduled in batches with delays to avoid hanging the system for an extended operation.

## Any (i.e. Background) Script
```javascript
var objInputs = {
		"strTableName": "x_803922_demo_cmdb_widget",  // Which table?
		"strEncodedQuery": "nameLIKE34",			  // Which records?
		"intBatchSize": 100,	 					  // How many records at a time?
		"intBatchDelay": 3,						      // How many seconds delay to schedule the next batch
		"strLogPrefix": 'JD: ',						  // Used to prefix log entries
		"strFunction": "function( tableName, query ){ // Function to be executed on each record. 
			new global.GlideQuery.parse( tableName, query )
			.deleteMultiple();		  
		}"
    };

new ScheduleRecursion().runMe( JSON.stringify( objInputs ) );
```

## Script Include
```javascript
var ScheduledRecursion = Class.create();
ScheduledRecursion.prototype = {
    initialize: function( strInputs ) {},
    type: 'ScheduledRecursion',
	
	runMe: function( strInputs ){
		var objInputs = JSON.parse( strInputs );
		
		return createTrigger( strInputs );
		
	},
	
	doIt: function( strInputs ){

		try{

			objInputs = JSON.parse( strInputs );

			var totalRecordCount = new global.GlideQuery.parse( objInputs.strTableName, objInputs.strEncodedQuery ).count(); // Total records matching the query
			if( totalRecordCount == 0 ){ return null; }

			if( objInputs.intBatchCount == undefined ){
				objInputs.intBatchCount = 0;
				gs.info( objInputs.strLogPrefix + 'Starting to process ' + totalRecordCount + ' records from ' + 
						objInputs.strTableName + ' in batches of ' + objInputs.intBatchSize + ' records.\nFunction: ' + JSON.stringify( objInputs.strFunction ) );				
			}
			gs.info( objInputs.strLogPrefix + 'Batch #' + ++objInputs.intBatchCount + ', Processing ' + objInputs.intBatchSize < totalRecordCount ? objInputs.intBatchSize : totalRecordCount + 
				' of ' + totalRecordCount + ' remaining records.' );

			var batchIDs = [];
			var grBID = new GlideRecord( objInputs.strTableName );
			grBID.addEncodedQuery( objInputs.strEncodedQuery );
			grBID.setLimit( objInputs.intBatchSize );
			grBID.query();
			while( grBID.next() ){
				batchIDs.push( grBID.getUniqueValue() );
			}

			objInputs.strFunction( objInputs.strTableName, 'sys_idIN' + batchIDs )

			gs.info( objInputs.strLogPrefix + 'Batch #' + objInputs.intBatchCount + ' is complete.' );
			
			strInputs = JSON.stringify( objInputs );
			createTrigger( strInputs );
			
		}
		catch( e ){
			gs.error( 
				objInputs.strLogPrefix + 'An error occurred trying to process records from ' + objInputs.strTableName + 
				'\nERROR: ' + e.name + ': ' + e.message 
			);
		}

	},
	
	createTrigger: function( strInputs ){
		var objInputs = JSON.parse( strInputs ),
			intBatchNumber = ( objInputs.intBatchCount || 0 ) + 1,
			gdtNextAction = new GlideDateTime(),
			grTrigger = new GlideRecord( 'sys_trigger' );
		
		gdtNextAction.addSeconds( objInputs.intBatchDelay );
			
		grTrigger.initialize();
		grTrigger.setValue( 'name', 'MassRecordDeletes Batch #' + intBatchNumber);
		grTrigger.setValue( 'next_action', gdtNextAction );
		grTrigger.setValue( 'trigger_type', 0 ); // Run Once
		grTrigger.setValue( 'script', "new ScheduledRecursion().doIt( '" + strInputs + "' )" );
		
		return 'Trigger: ' + grTrigger.insert() + ': ' + gs.getProperty('glide.servlet.uri') + 'sys_trigger_list.do?nameSTARTSWITHMassRecordDeletes';
		
	},

};
```
Folder Name:

  - ./Script Includes/Scheduled Recursion
    - # Scheduled Recursion

To take action on a large number of records in a table, a single script may time out before the actions are completed. This is especially true for deletes. To avoid timing out the script, this solution will enable the action to be scheduled in batches with delays to avoid hanging the system for an extended operation.

## Any (i.e. Background) Script
```javascript
var objInputs = {
		"strTableName": "x_803922_demo_cmdb_widget",  // Which table?
		"strEncodedQuery": "nameLIKE34",			  // Which records?
		"intBatchSize": 100,	 					  // How many records at a time?
		"intBatchDelay": 3,						      // How many seconds delay to schedule the next batch
		"strLogPrefix": 'JD: ',						  // Used to prefix log entries
		"strFunction": "function( tableName, query ){ // Function to be executed on each record. 
			new global.GlideQuery.parse( tableName, query )
			.deleteMultiple();		  
		}"
    };

new ScheduleRecursion().runMe( JSON.stringify( objInputs ) );
```

## Script Include
```javascript
var ScheduledRecursion = Class.create();
ScheduledRecursion.prototype = {
    initialize: function( strInputs ) {},
    type: 'ScheduledRecursion',
	
	runMe: function( strInputs ){
		var objInputs = JSON.parse( strInputs );
		
		return createTrigger( strInputs );
		
	},
	
	doIt: function( strInputs ){

		try{

			objInputs = JSON.parse( strInputs );

			var totalRecordCount = new global.GlideQuery.parse( objInputs.strTableName, objInputs.strEncodedQuery ).count(); // Total records matching the query
			if( totalRecordCount == 0 ){ return null; }

			if( objInputs.intBatchCount == undefined ){
				objInputs.intBatchCount = 0;
				gs.info( objInputs.strLogPrefix + 'Starting to process ' + totalRecordCount + ' records from ' + 
						objInputs.strTableName + ' in batches of ' + objInputs.intBatchSize + ' records.\nFunction: ' + JSON.stringify( objInputs.strFunction ) );				
			}
			gs.info( objInputs.strLogPrefix + 'Batch #' + ++objInputs.intBatchCount + ', Processing ' + objInputs.intBatchSize < totalRecordCount ? objInputs.intBatchSize : totalRecordCount + 
				' of ' + totalRecordCount + ' remaining records.' );

			var batchIDs = [];
			var grBID = new GlideRecord( objInputs.strTableName );
			grBID.addEncodedQuery( objInputs.strEncodedQuery );
			grBID.setLimit( objInputs.intBatchSize );
			grBID.query();
			while( grBID.next() ){
				batchIDs.push( grBID.getUniqueValue() );
			}

			objInputs.strFunction( objInputs.strTableName, 'sys_idIN' + batchIDs )

			gs.info( objInputs.strLogPrefix + 'Batch #' + objInputs.intBatchCount + ' is complete.' );
			
			strInputs = JSON.stringify( objInputs );
			createTrigger( strInputs );
			
		}
		catch( e ){
			gs.error( 
				objInputs.strLogPrefix + 'An error occurred trying to process records from ' + objInputs.strTableName + 
				'\nERROR: ' + e.name + ': ' + e.message 
			);
		}

	},
	
	createTrigger: function( strInputs ){
		var objInputs = JSON.parse( strInputs ),
			intBatchNumber = ( objInputs.intBatchCount || 0 ) + 1,
			gdtNextAction = new GlideDateTime(),
			grTrigger = new GlideRecord( 'sys_trigger' );
		
		gdtNextAction.addSeconds( objInputs.intBatchDelay );
			
		grTrigger.initialize();
		grTrigger.setValue( 'name', 'MassRecordDeletes Batch #' + intBatchNumber);
		grTrigger.setValue( 'next_action', gdtNextAction );
		grTrigger.setValue( 'trigger_type', 0 ); // Run Once
		grTrigger.setValue( 'script', "new ScheduledRecursion().doIt( '" + strInputs + "' )" );
		
		return 'Trigger: ' + grTrigger.insert() + ': ' + gs.getProperty('glide.servlet.uri') + 'sys_trigger_list.do?nameSTARTSWITHMassRecordDeletes';
		
	},

};
```
Folder Name:

  - ./Script Includes/Project Base Line
    - 
Folder Name:

  - ./Script Includes/Store data in User Session
    - 
Folder Name:

  - ./Script Includes/ArrayUtil
    - ArrayUtil API is a script include with useful functions for working with JavaScript arrays.
The example shared helps removes duplicate items from an array using the 'unique' method
Folder Name:

  - ./Script Includes/SRAPIUtil
    - #SRAPIUtil

Utility class for common methods when implementing SRAPIs. Also includes examples of SNDocs and Revealing Module script include pattern with true private methods
Folder Name:

  - ./Script Includes/Check Valid Choice
    - Introduction :

This script include is a client callable script include which can be used to check if the value of a choice field is valid, optionally given a dependent value. This is helpful when you do transforms and when you want to do some validations in your REST inbound messages.

Inputs and Outputs :
     * @param {object} current - GlideRecord object containing the current record
     * @param {string} The name of the choice field
     * @returns {bool}         - Boolean indicating whether the value of a choice field is valid
Folder Name:

  - ./Script Includes/OrderedRecords
    - # ArtifactRank
Script Include that helps with getting the next spaced out ordering 

## Example Script
```javascript
var nextRank = new ArtifactRank.getNextRank();
```
Folder Name:

  - ./Script Includes/ListFieldUtil
    - # ListFieldUtil
Script Include that helps with handling list fields, like for example "Watch List" on the task table.

It doesn't use the typical `Class.create`, instead it is a simple javascript function.
Check out this blog post for more info about the "Function Pattern": https://codecreative.io/blog/interface-design-patterns-function-pattern/

## Example Script
```javascript
var watchListVal = grMyIncident.getValue("watch_list");
//add current user to watch list
var newWatchListVal = ListFieldUtil(watchListVal).add(gs.getUserID());
grMyIncident.setValue("watch_list", newWatchListVal);

//remove current user from watch list
var newWatchListVal = ListFieldUtil(watchListVal).remove(gs.getUserID());
grMyIncident.setValue("watch_list", newWatchListVal);

//check if current user exists in watch list
var currentUserInWatchList = ListFieldUtil(watchListVal).exists(gs.getUserID());
gs.debug("Current user is in watch list: " + currentUserInWatchList);
```
Folder Name:

  - ./Script Includes/TimeZoneUtils
    - # TimeZoneUtils
This Script Include is a tool for handling time-zones in ServiceNow. Specifically, this solves the problem of being unable to get a GlideDate/GlideDateTime object in a SPECIFIED time-zone, without having to get a user object for a user who's already in that specific time-zone.

## getGDT()
Get the GlideDateTime object (as a reference).

This will return a *reference* to the GlideDateTime object. Note that because of JavaScript's
pass-by-reference jive, you should expect that if you set a variable using this method, then
call another method which modifies the GDT object referenced in this class, you will be modifying
the object to which your variable is a reference! In other words, your variable will be modified *in-place*.

## setTZ(tz) / setTimeZone(tz)
Note that you can specify time-zones in a number of formats, like "US/Pacific",
"US\\Eastern", or by short name (such as "mountain").

Currently, this utility only understands a few time-zones by short name. You can print out a list of
pre-defined these supported short-names by printing out the keys in the timeZones property.

Example: gs.print(Object.keys(new TimeZoneUtils().timeZones));

You can reference any time-zone using the following (case-sensitive) format:

{Region}\{Zone}

Example: "Pacific\Guam", or "America\Puerto_Rico"

## getValue()
Gets the value of the current GlideDateTime object.

This will get the value in SYSTEM-time, so it will return the same value no matter which time-zone you've specified.

If the GDT's time value was set prior to passing it into TimeZoneUtils, this will return that date/time
in the specified time-zone.

## getDisplayValue()
Gets the display value of the current GlideDateTime object.

If a time-zone was specified by calling .setTimeZone(), this will return the time in that time-zone.

If the GDT's time value was set prior to passing it into TimeZoneUtils, this will return that date/time
in the specified time-zone.

### Example server-side call (background script)
```javascript
var bmr;
var argsArray = [
	{
		"some_object": {
			"some_object": {
				"some_object": {
					"some_number": 123,
					"some_string": "abc123",
					"some_boolean": 123,
					"some_null": null,
					"some_method": function() {
						return "some_string";
					}
				}
			}
		}
	}
];

argsArray.push(JSON.stringify(argsArray[0]));

/*
	argsArray[0] now contains the object, and argsArray[1] contains the
	 stringified object.
	We'll test whether it's faster to stringify an object, or to parse an
	 object string.
 */

bmr = new BenchmarkRunner()

bmr.printComparisonResults(
	bmr.compareFunctions(
		thingOne,
		thingTwo,
		20000,
		argsArray
	),
	20000
);

function thingOne(arrArgs) {
	var strObj = JSON.stringify(arrArgs[0]);
	return strObj;
}

function thingTwo(arrArgs) {
	var objObj = JSON.parse(arrArgs[1]);
	return objObj;
}
Folder Name:

  - ./Script Includes/Find months between two dates
    - # getMonths

Helper function that calculates total months between two specified dates e.g. total months between 2020-01-01 and
2022-01-01 is 24!

## Usage

```javascript
var helper = new DateUtils();

gs.log(helper.getMonths('2020-01-01', '2022-01-01')); // This returns 24
```
Folder Name:

  - ./Script Includes/JSONPath
    - # JSONPath Plus

Analyse, transform, and selectively extract data from JSON documents (and JavaScript objects).

jsonpath-plus expands on the original specification to add some additional operators and makes explicit some behaviors the original did not spell out.

You can try it within the [browser demo](https://jsonpath-plus.github.io/JSONPath/demo/)

## Features

- **Compliant** with the original jsonpath spec
- Convenient **additions or elaborations** not provided in the original spec:
  - `^` for grabbing the **parent** of a matching item
  - `~` for grabbing **property names** of matching items (as array)
  - **Type selectors** for obtaining:
    - Basic JSON types: `@null()`, `@boolean()`, `@number()`, `@string()`, `@array()`, `@object()`
    - `@integer()`
    - The compound type `@scalar()` (which also accepts `undefined` and
      non-finite numbers when querying JavaScript objects as well as all of the basic non-object/non-function types)
    - `@other()` usable in conjunction with a user-defined `otherTypeCallback`
    - Non-JSON types that can nevertheless be used when querying
      non-JSON JavaScript objects (`@undefined()`, `@function()`, `@nonFinite()`)
  - `@path`/`@parent`/`@property`/`@parentProperty`/`@root` **shorthand selectors** within filters
  - **Escaping**
    - `` ` `` for escaping remaining sequence
    - `@['...']`/`?@['...']` syntax for escaping special characters within
      property names in filters
  - Documents `$..` (**getting all parent components**)
- In addition to queried values, **can return various meta-information**
  including paths or pointers to the value, as well as the parent
  object and parent property name (to allow for modification).
- **Utilities for converting** between paths, arrays, and pointers
- Option to **prevent evaluations** permitted in the original spec or supply
  a **sandbox** for evaluated values.
- Option for **callback to handle results** as they are obtained.

## Setup

1. create a script include `JSONPath`
2. fill in the script field with the content of [JSONPath.js file](JSONPath.js)
3. you should now be able to call it via globally available function e.g. `JSONPath(path, json)`

## Usage

The full signature available is:

```
var result = JSONPath([options,] path, json, callback, otherTypeCallback);
```

The arguments `path`, `json`, `callback`, and `otherTypeCallback`
can alternatively be expressed (along with any other of the
available properties) on `options`.

Note that `result` will contain all items found (optionally
wrapped into an array) whereas `callback` can be used if you
wish to perform some operation as each item is discovered, with
the callback function being executed 0 to N times depending
on the number of independent items to be found in the result.
See the docs below for more on `JSONPath`'s available arguments.

See also the [API docs](https://jsonpath-plus.github.io/JSONPath/docs/ts/).

### Properties

The properties that can be supplied on the options object or
evaluate method (as the first argument) include:

- **_path_** (**required**) - The JSONPath expression as a (normalized
  or unnormalized) string or array
- **_json_** (**required**) - The JSON object to evaluate (whether of
  null, boolean, number, string, object, or array type).
- **_autostart_** (**default: true**) - If this is supplied as `false`,
  one may call the `evaluate` method manually.
- **_flatten_** (**default: false**) - Whether the returned array of results
  will be flattened to a single dimension array.
- **_resultType_** (**default: "value"**) - Can be case-insensitive form of
  "value", "path", "pointer", "parent", or "parentProperty" to determine
  respectively whether to return results as the values of the found items,
  as their absolute paths, as [JSON Pointers](https://tools.ietf.org/html/rfc6901)
  to the absolute paths, as their parent objects, or as their parent's
  property name. If set to "all", all of these types will be returned on
  an object with the type as key name.
- **_sandbox_** (**default: {}**) - Key-value map of variables to be
  available to code evaluations such as filtering expressions. (Note
  that the current path and value will also be available to those
  expressions; see the Syntax section for details.)
- **_wrap_** (**default: true**) - Whether or not to wrap the results
  in an array. If `wrap` is set to `false`, and no results are found,
  `undefined` will be returned (as opposed to an empty array when
  `wrap` is set to true). If `wrap` is set to `false` and a single
  non-array result is found, that result will be the only item returned
  (not within an array). An array will still be returned if multiple
  results are found, however. To avoid ambiguities (in the case where
  it is necessary to distinguish between a result which is a failure
  and one which is an empty array), it is recommended to switch the
  default to `false`.
- **_preventEval_** (**default: false**) - Although JavaScript evaluation
  expressions are allowed by default, for security reasons (if one is
  operating on untrusted user input, for example), one may wish to
  set this option to `true` to throw exceptions when these expressions
  are attempted.
- **_parent_** (**default: null**) - In the event that a query could be
  made to return the root node, this allows the parent of that root node
  to be returned within results.
- **_parentProperty_** (**default: null**) - In the event that a query
  could be made to return the root node, this allows the `parentProperty`
  of that root node to be returned within results.
- **_callback_** (**default: (none)**) - If supplied, a callback will be
  called immediately upon retrieval of an end point value. The three arguments
  supplied will be the value of the payload (according to `resultType`),
  the type of the payload (whether it is a normal "value" or a "property"
  name), and a full payload object (with all `resultType`s).
- **_otherTypeCallback_** (**default: \<A function that throws an error**
  **when @other() is encountered\>**) - In the current absence of JSON
  Schema support, one can determine types beyond the built-in types by
  adding the operator `@other()` at the end of one's query. If such a
  path is encountered, the `otherTypeCallback` will be invoked with the
  value of the item, its path, its parent, and its parent's property name,
  and it should return a boolean indicating whether the supplied value
  belongs to the "other" type or not (or it may handle transformations and
  return false).

### Instance methods

- **_evaluate(path, json, callback, otherTypeCallback)_** OR
  **_evaluate({path: \<path\>, json: \<json object\>, callback:_**
  **_\<callback function\>, otherTypeCallback:_**
  **_\<otherTypeCallback function\>})_** - This method is only
  necessary if the `autostart` property is set to `false`. It
  can be used for repeated evaluations using the same configuration.
  Besides the listed properties, the latter method pattern can
  accept any of the other allowed instance properties (except
  for `autostart` which would have no relevance here).

### Class properties and methods

- **_JSONPath.cache_** - Exposes the cache object for those who wish
  to preserve and reuse it for optimization purposes.
- **_JSONPath.toPathArray(pathAsString)_** - Accepts a normalized or
  unnormalized path as string and converts to an array: for
  example, `['$', 'aProperty', 'anotherProperty']`.
- **_JSONPath.toPathString(pathAsArray)_** - Accepts a path array and
  converts to a normalized path string. The string will be in a form
  like: `$['aProperty']['anotherProperty][0]`. The JSONPath terminal
  constructions `~` and `^` and type operators like `@string()` are
  silently stripped.
- **_JSONPath.toPointer(pathAsArray)_** - Accepts a path array and
  converts to a [JSON Pointer](https://tools.ietf.org/html/rfc6901).
  The string will be in a form like: `/aProperty/anotherProperty/0`
  (with any `~` and `/` internal characters escaped as per the JSON
  Pointer spec). The JSONPath terminal constructions `~` and `^` and
  type operators like `@string()` are silently stripped.

## Examples

Given the following JSON, taken from <http://goessner.net/articles/JsonPath/>:

```json
{
  "store": {
    "book": [
      {
        "category": "reference",
        "author": "Nigel Rees",
        "title": "Sayings of the Century",
        "price": 8.95
      },
      {
        "category": "fiction",
        "author": "Evelyn Waugh",
        "title": "Sword of Honour",
        "price": 12.99
      },
      {
        "category": "fiction",
        "author": "Herman Melville",
        "title": "Moby Dick",
        "isbn": "0-553-21311-3",
        "price": 8.99
      },
      {
        "category": "fiction",
        "author": "J. R. R. Tolkien",
        "title": "The Lord of the Rings",
        "isbn": "0-395-19395-8",
        "price": 22.99
      }
    ],
    "bicycle": {
      "color": "red",
      "price": 19.95
    }
  }
}
```

### Filter all books cheaper than 10

```javascript
var result = JSONPath("$..book[?(@.price<10)]", json);

// [
//   {
//     "category": "reference",
//     "author": "Nigel Rees",
//     "title": "Sayings of the Century",
//     "price": 8.95
//   },
//   {
//     "category": "fiction",
//     "author": "Herman Melville",
//     "title": "Moby Dick",
//     "isbn": "0-553-21311-3",
//     "price": 8.99
//   }
// ]
```

### Grab all authors

```javascript
var result = JSONPath("$..author", json);

// [
//   "Nigel Rees",
//   "Evelyn Waugh",
//   "Herman Melville",
//   "J. R. R. Tolkien"
// ]
```

More examples can be found [here](https://github.com/JSONPath-Plus/JSONPath/blob/main/README.md#syntax-through-examples)

## Credits

The code has been taken from [JSONPath-Plus repo](https://github.com/JSONPath-Plus/JSONPath) and slightly adjusted to be able to run on the platform JavaScript engine.
Folder Name:

  - ./Script Includes/getCountFunction
    - Introduction :

We have two script includes in here. Main aim for this is to have a generic count function which can be called from all server side scripts and you don’t have to write GlideAggregate every time. It is scripted in such a way that you can pass table name and query dynamically and get the count.

Script Include Significance :
1)	Code.js – This is the generic script include used to return the count of the table passed as parameters.
2)	callingSI.js – This script include shows how to call the code.js script include and how to pass the parameters to get the count dynamically.

Parameters in script include to be passed:
•	Table Name.
•	Query.
•	Sys Id which is mentioned as id in callingSI.js

Output:
Count of records matching the query.
Folder Name:

  - ./Script Includes/getCountFunction
    - Introduction :

We have two script includes in here. Main aim for this is to have a generic count function which can be called from all server side scripts and you don’t have to write GlideAggregate every time. It is scripted in such a way that you can pass table name and query dynamically and get the count.

Script Include Significance :
1)	Code.js – This is the generic script include used to return the count of the table passed as parameters.
2)	callingSI.js – This script include shows how to call the code.js script include and how to pass the parameters to get the count dynamically.

Parameters in script include to be passed:
•	Table Name.
•	Query.
•	Sys Id which is mentioned as id in callingSI.js

Output:
Count of records matching the query.
Folder Name:

  - ./Script Includes/Get Approvers of a Ticket
    - # Get Approvers of a Ticket

This script returns the number of approvers sys_id that are being requested for Approval
Folder Name:

  - ./Script Includes/get field values for multiple records from a table
    - ## Script contains scalable method to get display value of particular field from a table for any number of records filtered by a encoded query

> Method: \_getFieldDisplayValues(tableName, query, fieldName)

-   @param {String} tableName: Table name
-   @param {String} query: query to filter the records
-   @param {String} fieldName: Field name for which display value is required

-   @returns {String OR boolean}: comma separated field display values of filtered records
    **OR** false if no record/no display value if found on filtered records

### Example Methods

> getUserEmailAddressesBySysIDs(sysIDs)

-   @param {String} sysIDs: Comma separated list of sysIDs (can also be single sysID)
-   @returns {String}: comma separated email addresses of user profiles sys_id passed in as comma separated values.

> getUserNamesBySysIDs(sysIDs)

-   @param {String} sysIDs: Comma separated list of sysIDs (can also be single sysID)
-   @returns {String}: comma separated names of user profiles sys_id passed in as comma separated values.
Folder Name:

  - ./Script Includes/Non Prod Instance Password Reset
    - 
Folder Name:

  - ./Script Includes/Return Object
    - ## ReturnRecord Script Include
- The script include is client callable
- The returnRecordObject function allows for users to return a record values within the objects properties.
- In call back function, in client script, parse the object that is return, then dot walk to access its propery values.
Folder Name:

  - ./Script Includes/EvtMgmtCustom_PostTransformHandler
    - ## EvtMgmtCustom_PostTransformHandler Script Include

I came across a requirement where we wanted to a create a new alert/incident when the same event is encountered after a certain amount of time, even if the existing alert/incident are still open. OOTB if this is the case and same event comes into the system, it will go ahead and append it to the existing alert. 

So, I made the EvtMgmtCustom_PostTransformHandler as active and scripted the code as per my requirement, here I query for an existing event based on certain parameters(check script) and if a event is found, I calculate the difference between current time of event and previous time of event. If difference is more than desired limit, I apent the message key with time of event for new event before being processed as alert. This will create a new alert with the updated message key and create a new incident.

Note: This script is present in the system to make any changes to the alert which will be created out of this Event. The Event itself is immutable, and will not be changed in the database
Folder Name:

  - ./Script Includes/Extending OOB TableUtils
    - # Extending the baseline TableUtils Script Include

This code snippet extends the out of the box __Table Utils__ Script Include by adding a method to retrieve all fields -and the properties- of a given table. There is already a baseline API called _getFields()_ that does the same, but it required an existing GlideRecord to perform it. There are cases where we want the fields of a table without necessarily having a GlideRecord.

The code snippet also shows how to extend an existing class and how to invoke the parent class constructor to ensure proper behavior.

It is invoked like this:
```
new EXT_TableUtils(<table_name>).getFieldsAndAttributes();
```

So for example with the _incident_ table:
```
var fields = new EXT_TableUtils('incident').getFieldsAndAttributes();
for (var fieldName in fields) {
    gs.debug('Field ' + fieldName + ' is of type ' + fields[fieldName].field_type);
}
```

And returns a JSON structure of this format:
```
{
    <field_name_1>: {
        field_label: <label>,
        field_size: <size>,
        field_type: <type>,
        reference_table: <table> (only for reference or glide_list types)
    },
    <field_name_2>: {
        ...
    }
}
```
Folder Name:

  - ./Script Includes/GlideRecordHelper
    - Various functions for working with gliderecords, inspired by some of the methods available in the service portal with $sp. Functions have JSDoc documnetation for use.

@name getField
@description: Checks the specified field and returns an object.

@name getFields
@description: Checks the specified fields and returns an array of field objects.

@name getFieldsObject
@description: Checks the specified fields and returns an object of objects.

@name getFieldsObjectWithQuery
@description: Checks the specified fields and returns an object of objects with a specified filter

@name getFieldsObjectWithQueryAjax
@description: Client callable to get fields array of objects with query
Folder Name:

  - ./Script Includes/Custom Discovery Schedule With Freeze Periods
    - # Custom Discovery Schedule

One of the requirements we had from one of our client was that they didn't want discovery schedules to run for few days at the begining of the month (BOM) and few days for the end of the month (EOM) as they internally had to generate some big financial reports and didn't want discovery to take any network resources.

So this custom discovery script enables to run discovery on daily basis but will ignore the schedules if it was end of month or begining of the month as configured in system properties. There are 4 system properties that are attached as xml and needs to be imported into sys_properties.

This script submits the Pre-created discovery schedules (On Demand schedules) but it honours
pre-configured days to be skipped at the begining of the month and days at the end of the month.

It also honours the pre-configured times that discovery should be skipped.

### Configurations required

- Standard discovery schedules with Run (On Demand)
- The following sys_properties needs to be configured
    * VF.Discovery.BOM.DaysToFreeze
    * VF.Discovery.EOM.DaysToFreeze
    * VF.Discovery.Freeze.StartTime
    * VF.Discovery.Freeze.EndTime

Details of sys_properties are below:

| Name | Description  | Type  | Value |
| :-------------------------:   | :-: | :-: |  :-: |
| VF.Discovery.Freeze.StartTime | The start time that discovery will not be submitted. Should be in system date/time format e.g. 09:00:00 for 9 am | string | 08:00:00 |
| VF.Discovery.Freeze.EndTime | The end time that discovery will not be submitted. Should be in system date/time format e.g. 21:00:00 for 9 pm | string | 21:00:00 |
| VF.Discovery.EOM.DaysToFreeze | Number of days to freeze (skip) discovery at the end of month (EOM) | integer | 2 |
| VF.Discovery.BOM.DaysToFreeze | Number of days to freeze (skip) discovery at the begin of month (BOM) | integer | 3 |

## Usage

- Create the required sys_properties and set the values as per requirements
- Create a new schedule job that runs on daily basis
- Keep the Discovery schedules that you want to be submitted by this script to On Demand
- Include the following script in the schedule job script

```javascript

var helper = new VF_DiscoveryScheduleWithFreezePeriod(new GlideDateTime());
helper.process();

```
Folder Name:

  - ./Script Includes/BenchmarkRunner
    - # BenchmarkRunner
This Script Include is a tool for benchmarking individual functions, or comparing the execution time or two functions, to determine whether one method of doing something is faster than another, and by how much. 

For example (as you can see in the example below), comparing whether it's faster to *stringify* an object, or *parse* a JSON string into an object. 

## compareFunctions(methodOne, methodTwo, iterations, args)
Execute two functions with the specified arguments, and get info about which was faster
(and by how much).

## benchmarkSingleFunction(functionToBenchmark, iterations, args)
Benchmark a single function, and return information about how long it took for the specified number of iterations, and how long each iteration took on average. 

## Example server-side call (background script)
```javascript
var bmr;
var argsArray = [
	{
		"some_object": {
			"some_object": {
				"some_object": {
					"some_number": 123,
					"some_string": "abc123",
					"some_boolean": 123,
					"some_null": null,
					"some_method": function() {
						return "some_string";
					}
				}
			}
		}
	}
];

argsArray.push(JSON.stringify(argsArray[0]));

/*
	argsArray[0] now contains the object, and argsArray[1] contains the
	 stringified object.
	We'll test whether it's faster to stringify an object, or to parse an
	 object string.
 */

bmr = new BenchmarkRunner()

bmr.printComparisonResults(
	bmr.compareFunctions(
		thingOne,
		thingTwo,
		20000,
		argsArray
	),
	20000
);

function thingOne(arrArgs) {
	var strObj = JSON.stringify(arrArgs[0]);
	return strObj;
}

function thingTwo(arrArgs) {
	var objObj = JSON.parse(arrArgs[1]);
	return objObj;
}
Folder Name:

  - ./Script Includes/Number Padding
    - Lets you pad your single digit number for better formating
Folder Name:

  - ./Inbound Actions/Email Text as Attachment
    - # Save Email Text as Attachment

### Steps:

Navigate to System Definition \ Script Includes and click New.
Set the following values:<br />
**Name:** emailAsAttachmentUtil<br />
**Accessible from:** All application Scopes = this will allow it to be called by all applications<br />
**Active:** checked<br />
**Description:** You may want to set the description to something like the following to document what this script includes does and how to call it<br />

* [Click here for Script include script](script.js)

**Example of calling a script include from the Inbound action**
```js
//This utility script will take contents from an inbound email and create an attachment on the created record from the inbound email action.  To utilize this script, add the following lines at the end of the inbound email action script:
var emailAsAttachment = new global.emailAsAttachmentUtil();
emailAsAttachment.createAttachment(email, current);
```
Folder Name:

  - ./Inbound Actions/Automate creation of incidents through inbound actions
    - This is a simple code to automate creation of incidents for the alerts receiving to ServiceNow instance. This code has functionality of adding receipients (excluding service-now instance emails) of email to watchlist of incident.
Folder Name:

  - ./Inbound Actions/Advanced Scripts
    - ## These inbound action scripts will help you with the following:

### 1) Creation - Map values from an email to variables and create a requested item for the same.
Check with script -> create_catalog_item_from_email.js  

This script will help you map the values coming with the email body to variables of a catalog items and submit a catalog item. In this particular script we're submitting the request for user-offboarding by mapping the userID and termination date. So, in a similar way as per your requirement you can map/add variables from an email to submit an catalog item.

### 2) Updating - Check with already created requested item and update the variables and restart the workflow.
Check with script -> update_catalog_item_from_email.js

Now, Once you've successfully mapped the values and submitted an item from the email that first came into ServiceNow, there can be a case scenario where we need to update the termination date to a new value. This script will help you query the existing RITM for the user and update the value for termination date to the new values that came into the new email and restart the workflow. So, again as per your requirement in a similar way you can query the existing RITM and update variables coming in with an email and update the RITM.

### 3) Cancellation - Check with already created requested item and cancel the same also cancel the workflow.
Check with script -> cancel_catalog_item_from_email.js

Third Scenario, here is once a termination request is submitted, now we need to re-hire the candidate. So, in this case we need to cancel the RITM. 
This script will help you query the existing RITM for the user and cancel the RITM and all related tasks. So, as per your case scenario in a similar way you can query the existing RITM and cancel it with all the related catalog tasks.
Folder Name:

  - ./Inbound Actions/Advanced Scripts
    - ## These inbound action scripts will help you with the following:

### 1) Creation - Map values from an email to variables and create a requested item for the same.
Check with script -> create_catalog_item_from_email.js  

This script will help you map the values coming with the email body to variables of a catalog items and submit a catalog item. In this particular script we're submitting the request for user-offboarding by mapping the userID and termination date. So, in a similar way as per your requirement you can map/add variables from an email to submit an catalog item.

### 2) Updating - Check with already created requested item and update the variables and restart the workflow.
Check with script -> update_catalog_item_from_email.js

Now, Once you've successfully mapped the values and submitted an item from the email that first came into ServiceNow, there can be a case scenario where we need to update the termination date to a new value. This script will help you query the existing RITM for the user and update the value for termination date to the new values that came into the new email and restart the workflow. So, again as per your requirement in a similar way you can query the existing RITM and update variables coming in with an email and update the RITM.

### 3) Cancellation - Check with already created requested item and cancel the same also cancel the workflow.
Check with script -> cancel_catalog_item_from_email.js

Third Scenario, here is once a termination request is submitted, now we need to re-hire the candidate. So, in this case we need to cancel the RITM. 
This script will help you query the existing RITM for the user and cancel the RITM and all related tasks. So, as per your case scenario in a similar way you can query the existing RITM and cancel it with all the related catalog tasks.
Folder Name:

  - ./Inbound Actions/Advanced Scripts
    - ## These inbound action scripts will help you with the following:

### 1) Creation - Map values from an email to variables and create a requested item for the same.
Check with script -> create_catalog_item_from_email.js  

This script will help you map the values coming with the email body to variables of a catalog items and submit a catalog item. In this particular script we're submitting the request for user-offboarding by mapping the userID and termination date. So, in a similar way as per your requirement you can map/add variables from an email to submit an catalog item.

### 2) Updating - Check with already created requested item and update the variables and restart the workflow.
Check with script -> update_catalog_item_from_email.js

Now, Once you've successfully mapped the values and submitted an item from the email that first came into ServiceNow, there can be a case scenario where we need to update the termination date to a new value. This script will help you query the existing RITM for the user and update the value for termination date to the new values that came into the new email and restart the workflow. So, again as per your requirement in a similar way you can query the existing RITM and update variables coming in with an email and update the RITM.

### 3) Cancellation - Check with already created requested item and cancel the same also cancel the workflow.
Check with script -> cancel_catalog_item_from_email.js

Third Scenario, here is once a termination request is submitted, now we need to re-hire the candidate. So, in this case we need to cancel the RITM. 
This script will help you query the existing RITM for the user and cancel the RITM and all related tasks. So, as per your case scenario in a similar way you can query the existing RITM and cancel it with all the related catalog tasks.
Folder Name:

  - ./Inbound Actions/Auto Reply Email
    - There are use cases where it has been requested to setup an "auto reply" type process within ServiceNow

To accomplish this, you'll need to do 3 steps:
1) Create an event - https://docs.servicenow.com/bundle/rome-platform-administration/page/administer/platform-events/task/t_CreateYourOwnEvent.html
2) Create a notification - https://docs.servicenow.com/bundle/rome-servicenow-platform/page/administer/notification/task/t_CreateANotification.html:
- Click the "Advanced view" related link on the notification form
- Select the table associated to this process
- Set the "When to send" condition to send when "Event is fired"
- Select your event you created from step 1 within the "Event name" field
- Within the "Who will receive" tab, set the "Event parm 1 contains recipient" checkbox to true
- Within the "What it will contain" tab, set your subject/message, etc.
3) Create or edit an inbound action record to house the script within the code.js file from this code-snippet folder

Additional things to keep in mind is that this setup is recommended for an already established process/inbound action, so you can simply take the script from code.js and add it to your current script at the point where you'd like the email sent. If this is for a new inbound action, select the table that matches the table you set on the notification. You'll want to ensure that the "Execution order" field within the inbound action is set low enough number that this process will not be blocked by other inbound action that was evaluated before it and has its "Stop processing" checkbox set to true. For the inbound action you've created, also ensure the "Stop processing" checkbox is not checked if you require additional inbound actions to evaluate the inbound email and complete other actions.
Folder Name:

  - ./Client Scripts/Validate date is in future without GlideAjax
    - # Client Script - Date in future

A client script that validates that a specified date is in future without the need for a GlideAjax and Script Include

## Usage

- Create a new client script
- Set the type to OnChange
- Select a date field that you want to validate
- Navigate to the form and set the date field to the past
- There will be a validation error close to the field
Folder Name:

  - ./Client Scripts/Make Variable Editor Read Only for Catalog Items containing MRVS
    - # Make Variable Editor Read Only for Catalog Items which have a Multi Row Variable Set
Create an onLoad Client Script which would call a Script Include and pass in the Catalog Item sys_id to check if the Catalog Item contains a MRVS. The script has been tailored to work with the Requested Item table. To make it work for any other table which has the Variable Editor replace the field "cat_item" with the field containing the details of the Catalog Item
Folder Name:

  - ./Client Scripts/Make Variable Editor Read Only for Catalog Items containing MRVS
    - # Make Variable Editor Read Only for Catalog Items which have a Multi Row Variable Set
Create an onLoad Client Script which would call a Script Include and pass in the Catalog Item sys_id to check if the Catalog Item contains a MRVS. The script has been tailored to work with the Requested Item table. To make it work for any other table which has the Variable Editor replace the field "cat_item" with the field containing the details of the Catalog Item
Folder Name:

  - ./Client Scripts/End Date can't be before Start Date
    - This script is for an onChange client script

This is using an example where you have two date variables and need to ensure the user does not choose an end date that's before the start date

1. replace 'start_date' in the script with your actual start date field name
2. replace 'end_date' in the script with yoru actual start date field name
3. replace showFieldMsg and showErrorBox messages with your own message, if applicable

This script works for both the standard (desktop) UI and Service Portal
Folder Name:

  - ./Client Scripts/Make all fields read only
    - Use this script to make all fields readonly via client script.

**Tested in Global scope
**You can't make mandatory fields as readonly
**Best Practice is to use ACLs
Folder Name:

  - ./Client Scripts/g_form console access in workspace
    - # Access g_form instance inside Agent Workspace from DevTools Console
When developing forms in ServiceNow it can be useful to try stuff out directly in the DevTools Console.
In UI16 this was pretty straightforward because g_form was available globally, Agent Workspace makes this a little bit more complicated.
So this script provides access to the g_form object of the currently active tab in a Workspace.

Just copy the Script in the DevTools Console and run `var g_form = getGlideFormAW()` 
now you should be able to do stuff like `g_form.setValue("short_description", "Lorem ipsum")`
Folder Name:

  - ./Client Scripts/MRVS variables validations
    - Multi Row Variable Set (MRVS) variables validations which are based on variables out of MRVS

for this we need to use "g_service_catalog" client side API of ServiceNow

Example:
Requirement is like there is an adaptation leave form, where the user can take 30 leaves in batches not all at once. 
Users can enter the last working date which is a normal variable in catalog item and batched leaves in MRVS where the Extended leave start and end dates will populate.
We are restricting here only to enter extended leave start date after the last working date. 

![image](https://user-images.githubusercontent.com/46869542/193416763-27fb52c9-e15b-48b5-99fd-6c146a6819c3.png)
Folder Name:

  - ./Client Scripts/Check all mandatory fields using mandatoryCheck()
    - **Client Script**

Client script which is showing how to use g_form.mandatoryCheck() function, which allows to easily detect if any of mandatory field is not filled on record.

**Example configuration**

![Coniguration](ScreenShot_1.PNG)

**Example execution**

![Execution](ScreenShot_2.PNG)
Folder Name:

  - ./Client Scripts/Add Image to Field Based on Company
    - # Add Image to Field Based on Company
From the User Profile get the Company associated to the User using a Display Business Rule and putting the value in the scratchpad. After that use the scratchpad value in the Client Script to check the company name and then associate the image accordingly. You would need to add all your images to the ServiceNow instance first with the correct names.
Folder Name:

  - ./Client Scripts/Add Image to Field Based on Company
    - # Add Image to Field Based on Company
From the User Profile get the Company associated to the User using a Display Business Rule and putting the value in the scratchpad. After that use the scratchpad value in the Client Script to check the company name and then associate the image accordingly. You would need to add all your images to the ServiceNow instance first with the correct names.
Folder Name:

  - ./Client Scripts/Verify if e-mail already exists with Ajax call
    - **Client Script**

Client script for verification if changed e-mail adders on user record is not already existing in sys_user table (real-time information about duplicated e-mail). Check is performed using asynchronous Ajax call and processed in callback function. In case e-mail already exists in sys_user table, message is displayed under email field with information which has have that e-mail.

**How to use**

You need to prepare both Script Include (which is processing check on backed) and Client Script (which is sending Ajax call after change on email field and display message).

Example Script Include configuration (code in [scriptInclude.js](scriptInclude.js)):
![Coniguration_SI](ScreenShot_2.PNG)

Example Client Script configuration (code in [clientScript.js](clientScript.js)):
![Coniguration_CS](ScreenShot_1.PNG)

**Example effect of execution**

![Coniguration_SI](ScreenShot_3.PNG)
Folder Name:

  - ./Client Scripts/Verify if e-mail already exists with Ajax call
    - **Client Script**

Client script for verification if changed e-mail adders on user record is not already existing in sys_user table (real-time information about duplicated e-mail). Check is performed using asynchronous Ajax call and processed in callback function. In case e-mail already exists in sys_user table, message is displayed under email field with information which has have that e-mail.

**How to use**

You need to prepare both Script Include (which is processing check on backed) and Client Script (which is sending Ajax call after change on email field and display message).

Example Script Include configuration (code in [scriptInclude.js](scriptInclude.js)):
![Coniguration_SI](ScreenShot_2.PNG)

Example Client Script configuration (code in [clientScript.js](clientScript.js)):
![Coniguration_CS](ScreenShot_1.PNG)

**Example effect of execution**

![Coniguration_SI](ScreenShot_3.PNG)
Folder Name:

  - ./Client Scripts/Translate Message
    - # Translate your messages in client script using getMessage method

  *[getMessage() code snippet](getMessage.js)
  
  *[Translate message in client script doc](https://docs.servicenow.com/bundle/rome-platform-administration/page/administer/localization/task/t_TranslateAClientScriptMessage.html)
Folder Name:

  - ./Client Scripts/Make fields read only in specific states
    - 
Folder Name:

  - ./Client Scripts/Sync Ajax with no getXMLWait
    - # onSubmit Ajax validation with no getXMLWait

Using getXMLWait() ensures the order of execution, but can cause the application to seem unresponsive, significantly degrading the user experience of any application that uses it.

Also, the getXMLWait method is not available in scoped applications.

This snippet simulates the behavior of the getXMLWait method.
Folder Name:

  - ./Client Scripts/Auto-populate watch_list based on company
    - Table: Incident
Type: onChange
field: caller_id

Sometimes customers have a requirement to add users or distribution lists to all tickets that are raised for their company. This script allows to automatically add a list of users or external email addresses to the watch_list field.
Folder Name:

  - ./Client Scripts/Client script using getMessage() function without filling Messages field
    - # Client scripts using getMessage() function without filling Messages field

**Problem scenario :**
Developers while writing a client script uses getMessage() function but there are no messages preloaded in the 'Messages' field in client script form

**Solution :**
Write an onSubmit client script to check the above scenario and prevent client script submission with an error message on top of the form.

Check the file `script.js` file for example.

Note : As a best practice for this scenario use 'Checks' in the'Instance scan' feature of serviceNow. If Instance scan is not configured in your instance yet or if you want to avoid the problem during development itself then use this client script.
Folder Name:

  - ./Client Scripts/Get URL Parameters
    - # Get URL Parameters in Global,Scoped Application for Record & Catalog Item

Many times there is a need to grab parameters from URL. This could be required at table form load or catalog item load and either in Global scope or custom scope application when redirection happened. Given script will help you in achieving this:

[Click here for the script](script.js)
Folder Name:

  - ./Client Scripts/Populate Jelly Slushbucket with Values
    - This code is used to populate the <g:ui_slushbucket up_down="true"/> Jelly tag within a UI Page.

In the UI Page, must ensure that this tag is located in the HTML section.

Then in the client script, include the code provided in the example.
Folder Name:

  - ./Client Scripts/Get Value from URL Parameter
    - Script that can be used in Client scripts to get URL parameter value.

** Isolate script should be **false**
Folder Name:

  - ./Client Scripts/Show field if x things are checked
    - Use this script to show a field after `n` checkboxes are checked and not before.

**Tested in Global scope
**You can't make mandatory fields as readonly
**Best Practice is to use UI Policies
**Sometimes you have a lot of check marks and that logic gets narly
Folder Name:

  - ./Client Scripts/Only number validation for input
    - # Client Script - Input is number only

A client script that validates that the input entry is number only

## Usage


- Create a new client script
- Set the type to OnChange. Update the field in the client script to <your field name>
- Select a field field that you want to be number
- Navigate to the form and set the field to a string
- There will be a validation error close to the field
Folder Name:

  - ./Client Scripts/Hide Work Notes section
    - **Client Script**

Client Script for hiding work notes section on incident form. In this example it is configured to hide work notes section, when incident is in state new, but you can adjust condition to fit your requirements. 

**Example configuration of Client Script**

![Coniguration](ScreenShot_1.PNG)

**Example effect of execution**

When incident is in state NEW (Work notes section not visible):

![Not Visible](ScreenShot_2.PNG)

When incident is not in state NEW (Work notes section visible):

![Visible](ScreenShot_3.PNG)
Folder Name:

  - ./Client Scripts/Expanding Info Message
    - This is an expanding info message. It can even run a script when an element is clicked.
Folder Name:

  - ./Client Scripts/onfocus and onblur
    - Using "onfocus" & "onblur" Show/Hide field messages while updating a field.

Example:On load Client script on the incident form

![image](https://user-images.githubusercontent.com/42912180/195825979-e69e5798-a241-4fe8-8f49-7f70f1f3ae6e.png)



**Quick video how it works:**


https://user-images.githubusercontent.com/42912180/195825799-aff13ca5-0b85-4660-98a3-ea1af8b61974.mp4
Folder Name:

  - ./Client Scripts/Set field style like font and background
    - # Client Script - Change field style

A client script that changes field font, and background based on some condition
And example would be if the currently raised incident is by a VIP user and hightlight the caller...

## Usage

- Create a new OnLoad script
- Copy this script into it
- Set the condition and the field that requires to be changed
Folder Name:

  - ./Catalog Client Script/PopulateDropdown
    - ## Load / Populate the options for the second dropdown field (select box) based on what user chooses in the first dropdown
![alt text](demo_catalog.png)

### Use case

You need to dynamically populate the options for a dropdown (select box) field following another field.

For example, you need to create a catalog that has 2 fields: country and city, when the user chooses a country, the city field will only show the cities of that country.

This will especially come in handy when you have hundreds of options to populate, and easier to maintain than using catalog UI policies 👍

### Set up

- On the catalog, create 2 select box fields, for example: `city` and `country`
- Add the question choices for the 1st dropdown
- In the 2nd dropdwon, add any value for the question choices to bypass the mandatory
- Create new client script, on change, for the FIRST dropdown. Only applies on Catalog Item view. It is recommended to set the variables readonly on the RITM and SCTASK view.
Folder Name:

  - ./Catalog Client Script/Add Label For Attachment
    - 
Folder Name:

  - ./Catalog Client Script/Prevent duplicate records on MRVS
    - # Prevent duplicate records to be selected in Multi row variable set

We have many ways to do this but this is bit unique compare to what you find in community, you can do it in one single script within the Variable set. 
Of course ServiceNow introduce a new feature in Quebec and have Unique checkbox field introuduced but to have a custom info message you need to go with the custom script.

  [ServiceNow Docs to disallow duplicate values](https://docs.servicenow.com/bundle/quebec-servicenow-platform/page/product/service-catalog-management/task/t_CreateAVariableForACatalogItem.html)
  
  [Click here for the script](script.js)
Folder Name:

  - ./Catalog Client Script/Mandatory Attachments with 'n' numbers
    - # Enable Mandatory Attachments Count wtih 'n' numbers on Service Catalog item
**Problem:** Check if exact 'n' number of attachments are added or not when user submit a request through service catalog from Portal/Platform UI.

**For example:** We need to ensure there are exact 3 attachments added before submission

**Note:** Ensure Isolate Script field is set to False for this Catalog Client Script to ensure DOM manipulation works

* [Click here for script](onSubmitClientScript.js)
Folder Name:

  - ./Catalog Client Script/Set fields from URL Parameters
    - # Set fields on a catalog item from URL parameters.

This only works on both the classic ui and service portal.

To use this you must provide the technical name as a url parameter and then provide the value you would like set. This script is also console logging the techcnical names if you don't have them handy. Reference fields require using the sys_id.


### Example

For the OOTB Password Reset catalog item it has a field "Whose password needs to be reset?" with a technical value of "caller_id" after adding this script you could use the below url parameter to auto populate the form with Abel Tuter.

/sp?id=sc_cat_item&sys_id=29a39e830a0a0b27007d1e200ad52253&**caller_id=62826bf03710200044e0bfc8bcbe5df1**
Folder Name:

  - ./Catalog Client Script/Restrict Number of rows in Multi Row Variable
    - ## restrict_multi_row.js
Use this to restrict multi row variable set rows to 1. this value can be changed to any number of rows as requirement.
Folder Name:

  - ./Catalog Client Script/Block Submit
    - 
Folder Name:

  - ./Catalog Client Script/Currency Validation
    - ## Currency Validation 

Use this catalog client script to validate the value of a variable used to get currency. As of now 3 things are being checked in the script but you can make changes as per requirement.

1) Characters after the $ sign should be numerics.
2) Entered value should have a decimal point.
3) There must be 2 digits only after the decimal.
Folder Name:

  - ./Catalog Client Script/Date Management
    - #### Useful ways to interact with variable date/time values without needing to make a trip to the server

The following functions and variables are defined by ServiceNow and loaded at run-time. They are accessible from within the client script without the need to turn off script isolation.

- g_user_date_format
- g_user_date_time_format
- isDate()
- compareDates()
- formatDate()
- getDateFromFormat()
Folder Name:

  - ./Catalog Client Script/Make OOB Attachment Mandatory
    - # Make out of the box attahcment mandatory onChange of a field in Catalog Item

This scripts makes the out of the box attachments to mandatory on the Service Portal for any Catalog Item.

Usage:

Step #1 - Create the UI Script 
* [Click here for script](UI Scripts/Make OOB Attachment Mandatory/setAttachmentMandatory.js)

Step #2 - Include the UI Script in the Portal Theme under JS Includes

Step #3 - Create a Catalog Client Script for the respective Catalog Item where you want to make the OOB attachment mandatory for certain criteria

* [Click here for script](Catalog Client Script/Make OOB Attachment Mandatory/onChange.js)
Folder Name:

  - ./Catalog Client Script/Remove reference icon from portal
    - 
Folder Name:

  - ./Catalog Client Script/Combine variables into Description
    - OnSUbmit Catalog Client script is created to Combine all variable values required and display in Description field.
Steps:
1. Navigate to your instance open catalog client script table [catalog_script_client]
2. Create new catalog client script -> click new
3. Provide following values:
      - Name: Any relevant to your script
      - Applies to: A catalog Item
      - UI Type: All
      - Isolated script: checked
      - Application: Application scope applies to
      - Type: onSubmit
      - Catalog item: select your catalog item
 4. create the script as per script.js file.  
Folder Name:

  - ./Catalog Client Script/Control all RITM variables in one go
    - # Control all RITM variables in one go

Requirement : We need to make all the variables on the RITM (sc_req_item) form read only or editable

Problem : If there are so many variables then it becomes difficult to write multiple UI policies or writing multiple lines of code in catalog client script for each variable seperately.

Solution : With the above code snippet you can control(make read-only or editable) all the variables in the RITM form with very minimal code)
Folder Name:

  - ./Catalog Client Script/Autopopulate Department
    - # Autopopulate Department Catalog Client Script

Use this onChange catalog client script to populate a **department** variable in a catalog item based on a modifiable **requested_for**. Both variables must be reference type pointing to their respective tables.

## Use case

The GlideUser API (g_user) does not provide a way to retrieve a user's department in a client-side script. Here is a small snippet using `g_form.getReference()` to retrieve the user from the **requested_for** variable and populate the **department** variable in a catalog item while allowing the submitter to still change the department if the data is incorrect.

Attach this client script to a variable set for easy reuse. It can be augmented with a number of other fields from the user record such as email, phone number, manager, etc. Just be mindful of field types and whether the desired field will return a sys_id or display text.
Folder Name:

  - ./Catalog Client Script/Special Characters
    - # Validate Special Characters for a catalog variable

With this onChange catalog client script you can validate if there are any special characters present in the input given by user in a particular field and show an error message below the field and clear the field value. Although we have other methods to do this, it is much easier and you can customize your error message.
Folder Name:

  - ./Catalog Client Script/Regex Validation
    - # Regular Expression on Catalog Client script
  
With the help of this code you can easily validate the input value from the user and if it's not a email format you can clear and throw a error message below the variable. Of course you can use Email type variable as well but you cannot have a formatted error message.

* [Click here for script](script.js)
Folder Name:

  - ./Catalog Client Script/Rounding Money or Price Field
    - This script is OnChange, and will automatically round the selected field to [x] value.
The script can either be applied to a Catalog Item, or a specific Variable in a Var Set.

For example, if prompting a user for a cost, and said cost should only be in multiples of $5.

Any instance of `[VAR NAME]` in these files should be replaced with the name of the variable that the script is being applied to.

More information and a full write-up available on [Community](https://community.servicenow.com/community?id=community_article&sys_id=75ab01271bac5d10c17111751a4bcb40).
Folder Name:

  - ./Catalog Client Script/MRVS Interact With Parent Form
    - Use this code snippet to interact with the parent form (i.e the main catalogue item) from within a catalog client script on a Multi-row variable set.

The g_service_catalog object allows for accessing the "parent" GlideForm (g_form) object and its related functions
Folder Name:

  - ./Catalog Client Script/Clear all fields
    - # Clear all fields on a catalog item form

This works on both the native platform and service portal / mobile. Typically used with an OnChange catalog client script when you would like to reset all the fields after a certain variable is changed.

This function does support an exclusion list if there are fields you would like to exclude from being reset, typically you would want to add the field that triggered to the change to the exlusion

### Example

```js
clearFields(['field1', 'field2']);
```

All fields on the form **except** field1 and field2 will be cleared.
Folder Name:

  - ./Catalog Client Script/MRVS Loop Rows
    - Use this to loop through a Multi Row Variable Set and create an array of objects with the variables in it.
Folder Name:

  - ./Catalog Client Script/Set User Field Values on Load
    - On Load Catalog client script is created to auto set the field values and make that field read only
 - Navigate to your instance -> App Navigator > Open Catalog CLient Script [catalog_script_client]
 - Set following field Values
        - Name: xyz
        - Applies to: A Catalog item
        - Type: onLoad
        - Catalog item: Select your Catalog item
        - UI Type: All
        - Isolated script: Checked
  -  Create the script as per script.js file.
Folder Name:

  - ./GlideElement/getDependent
    - GlideElement API provides different functions to work with the fields, attribute, values, etc.,
getDependent function on GlideElement API - helpful in validating the dependent field values if any for the given field. 

Used subcategory field in incident table as an example so that it will print "category" as result.
If we update the field_name variable to some other field that is not dependent on another field then the method prints null as result.

Link to documentation - https://developer.servicenow.com/dev.do#!/reference/api/paris/server_legacy/c_GlideElementAPI#r_GlideElement-getDependent
Folder Name:

  - ./GlideElement/Display available choices
    - 
Folder Name:

  - ./Advanced Conditions/Exclude Email Reply Comment Notifications by Group
    - # Exclude Email Replies from Comment Notifications based on Group Membership

### This is an advanced condition script for new comment notifications that will exclude new comments that are email replies for specific groups.  

Step 1.
Specify the user field such as assigned_to, caller_id, or opened_by, etc in the line of code below:

```js 
var groupMember = current.getValue('assigned_to'); //get value of the desired field
```

Step 2.
Specify the group name such as Service Desk, Network Team, or CAB Approvers etc in the line of code below:

```js
if (groupMember.isMemberOf('Special Group')) { //check if membership is true
```
Folder Name:

  - ./Advanced Conditions/Group Approval Check
    - # Group Approval Check

### This is an email notification advanced condition script for approval requests that will check if an approval has already been granted prior to sending out a request.

This script can be applied to any approval request notification on the sysapproval_approver table with no additional configuration necessary
Folder Name:

  - ./MIDServer/API Class Examples
    - # MIDServer class samples

* Description: Usage samples for the MIDServer API class.
* [MIDServer Code Snippet](scripts.js)
* [MIDServer API Doc](https://developer.servicenow.com/dev.do#!/reference/api/rome/server_legacy/c_MIDServerAPI)
Folder Name:

  - ./Flow Actions/Check MID Server Availability
    - ## Action Script to check mid server availability

### Use this script in a new flow action to check if a mid server is up/available or not. This can be used to for orchestration projects or similar. 
### Note: The script returns availability as true/false back as the action output to the flow.
Folder Name:

  - ./Flow Actions/Scheduled data import trigger
    - This action script will execute the scheduled import via a flow action.

Inputs are  - 'importSet'  - the sys_id of the scheduled import set  - mandatory

Outputs are - 'returnerror'- true if no import set found             - mandatory

We found this useful when triggering a data import from a catalog item. User attaches the import file to catalog item and submit, which triggers flow, which then
had this action to import the file using the right import set.
Folder Name:

  - ./Flow Actions/get Catalog Variables as JSON
    - Get catalog variables from a given RITM
Folder Name:

  - ./Flow Actions/Runscript activities
    - This code help to set the RITM description as the summary of catalog item variables.
we can reuse the code on catalog workflows in runscript activity and flow designers
Folder Name:

  - ./Flow Actions/Get Property
    - Flow Action to return the value of a sys_properties

Action requires:
- One string input for sys_properties name
- Script Step (provided in getPropertyFlowAction.js)
- One string output for returned value
Folder Name:

  - ./Flow Actions/Trigger event action
    - Useful for tasks like triggering notifications or to trigger asynchronous script actions from a flow. 

This flow action triggers the passed in event with optional parameters. Will work for most scenarios as the event record is passed in as a Document ID input.

Inputs:

event_name		- Reference.Event Record - Mandatory

event_record	- Document ID            - Mandatory

parm1					- String 

parm2					- String
Folder Name:

  - ./Fix scripts/Swiss German Language Update
    - # Swiss German Language Update

This Fix Script replaces all "ß" special characters generated by the German language plugin (com.snc.i18n.german). 
In Swiss German, this character does not exist and must be replaced with "ss". Currently, unfortunately, there is no dedicated Swiss German language plugin available. 

### Instruction

As a prerequisite the "regular" German language plugin (com.snc.i18n.german) must be installed. 
After that the Fix Script can be executed, replacing the German special charactrer "ß" in the following relevant language tables with "ss": 
sys_translated, sys_ui_message, sys_documentation, sys_choice and sys_translated_text. 
I would recommend to run the Fix Script in the background, since the execution might take some time. 


### Benefits

- Quick fix to automatically replace all customer/end user visible special characters "ß" 
Folder Name:

  - ./Fix scripts/Fiscal period renamer
    - OOTB the Fiscal periods are named as such - "FY21: M01". This naming convention relies on each and every user knowing what M01 is (i.e. does the fiscal year start in January or does it start in March). This renaming script will append a descriptor to the end of each fiscal period name to increase usability and to preserve numeric sorting. Assuming M01 is January, the renamed fiscal period might be - "FY21: M01 Jan".

The fiscal period generator also assumes a hard-coded convention for the FYXX component of the name. Many customers differ from this and require it in the format FY23-24 if a fiscal year stretches across two calendar years. This script will allow manual selection of the 'from' year component (i.e. if FY is FY23 and stretches from July 2022 to June 2023 the FY will be renamed FY22-23:).

Instructions:
1. Update the fpQuery variable to be an encoded query that represents the fiscal periods you wish to rename
2. Update the orderedMonth variable to represent the descriptor to append to each period name. These must be in the order required for the fiscal year created.
3. Update the startAdditionalYear variable - this will prepend the financial year value with this value (i.e. change FY21 to FY20-21). This will increment for each FY so input the first value required.
4. Update the fiscalPeriodRecordsPerYear variable - this is the number of fiscal period records you've created per fiscal year - this is typically 17. Increment this value by one and input (i.e. I'd input 18 if I had 17 records)
5. Run the script and confirm the log statements are correct
6. Uncomment row 83 and run again to commit output of step 5
Folder Name:

  - ./Fix scripts/Post-clone Email Properties Script
    - # Post-clone script for email properties

To be used as a fix script or background script, meant to help with small adjustments needed per-environment after a clone.

Notes: Make sure you fill in all of the instance names up top, with anything in your instance name before the [.service-now.com]

This makes sure your email properties are disabled.
Folder Name:

  - ./Fix scripts/Cancel Workflow
    - Script to Cancel the workflow context attached to a record
Folder Name:

  - ./Fix scripts/Find duplicate records
    - # Find duplicate records

Run the script to find duplicate records in a table. It is using GlideAggregate to find duplicate records. Replace the TABLE_TO_FIND_DUPLICATE_IN and FIELD_TO_GROUP_BY constants with your table and field and it will spit the records.
Folder Name:

  - ./Fix scripts/Post-clone Set Banner Name
    - # Post-clone script for email properties

To be used as a fix script or background script, meant to help with small adjustments needed per-environment after a clone.

Notes: Make sure you fill in all of the instance names up top, with anything in your instance name before the [.service-now.com]

This sets the banner description (that appears at the top of the instance) to the instance name and the date/time of the last clone. Helps keep users of that sub-prod instance informed of when the last clone date/time.
Folder Name:

  - ./Fix scripts/Assign user list to a specific group
    - **Fix Script**

Script to *automatically assign a list of users to a specific group*; you can change the user query to prepare a correct list of users according to your needs. To assign a different group, change the value of the GROUP_ID variable to the sys_id of the group which you would like to assign. 

**Example configuration of Fix Script**

![Configuration](ScreenShot_1.PNG)

**Example execution logs**

![Logs](ScreenShot_2.PNG)
Folder Name:

  - ./Fix scripts/Multiply records from filer breadcrumbs
    - ## Multiply records from filer breadcrumbs

Using this script you can multiply records (such as Story, Incident, SCTASK, ...), while assigning them to a different user. 
The script will also copy the attachments to the duplicate record.

I use this script to create sample stories / incidents for our new joiners that they can practice on in a non productive instance.
Folder Name:

  - ./Fix scripts/Install Demo Data
    - Add demo data to a list of installed plugins. I use this to add demo data for the OOTB ATF tests to work in sub-prod instances. It is expected that the corresponding ATF Test plugins are installed on the production instance already, and we are only adding the demo data.
Folder Name:

  - ./Fix scripts/Delete Duplicate Mobile records
    - Below script is a Fix script used to delete duplicate mobile assets and Cis in your CMDB. In this script we keep recently created assets and its related CI and delete other duplicate assets and related Cis if any.

Note : In this script I have used u_alm_mobile as the table and u_cmdb_ci_mobile, this are my tables but you can use your own table where you have stored your mobile devices.
Folder Name:

  - ./Fix scripts/Post-clone Set Instance Banner
    - # Set a unique banner to your non-production instance to help users realise where they are :)
 ## Can be used as clean-up script on a clone profile, or run as fix script, background script etc. manually on the target instance after cloning.


 ### Prerequisites:
 * 1) You need to have the target instance's banner image attached to a record on the source system, e.g. have a knowledge article in production with the banner attached to it.
 * 2) Make sure the table above mentioned table and record and included in your clone!
 * 3) Set the source table name and the source record's sys_id as values for srcTbl and srcRec variables in the below section!
Folder Name:

  - ./Fix scripts/Delete Change Conflict
    - Use this script to delete change Conflicts and set conflict status as 'No Conflict' using fix script.
Folder Name:

  - ./Fix scripts/Add Fields On All List Views
    - # Add Fields On All List Views

This will add Updated On, Updated By, Created on, and Created by to every list view for the current user. You can add or remove fields to fieldsToAdd if you want others added as well
Folder Name:

  - ./Fix scripts/Ignore outbound emails
    - 
Folder Name:

  - ./Fix scripts/Log out active User sessions
    - 
Folder Name:

  - ./Fix scripts/Adjust Variable Order on Catalog Item
    - # Adjust Variable Order on Catalog Item

This Fix Script helps developers to automatically re-order all variables of a given Catalog Item or Variable Set.  
We all know the struggle, that initially we set up variables with fixed order steps such as: 100, 200, 300, 400    
However, over time, additional variables are inserted in between, resulting in a messy looking order, e.g.: 10, 15, 50, 55, 100, 200, 350, 300, 400   
This fix script should enable developers to keep their Catalog Items clean and structured, with minimal effort.   

### Instruction

At the beginning of the script you have to set the Sys ID of the Catalog Item or Variable Set where you want to re-order the variables.
The Script is built in a way, that this Sys ID can belong to either a Variable Set or Catalog Item.
Furthermore, you have to define the step size for the order. My recommendation would be to use 100.
 
```javascript
var sys_id = "e0ecd03947e29110d3c0c789826d4332"; //provide a catalog item or variable set sys id
var step_size = 100; //provide the step size for the new order
```

### Benefits

- Keep Catalog Items and Variable Sets clean and structured
- Reduce efforts maintaining variable orders
Folder Name:

  - ./Fix scripts/Restart Flow (CatalogItem)
    - # Restart a Catalog Item Flow

To be used as a fix script or background script to restart a flow for a catalog item or selection of catalog items.  Typically this might be used in a scenarion in which you've modified a Flow and need to ensure that existing items are running the current version of the flow.

Note: This will RESTART your flows from the beginning.  So if your item is in progress you may see some undesirable behavior.  Also keep in mind any notifications you may have set to fire from the Flow.
Folder Name:

  - ./Fix scripts/Copy favourite to other users
    - You can use this script to take an existing favaourite from the sys_ui_bookmark table and create a copy of it for any number of users.
Can be useful when onboarding new staff, doing testing, etc.

You will need two things to get started:
* the sys_id of the original favourite you want to copy - take this from sys_ui_bookmark table
* an ecoded query string of a filtered list of users that you want to copy the favourite to

Run the script wherever you like, background script, Xplore, or as fix script.
Have fun!
Folder Name:

  - ./Fix scripts/Add Variable set to multiple catalog items
    - 
Folder Name:

  - ./Fix scripts/deleteMultiple
    - This script is recommended to be used (with caution) when it's necessary to delete multiple records from a table.

deleteMultiple is considerably faster than deleteRecord

As stated in the script, it's important to limit the amount of records being processed by this script at a time and never test this on Production without doing so on Development first
Folder Name:

  - ./Fix scripts/Merge stages or choice
    - 
Folder Name:

  - ./Fix scripts/Measure code time execution
    - **Fix Script**

Script which is showing how to *measure time execution of specific part of code*. You can use it to check performance of code or track time execution of part of code in Fix Scripts. You can add any amount of measuring parts, based of your needs.

**Example configuration of Fix Script**

![Coniguration](ScreenShot_1.PNG)

**Example execution logs**

![Logs](ScreenShot_2.PNG)
Folder Name:

  - ./Fix scripts/Clean update set
    - **Fix script**

Fix Script for cleaning update set from customer updates made by a selected developer. Script can be adjusted to match different query for cleaning which fits your needs.

Cleaning customer updates from update set is not removing updates made in system on direct records! It is just removing customer updates from update set to not move it to forward environments. 

**Example configuration of Fix Script**

![Coniguration](ScreenShot_3.PNG)

**Example execution logs**

![Logs](ScreenShot_4.PNG)

**Example effect of execution**

Before execution:
![Before](ScreenShot_1.PNG)

After execution:
![After](ScreenShot_2.PNG)
Folder Name:

  - ./Fix scripts/Search Results Weight
    - # Find the weight of Search Results

The order in which search results are returned is based on the weight of the object against the searched value.  This script can be run as a background script to determine what results are returned for specific search results and what their weight is in the search.

This can be used to determine why one item might returned in front of another item.
Folder Name:

  - ./Fix scripts/De-Provision Admin user (configurable)
    - Objective:

The purpose of this standalone fix script is to routinize the common sysadmin task of stripping admin access from an account. The de-provisioning process is going to be different for every organization, but it is often useful to have a repeatable, predictable technical solution for literally stripping an account of its rights in the event of an organizational change or security incident.

Note that fix scripts are typically intended to be associated with things that need to be done after an application is installed or upgraded, and it might not be considered 'best practice' to use a fix script for a one-time administrative task such as this, particularly one that is not really very difficult to perform by way of form action. Again, the goal for storing a script object like this on the instance is to have a repeatable, easily examined technical solution for completing the task, but if that is a desired thing to have it might be better to migrate this code into a UI Action associated with the Users table. Having it as a fix script is simply a convenient, low-impact solution.

Usage:

As written the script is designed to be updated once for each use. Modify the variables at the top of the script to meet the needs of the current de-provisioning event. Clicking on the 'Proceed' choice when running this has a fix script will provide some informative output.

'target' is the user ID the Users table account record to be de-provisioned

'admin_roles' lists all of the roles to be considered in scope for the script. If the deprovision_level variable is set to 2 (as described below) these will be the only roles stripped from the account.

'deprov_level' sets the depth of the de-provisioning activity, and the comments describe valid value. This variable is included in order to make the script flexible enough to be used for a range of sysadmin tasks, from simply reviewing what level of access the account has to completing stripping it of all roles and groups. Note that this script is not designed to delete an account record.

'deprov_result_msg' includes the text that will be written to the system log (and outputted when running the fix script interactively)
Folder Name:

  - ./Fix scripts/Fix model names after enabling glide.cmdb_model.display_name.shorten
    - There is a property that enables de-duplication of Manufacturer/Publisher Names from Model records (property name: [glide.cmdb_model.display_name.shorten](https://docs.servicenow.com/bundle/rome-it-service-management/page/product/asset-management/concept/c_InstalledWithModelManagement.html#r_ModelManagementProperties "glide.cmdb_model.display_name.shorten")). If this property is not active and users enter the Manufacturer/Publisher name into the Model Name field the Manufacturer/Publisher name will show twice in the Display Name.

<div style="padding-left: 2em;">

For example,  
**Manufacturer/Publisher Name:** Microsoft  
**Model Name:** Microsoft Word  
**Display Name with Property FALSE:** <span style="color: #ff0000;">Microsoft Microsoft Word</span>  
**Display Name with Property TRUE:** <span style="color: #008000;">Microsoft Word</span>

</div>

Once this property is activated, inserts/updates of Model records will trigger the business rule to recalculate the Display Name when one of the following fields is updated: Manufacturer/Publisher, Name, Version, Edition, Platform, Language. If you activate this property AFTER many models have been loaded, you may need to run a fix script to retroactively clean the existing Model Display Names.

The script below can be run as a Fix Script or as a Background Script. Normally, I would `setWorkflow(false)` for this kind of cleanup, but there are a few cascade Business Rules that need to run as this fix is implemented.
Folder Name:

  - ./Fix scripts/Install Base PDI Plugins
    - 
Folder Name:

  - ./Fix scripts/Post-clone Clear Email Queue
    - # Post-clone script for email properties

To be used as a fix script or background script, meant to help with small adjustments needed per-environment after a clone.

Notes: Make sure you fill in all of the instance names up top, with anything in your instance name before the [.service-now.com]

This clears out the email queue.
Folder Name:

  - ./Fix scripts/Update field with value in sys_audit
    - Hopefully this is something you never need to use.   It will udpate with either the newest or oldest entry from sys_audit.

## Example

```Javscript
var updateArgs = {
    encodedQuery: 'u_some_cool_field=blahblahblahL',
    table: 'my_cool_table',
    updateField: 'field to update in target table',
    auditField: 'field name in sys_audit',
    sort: 'DESC'
}


try {

    gs.print(updateRecords(updateArgs).join('\n'));
} catch (ex) {
    gs.error(ex.message || ex);
}

```
Folder Name:

  - ./Fix scripts/Anonymise Data
    - **Script Include** 

Script for anonymising data in specified table and chosen fields. You can pass an additional query to limit records which will be cleared. It can be used for example to remove GDPR data from development instances or anonymise old records. It can be used for example in fix script or scheduled job for long-term cleaning. 

**How to execute**

```javascript
//Table name which should be cleared
var table = 'sys_user';

//List of fields from table specified before
var fieldList = ['first_name', 'last_name'];

//Additional query
var query = 'user_nameSTARTSWITHTEST';

var anonymise = new AnonymiseData();
anonymise.anonymiseTable(table, fieldList, query, true);
```

You need to pass 4 parameters to function anonymiseTable

1. tablename - Name of table to be cleared ex. 'sys_user'
2. fieldList - Array of fields name, which should be cleared ex. ['first_name', 'last_name']
3. additionalQuery - Additional encoded query to limit list of records (if you would like to clear whole table just pass empty string)
4. logging - True/False value to determine if logging should be performed during execution

Example of Fix script execution:
 ![Coniguration](ScreenShot_2.PNG)

**Example configuration of Script Include** 

 ![Coniguration](ScreenShot_1.PNG)
 
**Execution logs**

 ![Coniguration](ScreenShot_3.PNG)

**Effect of execution**

 ![Coniguration](ScreenShot_4.PNG)
Folder Name:

  - ./GlideDateTime/Get Next Monday Date
    - 
# A Date Function to get the next upcoming Monday date.

This function uses a few Glide date and Glide Date Time API's 

1. First we get todays date with GlideDateTime()

2. Then we get the day of the month number with GlideDate().getDayOfMonthNoTZ();

3. Then we use the make a calculation to set the day to the next monday

4. Finally, we calcualtate the day using AddDays we return the New Date transforming it back with getDate()
Folder Name:

  - ./GlideDateTime/Due date generation
    - For the workflows created using flow designer, the due date for sctasks is not populated automatically.
This code populates the due date of sctask automatically when RITMs are created through flow designers.
Folder Name:

  - ./GlideDateTime/Current Date with Fixed Time
    - This script helps to set fixed time to Present Date..
Folder Name:

  - ./GlideDateTime/Set time zone and date format to output string dates
    - # Set time zone and date format to output dates.
Examples
```javascript
// Set time zone and date format to output string dates.
// Current time "2021-10-23 16:29:08" JST +0900
var gDateTime = new GlideDateTime();  
var calendar = Packages.java.util.Calendar.getInstance();
//Import dates in milliseconds
calendar.setTimeInMillis(gDateTime.getNumericValue());
//Java Date Object
var javaobjDate = calendar.getTime();

// Set the date format you want to output.
var simpleDateFormat = new Packages.java.text.SimpleDateFormat("EEEE,MMMM dd,yyyy HH:mm:ss z Z");
// Time zone string for current user ("Japan")
var strTz = gs.getSession().getTimeZoneName();
// Java TimeZone Object
var javaobjTz = Packages.java.util.TimeZone.getTimeZone(strTz);
// Set TimeZone
simpleDateFormat.setTimeZone(javaobjTz);
// Convert and date output
var strDate = '' + simpleDateFormat.format(javaobjDate);
// Output "Saturday,October 23,2021 16:29:08 JST +0900"
gs.info(strDate);
```

### Similar Functions: GlideDate.getByFormat()
Output in UTC, not in the time zone set by the user.

Examples
```javascript
// Current time "2021-10-23 17:03:56" JST +0900
var gd = new GlideDate();
// Time zone string for current user ("Japan")
var strTz = gs.getSession().getTimeZoneName();
var javaobjTz = Packages.java.util.TimeZone.getTimeZone(strTz);
gd.setTZ(javaobjTz);
gs.info( gd.getByFormat("EEEE,MMMM dd,yyyy HH:mm:ss z Z") );
// "Saturday,October 23,2021 08:03:56 UTC +0000"
// Output in UTC, not in the time zone set by the user.
```
Folder Name:

  - ./GlideDateTime/Check if today is weekend
    - Use this script to know whether today is weekend or weekday.

It helps to restrict the schedule job/ any other activity during weekends.
Folder Name:

  - ./GlideDateTime/Start, End, and Duration Updates
    - # Start, End, and Duration Updates
### Use this code to auto update associated GlideDateTime and Duration fields on a record.

This code assumes you're working on the sc_req_item and sc_task tables but can be modified to support other tables such as change.
1. Requires only a 2 of the 3 data points to work.  In this example, the start and duration variables are the required input.
2. Code checks for either a blank end time or if start or duration has changed. 
3. If start or duration has changed, it will calculate a new effective end date and duration accordingly.
4. If the end date is the one changing, it will calculate a new effective duration.
5. If all 3 data points change at the same time, only the start and duration fields will be accepted as input.  
6. It also includes a section to update an associated task if needed.
Folder Name:

  - ./GlideDateTime/AddDays
    - 
Folder Name:

  - ./GlideDateTime/Convert date format
    - # Convert date format

**Use-case / Requirement :**
Convert date from one format to another format
For example from dd-mm-yyyy to yyyy-mm-dd or yyyy/mm/dd etc

**Solution :**
Use GlideDate object and getByFormat method for conversion.
Check the script.js file to find the code
Folder Name:

  - ./Business Rules/Display current user display name on top of form
    - **Use case :**
 Display info message with current user display name on top of a form
 
 **Soulution :**
 Write a "Display business rule" on any table using `GlideSystem - getUserDisplayName()` API <br/>
 Check script.js file for example
Folder Name:

  - ./Business Rules/Create a copy of incident in another servicenow instance
    - # Create incident copy

**Use case** : Whenever a new incident is created in servicenow production instance, a copy of that incident should be created in backup instance.

*info* : This method is to achieve the above use-case just with business rule and without creating a record in sys_rest_message table.

**Solution** : Create a `After` business rule on incident table with `insert` checkbox checked. Follow the script present in [script.js](script.js) 
Folder Name:

  - ./Business Rules/Preserve enhancement when deleting project
    - Stops the related enhancement records being cascade deleted from a project record when they also belong to a demand (i.e. we're deleting the project, but want to re-evaluate the original demand with it's associated enhancements). IF you want all enhancements to be preserved then just adjust the filter conditions to suit.

Table: pm_project

When: before

Delete: true

Filter: Demand is not empty AND Demand is not ""
Folder Name:

  - ./Business Rules/Create comment on referenced record
    - **Business Rule**

 Script which allows adding comments to referenced records after some insert or update was made. In this example, after changing name on a Configuration Item, all incident which have that Ci  assigned will get comment about that change. You can change the script to different table, query and conditions to fit your needs.

 **Example configuration of  Business Rule** 

![Coniguration](ScreenShot_1.PNG)

**Example effect of execution**

![Effect](ScreenShot_2.PNG)
Folder Name:

  - ./Business Rules/Assign specific role to user
    - **Business Rule**

Script to *automatically assign* a *specific role* on creation or update of users, with additional protection against duplication of roles. You can run that Business Rules based on your needs (on user creation or on update when specific field was changed). To assign different role, copy sys_id of chose role into ROLE_ID variable.

**Example configuration of Business Rule**
![Configuration](ScreenShot1.PNG)

**Example execution effect**
![Execution](ScreenShot2.PNG)
Folder Name:

  - ./Business Rules/Enforce Percentage
    - # Objective
A Business Entity has multiple owners who are individuals. 
Each indivisual owns a percentage of the business.
This business rule insures that the total of all ownership percentage does not exceed 100%.

# Challenge
The aggregate function calculates the sum by using the values that are stored in the database. However we need to calculate the sum using the values that are in the database for all owners and use the value that the user is trying to update for the owner that is currently being udpated.

# Solution
1. Use the sum function from the [Calculator Script Include](https://github.com/ServiceNowDevProgram/code-snippets/tree/main/Script%20Includes/Calculator).
2. Calculate the sum using the values in the database
3. Substract the previous value and then add the current value to calculate what the future sum would be
Folder Name:

  - ./Business Rules/Recursive logic
    - Using this Recursive BR, when you select the CMDB CI on incident then it would automatically add all level of affected CIs and when you change the new cmdb_ci then its corresponding affected CIs will get added and old affected CIs will get deleted.
Folder Name:

  - ./Business Rules/DeleteUserRole
    - Bussienss Rule to delete the User Role from table like 'Service Category User Roles [service_category_user_role]'
Steps:
 - Navigate to your instance 
 - Open Business Rule Table [sys_script] and click on New
 - Create After BR and provide below condition
 - When to Run
        - AFter
        - Order: 100
        - Operation: Delete
  - Provide the condition as:
   !current.user_role.nil()
  - Select Advance option and use the script
Folder Name:

  - ./Business Rules/QueryBR-restrict users to see their company records
    - This script is used to restrict logged in users to see only their company records. This is a generic script and can be used in any table where there is a Company field present
which is associated to the User table.
Query BR contains below specifications:
1. Advanced = true
2. When = Before
3. Query = true
Folder Name:

  - ./Business Rules/Copy worknotes from SCTASK to RITM comments
    - 
Folder Name:

  - ./Business Rules/Update Child Incident based on Parent Incident
    - 
Folder Name:

  - ./Business Rules/Set program business duration
    - OOTB the project records exclude weekends and public holidays when calculating the duration, whereas program does not exclude these things. 

This business rule and associated script include address this issue and ensure that the duration field on the program record are calculated in the same way as projects.
Folder Name:

  - ./Business Rules/Set program business duration
    - OOTB the project records exclude weekends and public holidays when calculating the duration, whereas program does not exclude these things. 

This business rule and associated script include address this issue and ensure that the duration field on the program record are calculated in the same way as projects.
Folder Name:

  - ./Business Rules/Add itil role to ootb user query to also see inactive users
    - A common request is to also allow itil users to also be able to see inactive user records.
There are two pieces of code in the code.js file:
1) A conditional piece of code that should be added to the "Condition" field within the business rule
2) A single line that should be added to the "Script" field within the business rule
Folder Name:

  - ./Business Rules/Count Associated Incidents in Problem
    - <h2> Count the number of associated incidents in Problem Form </h2>
<h3>Use - Case: </h3>
<h4>Created a field in the Problem form which shows the number of incident records associated with the same problem. This makes it easy for the helpdesk to find out if there are any linked incidents without scrolling down.</h4>
Folder Name:

  - ./Business Rules/Exclude Redundant Email Recipients
    - # Exclude Redundant Email Recipients
### This business rule is designed to intercept new comment notifications and modify the recipients to mitigate redundant notifications in response to email replies that users were previously included on as a direct or copied recipient.

Initial Settings (modify as needed for your purposes)
- Table: sys_email
- Advanced: true
- When: before
- Insert: true
- Update: true
- Conditions:
  - Type > changes to > send-ready
  - Subject > contains > comment
Folder Name:

  - ./Business Rules/Prevent RITM to get closed
    - This is a code snippet which can be used in a Business rule to prevent the closure of RITM when there is any active catalog task attached to that RITM.
Below are the conditions of Business rule mostly suited.
When: Before
Update: True

Note: This script is helpful for all the tables and their related tables. It can work same way by editing the table names for other parent child ralations as well.
Folder Name:

  - ./Business Rules/Manipulating system properties values
    - **Business Rule**

Script which allows *getting value of specific system property and manipulate these values*. In this example, true/false property is got to determine if script should be executed. Then value of system property which is keeping last created user which gets 'admin' role is updated.

**Create new system property**

Before you can get or manipulate custom system property you need to create it in [sys_properties] table. Below you can see example of created property:

![Creating System Property](ScreenShot_0.PNG)

**Example configuration of Business Rule**

![Configuration](ScreenShot_1.PNG)

**Example execution effect**


![Execution effect](ScreenShot_2.PNG)
Folder Name:

  - ./Business Rules/Create choice sets if required for new choices
    - Type: Business Rule
When: Before
Insert: true

This script checks whether there is a choice set already created/available for the table:element pairing of a new sys_choice.
If there is, it returns without doing anything.
If there is not, it creates the choice set. This prevents the DELETE behaviour that occurs when a new choice is created that doesn't have a valid choice set available to be associated to.
Folder Name:

  - ./Business Rules/Randomly distrubite events between custom queues
    - 
Folder Name:

  - ./Business Rules/Transform Data from Attachment
    - 
Folder Name:

  - ./Business Rules/Copy Attachment INC to Case
    - 
Folder Name:

  - ./Business Rules/Display BR to get groupInfo of logged in User
    - This code snippet will help you to make fields read only/hide if a the logged in user belongs to a specific group.
To achieve this, we need to create a display Business rule and an onLoad client script.
Display BR will look for the group of logged in user and return true or false in a scratchpad variable.
Client script will validate the value and make the field read only/hide.
Folder Name:

  - ./Business Rules/Display BR to get groupInfo of logged in User
    - This code snippet will help you to make fields read only/hide if a the logged in user belongs to a specific group.
To achieve this, we need to create a display Business rule and an onLoad client script.
Display BR will look for the group of logged in user and return true or false in a scratchpad variable.
Client script will validate the value and make the field read only/hide.
Folder Name:

  - ./Business Rules/getMyDirectReports
    - This looping script traverses the User table from a certain point to get either one level of employees or all employees in the hierarchy underneath the logged on user. There are two functions:
* getMyDirectReports: gets only users directly connected to the User sys_id that is passed in
* getMyReports: gets all of the users underneath the the User sys_id that is passed in

This script is implemented as a Global Business rule and two Dynamic Filter records.
* Admins can use the script as a Reference Qualifier
* End Users can select the predefined filter in lists and reports (just like they can with "One of My Assignments").

There is some recursion protection, in that the script check to see if we've already collected the User before we go try to get their direct reports.

I have also included an XML file that will create the business rule and two dynamic filters for you.

Recommended values for the Dynamic filters if you should choose to create them on your own:

Dynamic Filter Option (sys_filter_option_dynamic)
* Label: One of My Direct Reports
* Script: getMyDirectReports()
* Field Type: Reference
* Reference Table: User (sys_user)
* Order: 500
* Reference script: Business Rule: getMyDirectReports
* Available for filter: true
* Available for ref qual: true

Dynamic Filter Option (sys_filter_option_dynamic)
* Label: One of My Reports
* Script: getMyReports()
* Field Type: Reference
* Reference Table: User (sys_user)
* Order: 600
* Reference script: Business Rule: getMyDirectReports
* Available for filter: true
* Available for ref qual: true

Use of this script could have performance impacts for very large organizations. Use at your own discretion.
Folder Name:

  - ./Business Rules/Change Lead Time Calculations
    - Before business rule runs on insert/update - you can set the conditions as you require. Script in change_lead_time_calculations.js

System property name:change.leadtime.values | type:string | value -> { "High": 5, "Moderate" : 3, "Low" : 1 } 
Folder Name:

  - ./Business Rules/Mandatory Attachment
    - 
Folder Name:

  - ./Business Rules/Auto add email recipients to the message body when Email Override is on
    - A common complaint I hear about testing email is that people don’t know who was actually supposed to receive emails when the override is on ([glide.email.test.user](https://docs.servicenow.com/bundle/rome-servicenow-platform/page/administer/reference-pages/reference/r_OutboundMailConfiguration.html) property).

The included business rule takes the intended recipients information and puts it in the body of the email at the bottom as shown below. This information can be used by testers to validate that emails would have been sent to the correct recipients.

*****
Email override is on. All outbound emails are currently sent to: bob.atherton@example.com, ccarter@example.com</br>
Original Intended Recipients:</br>
TO: Ray.Hatch@example.com,Ron.deGuzman@example.com,Glen.Traasdahl@example.com</br>
CC: Cherdell.Singleton@example.com,Ruthe.Aggarwal@example.com</br>
BCC: Morgan.Avery@example.com</br>
*****

If there aren’t any CC or BCC recipients those lines will be omitted respectively.

The business rule checks to see if the override is on, so it’s ok to have in a production instance because it won’t apply once they remove the override value.
Folder Name:

  - ./Business Rules/Copy attachments from idea to demand
    - Code will copy attachments from idea to demand

Name: Copy attachments to demand

Table: Idea

When: Async

Filter conditions: demand changes and demand is not empty

Update: true
Folder Name:

  - ./Business Rules/Copy latest comment from RITM to SCTASK
    - This simple snap code helps to copy latest comment of RITM to SCTASK.
Folder Name:

  - ./Business Rules/Make Attachment Mandatory
    - This simple code snippet will help in making attachments mandotary.
Can be used in Before BR/Script Inculde.
Folder Name:

  - ./Business Rules/Prevent invalid fiscal period in cost plan breakdown
    - Simple business rule that will ensure a cost plan breakdowns fiscal period will remain within the start and end period of the parent cost plan. If a cost plan breakdown is added ousdide of the start/end fiscal periods then rollups do not work correctly.
Folder Name:

  - ./Business Rules/setting future week dates
    - So the script "setting future week dates" is used to set a date field on a record to a future value and use that to trigger reminders to end users
or external customers. 

The script addresses the use case where the first reminder is expected to be sent 14 days from case create and the rest of the reminders every 3 days, and should be sent only on weekdays.

If the future computed date falls on a Sat 2 days are added, and if it falls on a Sunday 1 day is added.

Using this process a flow can be run each day to scan all the case records that have a notification date for the current day and a notification be sent
to the case contact.
Folder Name:

  - ./Business Rules/Previous Approval Check
    - # Previous Approval Check
### Business rule to check for any approval requests by previous approvers and auto approve them.  If an approver had already approved a request, and is later asked to approve the same request again, usually in a different capacity, then the approval will be set as approved by the system automatically. 

Business rule settings:
- Table: sc_req_item
- Advanced: True (Checked)
- When: async
- Order: 1000
- Insert: False (Unchecked)
- Update: True (Checked)
- Delete: False
- Query: True
- Conditions: 
  - Approval is Requested
  - Approval history changes

![image](https://user-images.githubusercontent.com/25243029/136676161-0a842f97-0721-4f28-8b20-a83f52bed949.png)
Folder Name:

  - ./Business Rules/Name Change Profile Update
    - This business rule is being used to update the live_profile record for a user if their first or last name changes. 
When a sys_user record is updated it runs a query against the live_profile table to match the document field with the sys ID of the user and then updates the name
field of the live_profile record with the name value from the sys_user record.	
Folder Name:

  - ./Business Rules/SCTASK_to_RITM
    - 
Folder Name:

  - ./Business Rules/Allow only unique insert
    - Before Business rule to check for existing entry in a table , incase one would want to make an insert to be unique based on a certain criteria.
Folder Name:

  - ./Business Rules/Enforce a 1-1 relationship
    - # Enforce a 1:1 relationship between two tables

ServiceNow does not provide a direct means of establishing a one-to-one relationship between two tables. Even so, you can enforce a 1:1 relationship with a remote table using business rules.
When the local reference field is changed, add the current record reference to the new remote record if applicable and remove the current record reference from the old/previous remote record if applicable.  

NOTE: Don't forget to:  
    1) Add this BR to both local and remote tables and   
    2) Swap the local and remote field names on the opposing table.  

NOTE: The table names are not required as they are defined by the table on which this BR runs and the table defined in the reference field.  

Attribution: This function is adapted from the example described in Tim "@TheProfessor" Woodruff's book "Learning ServiceNow (Second Edition)" available from Pakt Publishing.  
  

## Business Rule
When: BEFORE INSERT or UPDATE
Advanced Script:
```javascript
( function( current, previous /*null when async*/ ) {

    var remote_record,
        local_field_name = 'u_my_local_field',
        remote_field_name = 'u_the_remote_field';

    // Set the reference on the current remote record.
    if ( !current[ local_field_name ].nil() ){
        remote_record = current[ local_field_name ].getRefRecord();
        remote_record.setValue( remote_field_name, current.getUniqueValue() );
        remote_record.update();
    }

    // Clear the reference on the previous remote record.
    if ( !previous[ local_field_name ].nil() ) {
        remote_record = previous[ local_field_name ].getRefRecord();
        remote_record.setValue( remote_field_name, '' );
        remote_record.update();
    }
    
} )( current, previous );
Folder Name:

  - ./Business Rules/Pass server info to client
    - This BR can be used to pass any server information to the client side using the g_scratchpad variable.

BR Type:  Display business rule

Usage Scenario: We want to apply some logic based
    - on some property value stored at the server side.
    - on the department/manager associated with the user.

 
Folder Name:

  - ./Business Rules/Copy fields from Employee from
    - ## Copy response from Employee form to Specific cases/tasks/records

> This BR script can be used when auto field mapping feature on Employee forms is not fitting your requirements

### Usage scenarios

-   There are multiple Active employee forms associated with a single user at a time
-   Form field to be copied to different cases/tasks/records

### Implementation Guideline

-   Field name on employee form should be same as the field name on the record you want to copy. This is to avoid hard coding of field names/mappings in code and would help to scale the script for any employee form.

ex:

-   Case field name: u_employee_name, Employee form field name: u_employee_name

### Important Note

When a same survey (Employee form) is to be generated for a user who is already assigned to same employee form, then instead of creating new survey instance, OOB, system attaches/associates the existing active survey to the HR tasks. Update the below mentioned business rule to fix this issue.

**BR Name**: Create survey instance

**TODO**: Replace OOB code on line 9 with below code.

```JS

(function executeRule(current, previous /*null when async*/) {

	if(!current.survey || current.survey != previous.survey)
		if(current.survey_instance) {
			current.survey_instance.state = 'canceled';
		}

	if (current.survey)
		current.survey_instance = (new sn_assessment_core.AssessmentCreation()).createOrGetAssessment(current.survey, "", current.assigned_to);
})(current, previous);

```
Folder Name:

  - ./Business Rules/Generate event
    - **Business Rule**

Script to *generate new custom event*, which can be used on any conditions, on insert/update/delete of a record. In this example Business Rule is configured to generate custom event when any user get 'admin' role. 

**Event Registration**

Before you can generate custom event from script, you need to add Event Registration record *(sysevent_register table)*. Example Event Registration configuration:
![Event Registration](ScreenShot_0.PNG)


**Example configuration of Business Rule**

![Coniguration](ScreenShot_1.PNG)

**Example execution effect**

![Event Log](ScreenShot_2.PNG)
Folder Name:

  - ./Business Rules/Enforce Unique Rank
    - Before Business rule for keeping a rank field unique.

Conditions: current.rank.changes() && !current.rank.nil()
Folder Name:

  - ./Business Rules/Async REST Call
    - 
Folder Name:

  - ./Business Rules/Check domain of record against user session
    - Type: Business Rule
When: onDisplay
example Table: sys_script

This script gets the domain of the user session, and the domain of the record that you call it from, such as an onLoad Client Script.
Help to prevent accidental inserts of scripts in the wrong domain
eg:
Table: sys_script

function onLoad() {
	var currentUserDomain = g_scratchpad.currentDomain;
	var currentRecordDomain = g_scratchpad.recordDomain;
	
	if (currentUserDomain == 'Global') {
		g_form.addErrorMessage('You are currently in the Global domain. Editing this record won\'t create another record');
	} else if (currentUserDomain == currentRecordDomain) {
		g_form.addErrorMessage('You are currently in the same domain as the record you are about to edit: ' +currentUserDomain);
	} else {
		g_form.addErrorMessage('Your current domain is: ' +g_scratchpad.currentDomain +', and the record you are editing is in the ' +g_scratchpad.recordDomain +' domain. If you save any edits, the action will create a new record in your current domain');
	}
}
Folder Name:

  - ./Business Rules/After-BR to generate approvals for catalog tasks
    - This code snippet will help you to generate approvals for catalog tasks via scripting. You just need to create an after insert BR and put this script there.
This script can be used in a workflow run script as well and you can modify the script a little bit and use it for other tables as well. 

Fun fact: When you are playing with Document Id type field. You need to keep a field as dependent for the document ID like we have 'Source table' for 'Approving' field to put the correct table name there and with the help of that you can easily set the document ID field.

For e.g. dependent field name is u_table_name, so your script can be something like below:

- obj.u_table_name = 'Name of the table for your document ID type field';
- obj.u_document_id = 'Sys_id of the correct record from above table';
- obj.update();

where 'obj' is an object of the record you are referring to.
Folder Name:

  - ./Business Rules/ReRank item
    - Business rule for on after to re-rank a field spaced by 10 in each entry
it updates itself and any larger numbered rank item to keep them all in sync
Folder Name:

  - ./Business Rules/Prevent adding user to group if manager is inactive
    - 
# Prevent adding user to group

**Use case** : Whenever any user is getting added to any group, if the group manager is inactive then it should prevent the adding of user to the group

*info* : This method is to achieve the above use-case just with business rule

**Solution** : Create a `Before` business rule on `sys_user_grmember` table with `insert` checkbox checked. Follow the script present in [Script.js](https://github.com/ServiceNowDevProgram/code-snippets/blob/main/Business%20Rules/Prevent%20adding%20user%20to%20group%20if%20manager%20is%20inactive/Script.js)
Folder Name:

  - ./Business Rules/RoleUpdateOnGroupManagerChange
    - This business rule will update the group manager role on group manager change on Insert, Update, Delete
Steps:
  1. When new manager is updated from for the current group
  2. Current role of the manager will be updated and removed
  3. New Manager detail provided will be validated and it will assign the role to new manager 
  4. Configuration Details:
    - When to run:
        - After
        - Order:100
        - Operation: Insert, Update, Delete
     - Condition:
          current.manager.changes() || current.operation() == "delete"
     - Table: Group [sys_user_group]
Folder Name:

  - ./Business Rules/Block Attachments for specific conditions
    - This code is used to block attachments for a specific record condition (assignment group, state, etc)
Folder Name:

  - ./Business Rules/RITM_to_SCTASK
    - 
Folder Name:

  - ./Business Rules/Sync CI operational status with child related CIs
    - 
# Sync CI operational status with child related CIs

**Use case** : Whenever any configuration item becomes operational or non-operational, then all the CIs which are related to the current CI as a child in cmdb_rel_ci table will also update their operational status

*info* : This method is to achieve the above use-case just with business rule

**Solution** : Create a `Async` business rule on `cmdb_ci` table with `update` checkbox checked. 

*condition* : operational status CHANGES

Follow the script present in [script.js](https://github.com/ServiceNowDevProgram/code-snippets/blob/patch-1/Business%20Rules/Sync%20CI%20operational%20status%20with%20child%20related%20CIs/script.js)
Folder Name:

  - ./Business Rules/Copy Comments from RITM to SCTASK Vice versa
    - 
Folder Name:

  - ./Business Rules/Create catalog task for each row of MRVS
    - This code snippet will help you to generate tasks automatically for each row of MRVS present on RITM. This can be achieved by using a Before BR on RITM.
Specifications for Business rule will be:
1. When = Before
2. Insert = true
3. Advanced = true
4. Then write the script provided in script.js into the script section of BR.
Folder Name:

  - ./GlideRecord/Find No Of Days
    - This code will let you find the date difference between the provided dates: Helps in calculating No of days, payment processing , etc.
Folder Name:

  - ./GlideRecord/LEFT Join
    - 
Folder Name:

  - ./GlideRecord/LEFT Join
    - 
Folder Name:

  - ./GlideRecord/Fetch groups that have no members in them
    - This is script is useful in listing out the groups that do not have any members. You can use it before setting any group record/s as inactive. 
Folder Name:

  - ./GlideRecord/Multi Row Variable Set(MRVS)
    - This piece of code will let you insert MRVS Records without quering the Question Answers out of the box table!
Folder Name:

  - ./GlideRecord/UpdateMultiple
    - 
Folder Name:

  - ./GlideRecord/Find Date Overlapping
    - Logic to check if new dates are falling between already created record's dates.
Folder Name:

  - ./GlideRecord/Gets the display value according to the specified language
    - Get the display value according to the specified language.

(Install Language Plugin)

```javascript
var gr = new GlideRecord("incident");
gr.setLimit(1);
gr.query();
gr.next();
var user = gs.getUser();
var lang = user.getPreference("user.language");

// Japanese
user.setPreference("user.language", 'ja');
var outputJA = '' + gr.state.getLabel() + ' = ' + gr.state.getDisplayValue();
// English
user.setPreference("user.language", 'en');
var outputEN = '' + gr.state.getLabel() + ' = ' + gr.state.getDisplayValue();
gs.info(outputJA + ' / ' + outputEN);

user.setPreference("user.language", lang);
```
Folder Name:

  - ./GlideRecord/Get all user's group based on username
    - Get all user's group based on username

Just add replace the **userid** with the correct username in script
Folder Name:

  - ./GlideRecord/Get all task records with at least on active child task
    - 
Folder Name:

  - ./GlideRecord/getEncodedQuery
    - 1.In any GlideRecord query retrieve query using getEncodedQuery()

2.Apply this encoded query to create/update records (you can apply this query to other tables if query is appropriate).

![image](https://user-images.githubusercontent.com/42912180/195796801-4758afd0-4c35-4405-9836-560c6041dd4a.png)




Before Running the script :
![image](https://user-images.githubusercontent.com/42912180/195796529-cad998a9-c97e-40d7-b2b0-7bb48aaecf9a.png)


After Running the script:
![image](https://user-images.githubusercontent.com/42912180/195796411-dcb20d99-2bd7-4ef6-88bc-846f46006122.png)
Folder Name:

  - ./GlideRecord/GlideRecord with Performance Enhancement Condtions
    - A sample GlideRecord code with conditions to enhance performance.
Folder Name:

  - ./GlideRecord/Get Reference Record
    - 
Folder Name:

  - ./GlideRecord/findDuplicate
    - 
Folder Name:

  - ./GlideRecord/Get-task-containing-sensitive-data
    - This script is used to get all task records based on sensitive data entered into this task based records. To make it simple to add the criteria for GDPR or sentive data i 
have created a property and used it in this line : getProperty.addQuery('name', 'nn.criticalDataPhrases');

Example: 
Property name : criteria.gdpr
Value: BSN,Burgerservicenummer,voornaam,achternaam,geslacht,gender,Geboortedatum,Birth,adres,woonplaats,straatnaam,huisnummer,postcode,telefoonnummer,mobiel,hypotheeknummer,IBAN,Rekeningnummer,Rekeningnr,Rek. nr.,Verzekeringsnummer,verzekeringsnr,wachtwoord,gebruikersnaam,username,password,pwd

Output:
Task sys_ids which contains GDPR data.

Usage:
In scripted reports, in script includes,etc.
Folder Name:

  - ./GlideRecord/ACL enforcement using GlideRecord
    - 
Folder Name:

  - ./GlideRecord/Count Records By Column
    - 
Folder Name:

  - ./GlideRecord/Watch_List_functions
    - This code snippet is to help you remove a specific element/sys_id from a List or an array using javascript. This code can be run via any server side scripting.
For eg:
1. Background scripting
2. Fix script
3. BR
4. ScriptInclude etc.
Folder Name:

  - ./GlideRecord/Set Template
    - This function is useful in applying template on tables when creating new record using scripts.
Folder Name:

  - ./GlideRecord/Get all users whose email is empty
    - # Get all users without email

Use the script in script.js file to get the list of all users in sys_user table who do not have an email.
This GlideRecord script can be used in multiple places. For example in background scripts.

### Did some optimization in the code
1. Used different variable name instead of gr to reference a GlideRecord object.
2. Used addActiveQuery() method to filter out just the active records.
3. Used getDisplayValue() method to push string values in the array instead of using dot notation.
4. Used self executing function to wrap the code in a function for reducing variable scoping issues.
Folder Name:

  - ./GlideFilter/checkRecord
    - Ever wondered how business rule works in the background. This example depicts the common scenario where we want to analyse certain records against a certain condition. This is one of the OOB class provided by servicenow.
Folder Name:

  - ./GlideAjax/GlideAjax Example Template
    - # GlideAjax Example Template

When you need a client to contact the server after all OnLoad scripts have concluded.

Copy and paste and just change values around.

### Changes
  * Used GlideQuery instead of GlideRecord for better performance for counting records.
  * Reducing couple of lines of code.
  * Used g_form.addInfoMessage instead of alert for showing message.
Folder Name:

  - ./GlideAjax/GlideAjax Example Template
    - # GlideAjax Example Template

When you need a client to contact the server after all OnLoad scripts have concluded.

Copy and paste and just change values around.

### Changes
  * Used GlideQuery instead of GlideRecord for better performance for counting records.
  * Reducing couple of lines of code.
  * Used g_form.addInfoMessage instead of alert for showing message.
Folder Name:

  - ./GlideAjax/Reusable glideajax table query
    - 
Folder Name:

  - ./GlideAjax/Reusable GlideAjax
    - Reusable GlideAjax Example
When you need a client side script to contact the server and return few values from a table record matching your query. You can use this reusable GlideAjax code.

**An Example**
Need user fields like manager, Phone, Email matching sys_id of user:
function onChange(control, oldValue, newValue, isLoading) {
    if (isLoading || newValue == '') {
        return;
    }
    var g_ajax = new GlideAjax('ScriptIncludeName'); // pass name of Client callable script include name
    g_ajax.addParam('sysparm_name', 'scriptIncludeFunctionName'); // pass function name which will return result
    g_ajax.addParam('sysparm_table', 'sys_user'); 
    g_ajax.addParam('sysparm_query', 'sys_id='+g_form.getValue('requested_for')); 
    g_ajax.addParam('sysparm_returnAttributes', 'manager,email,phone'); 
    g_ajax.getXMLAnswer(callbackFunctionName);

    function callbackFunctionName(response) {
        var answer = JSON.parse(response);
        g_form.setValue('user_manager', answer.manager);
        g_form.setValue('email', answer.email);
        g_form.setValue('phone', answer.phone);
    }
}
Folder Name:

  - ./GlideAjax/Reusable GlideAjax
    - Reusable GlideAjax Example
When you need a client side script to contact the server and return few values from a table record matching your query. You can use this reusable GlideAjax code.

**An Example**
Need user fields like manager, Phone, Email matching sys_id of user:
function onChange(control, oldValue, newValue, isLoading) {
    if (isLoading || newValue == '') {
        return;
    }
    var g_ajax = new GlideAjax('ScriptIncludeName'); // pass name of Client callable script include name
    g_ajax.addParam('sysparm_name', 'scriptIncludeFunctionName'); // pass function name which will return result
    g_ajax.addParam('sysparm_table', 'sys_user'); 
    g_ajax.addParam('sysparm_query', 'sys_id='+g_form.getValue('requested_for')); 
    g_ajax.addParam('sysparm_returnAttributes', 'manager,email,phone'); 
    g_ajax.getXMLAnswer(callbackFunctionName);

    function callbackFunctionName(response) {
        var answer = JSON.parse(response);
        g_form.setValue('user_manager', answer.manager);
        g_form.setValue('email', answer.email);
        g_form.setValue('phone', answer.phone);
    }
}
Folder Name:

  - ./GlideAjax/ReturnMultipleProperties
    - ## Use values from returned object in Ajax call
- With this code snippet, make the ajax call from a client script.
- Replace `HM_Task_Details` with script include name of your choosing.
- Replace `sysparm_tableName` & `sysparm_recordID` with variable names from script include function. (can add as many as needed).
- Replace second argument (next to `sysparm_name`) with name of funtion from script include you would like to call. 
- In callback function use obj to access the property values of that object as shown in snippet.
Folder Name:

  - ./GlideAjax/EfficientGlideRecord (Client-side)
    - # EfficientGlideRecord
See related article for full usage instructions and API documentation:  
https://go.snc.guru/egr
Folder Name:

  - ./GlideAjax/EfficientGlideRecord (Client-side)
    - # EfficientGlideRecord
See related article for full usage instructions and API documentation:  
https://go.snc.guru/egr
Folder Name:

  - ./GlideAjax/EfficientGlideRecord (Client-side)
    - # EfficientGlideRecord
See related article for full usage instructions and API documentation:  
https://go.snc.guru/egr
Folder Name:

  - ./GlideAjax/EfficientGlideRecord (Client-side)
    - # EfficientGlideRecord
See related article for full usage instructions and API documentation:  
https://go.snc.guru/egr
Folder Name:

  - ./GlideAjax/AjaxAsyncOnSubmit
    - On submit client scripts do not support in making asynchronous calls to server on both platform and portal due to its nature of execution. This had always been a problem and there was a need to make validations work asynchronously on submitting a form/record. The support for getXMLWait() had also been removed which prevents the usage of synchronous GlideAjax call on a service portal. The snippet provides a workaround to execute async calls in both forms and catalog items, thus enabling server side validations during onsubmit.
Folder Name:

  - ./GlideAjax/AjaxAsyncOnSubmit
    - On submit client scripts do not support in making asynchronous calls to server on both platform and portal due to its nature of execution. This had always been a problem and there was a need to make validations work asynchronously on submitting a form/record. The support for getXMLWait() had also been removed which prevents the usage of synchronous GlideAjax call on a service portal. The snippet provides a workaround to execute async calls in both forms and catalog items, thus enabling server side validations during onsubmit.
Folder Name:

  - ./UX Client Script Include/Record Operation Utilities
    - #Record Operations Utilities which can be in imported in any UIB client script (Make sure to make the client script include accessible in all scopes)
1. createRecord - Function to execute create record data broker with necessary arguments
2. updateRecord - Function to execute update record data broker with necessary arguments
3. deleteRecord - Function to execute delete record data broker with necessary arguments

/*Sample script to show how to import client script include can be included :-
function handler({api, event, helpers, imports}) {
  const { createRecord, updateRecord, deleteRecord } = imports['global.Record Operation Utilities']();
}
*/
Folder Name:

  - ./RESTMessageV2/youtubeclient
    - Example of how you can utilize the older style rest message v2 to interact with youtube data client.
Has been replaced with the newer youtube spoke, but is fun to have around and reference how it used to be done.
Folder Name:

  - ./RESTMessageV2/Google-Chat
    - How we can use RESTMessageV2 to send notification in Google chat using Google chat webhook.

Reference link is given in the code on how we can get the Google chat webhook URL.
Folder Name:

  - ./RESTMessageV2/AzureDevOps
    - This rest message is used to create an issue in azure devops from servicenow using basic authentication
Folder Name:

  - ./RESTMessageV2/Web Scraping REST Message
    - # Web Scraper REST Message

This snippet shows how you would use RESTMessageV2 to scrape HTML from a website using a GET HTTP request.
Folder Name:

  - ./Scheduled Jobs/Approval Reminder
    - ## Use the code snippets to trigger approval reminder notifications. 

### 1 Change Approval Reminder.
change_reminder_scheduled_job.js

### 2 Requested item approval reminder to approvers.
requested_item_approval_reminder_approver.js

### 3 Requested item approval reminder to requestor.
requested_item_approval_reminder_requestor.js

*Note: Notifications and Events to be configured sepearately.*
Folder Name:

  - ./Scheduled Jobs/Approval Reminder
    - ## Use the code snippets to trigger approval reminder notifications. 

### 1 Change Approval Reminder.
change_reminder_scheduled_job.js

### 2 Requested item approval reminder to approvers.
requested_item_approval_reminder_approver.js

### 3 Requested item approval reminder to requestor.
requested_item_approval_reminder_requestor.js

*Note: Notifications and Events to be configured sepearately.*
Folder Name:

  - ./Scheduled Jobs/Approval Reminder
    - ## Use the code snippets to trigger approval reminder notifications. 

### 1 Change Approval Reminder.
change_reminder_scheduled_job.js

### 2 Requested item approval reminder to approvers.
requested_item_approval_reminder_approver.js

### 3 Requested item approval reminder to requestor.
requested_item_approval_reminder_requestor.js

*Note: Notifications and Events to be configured sepearately.*
Folder Name:

  - ./Scheduled Jobs/Auto close changes requests updated 30 days prior
    - This script can be used to auto close records if they have not been updated from past 30 days. For eg. I have taken change requests. This script can be written in a schedule job
to run it daily at 23:59:59 time to check if there is any such records present act accordingly.
Folder Name:

  - ./Scheduled Jobs/Deactivate INC in 90 days
    - This code snippet will help to inactivate the table records after 90 days of creation through schedule insert on sys trigger table  .
Can be used in BR/Script Inculde/Background script.
### Formatted for background script, please check the result in sys_ trigger Table or else click on document id it will redirect to  inserted JOb 


### Sample Output :
==============

Operation	Table	Row Count
insert	sys_trigger	1  

*** Script: Below runscript scheduled on sys trigger at 2023-01-23 13:29:48

var gr = new GlideAggregate('incident');
gr.addQuery('sys_id', '91cce5c52fb6111015d2e33df699b6f9');
gr.query();
if (gr.next()) {
gr.active = false;
gr.update();
}
Folder Name:

  - ./Scheduled Jobs/Remove Inactive and locked out users from All Groups and Roles
    - # Remove Inactive and locked out users from All Groups and Roles

It is always a good practise to have a secure and clean working instance. Having users with specific criteria such as the user is inactive and has been locked out should not have any role or belong to any group.
Folder Name:

  - ./Scheduled Jobs/ScheduleAtSpecificDaysAndTimes
    - Script to execute a schedule job on specific days and times. For eg: Schedule to run on all Mondays, Wednesdays and Fridays at 6, 12, 18 and 24 hours. You could place this in the condition script of a schedule job, configure the properties to setup the required number of days and times. The job should be scheduled to run periodically at every one hour and depending on the configured values, it will execute the job at the required days and time.
Folder Name:

  - ./Scheduled Jobs/Daily detection of customer updates made in 'Default' update set
    - **Scheduled Script Execution**

This script allows detecting any customer updates made in 'Default' update set (on different one based on configuration) in this day. You can change the action after detection from logging, to sending e-mail notification or creating event based on your needs.


**Example configuration of Scheduled Script Execution**

 ![Coniguration](ScreenShot_1.PNG)

**Example execution log**

 ![Log](ScreenShot_2.PNG)
Folder Name:

  - ./Scheduled Jobs/Get All Catalog Tasks without Request items
    - 
Folder Name:

  - ./Scheduled Jobs/Create Scheduled Imports Graphviz file
    - 
Folder Name:

  - ./Scheduled Jobs/Survey Trigger Scheduled Script
    - ## Use the code snippets to trigger survey via scheduled script. 

### Survey Trigger Scheduled Job
survey_trigger_sj.js

*Note:  Please update the query and sys_id as per the comments in the script*
Folder Name:

  - ./Scheduled Jobs/Lock out users who have not logged into the system longer than 30 days
    - **Scheduled Script Execution**

This script allows to *lock out* users who have not logged into the system for *longer than 30 days*. You can customize the additional query parameters and change the current ones for example in order to shorten or enlarge the time period. 

**Example configuration of Scheduled Script Execution**
 ![Coniguration](ScreenShot_1.PNG)

**Example execution log**
 ![Execution](ScreenShot_2.PNG)
Folder Name:

  - ./Scheduled Jobs/Paginated Export
    - 
Folder Name:

  - ./Integration/Import Sets/debug
    - 
Folder Name:

  - ./Integration/AzureAD Integration/Dynamically create reference records
    - ******* READ ME FOR AZURE USER PROVISIONING TO MAINTAIN REFERENCE FIELDS/TABLES ***** https://support.servicenow.com/kb?id=kb_article_view&sysparm_article=KB0779148

Because the Microsoft provided Azure Enterprise intergation with servicenow only creates records on the sys_user and sys_user_group tables this removes our ability to maintain the fields/tables that are referenced by these records (core tables).

This typically would be handled by a "Choice Action" of "create" on a transform map (in comparision to a typical LDAP user provisioning configuration).

In order to regain this functionality we must change the attribute mapping from within the Azure admin panel to map the attributes which correspond to these reference values to custom string fields on the ServiceNow side. (i.e u_department) once we are mapping these values to a custom string field we will manually add the "Find/Create" logic within a business rule configured to fire anytime these custom field values change.

Sudo logic is as follows(u_location example):

if u_location changes query for record on cmn_location with the same name if found result return sys_id if no result intitialize gliderecord, insert return new record sys_id

//relate returned sys_id in OOB reference field current.location = result.sys_id
Folder Name:

  - ./Integration/Import Sets Debug
    - 
Folder Name:

  - ./Integration/ITSM
    - Purpose: 

Allow bulk task_ci record inserts via a custom rest API endpoint. This will allow integration apps to insert task_ci relationships en masse on task records without needing to make an inordinate number of task_ci table API calls. Additionally, we can provide logic and filtering capabilities beyond the table API to make sure the right CI is associated to the task.

Endpoint:

https://<<<YOUR_INSTANCE_NAME>>>.service-now.com/api/gmi/related_live_ci_to_task

Payload Details:

User posts a JSON object with the task number and an array of CIs to associate to that task. Methods to identify the CIs being inserted can be sys_id, serial, FQDN, name, and IP, with that order of preference. Typically, we will only expect 1 identifier per CI line. fields in the post body:

Task: Task number that we should associate the CIs to. Required field, fail and return error code if this is not populated.

Post Body Example. Note that this is to illustrate the multiple ways users can identify CIs.


{
  "task": "INC123",
  "query_string": "status=1",
  "cis": [
    {
      "name": "p3acme1"
    },
    {
      "serial": "123"
    },
    {
      "sys_id": "abc123"
    },
    {
      "ip": "123.0.0.1"
    },
    {
      "FQDN": "p2acme.secureserver.net"
    }
  ]
}
Folder Name:

  - ./GlideAggregate/Count incidents based on category
    - Go to background and execute the script then you will get the total count of incidents based on category.

It will easily help to segregate the data based on categories/priority/ etc anything.
Folder Name:

  - ./GlideAggregate/Grouping by three columns
    - **GlideAggregate**

Script which allows to group by three columns (you can expand or decrease number of columns to fit your needs). In this example, the script allows counting number of active changes grouped by state, type and priority fields.

Special thanks to *SN-AJB* for his post about GlideAggregate: https://developer.servicenow.com/blog.do?p=/post/glideaggregate/. Absolutely worth taking a look!

**Example execution logs**

![Logs](ScreenShot_1.PNG)
Folder Name:

  - ./GlideAggregate/Tiered grouping of an integer column
    - # Tiered grouping of an integer column

If you have a column with points (as an integer), this script breaks them down by percentile tiers.
Folder Name:

  - ./GlideAggregate/getCountAfterDate
    - ## GlideAggregate
1. Instantiate GlideAggregate object, include table in parameter.
2. `addQuery` method will restrict returned data-set based on added queries.
3. `addAggregate` groups the returned data-set by second argument within parameters & the first argument within the parameters is the calulation ran based on that grouping.
4. `query` runs glideaggregate.
5. `getAggregate` collects the data-set grouped by data.
Folder Name:

  - ./GlideAggregate/Group Count
    - # Group Count
Sometimes you need to filter a list by group count (e.g. finding duplicates) unfortunately as of now the UI(16) doesn't provide a way to filter records based on group count. This function should help with that.

## Example Script
```javascript
var table = "sys_user";
var encodedQuery = "employee_numberISNOTEMPTY";
var groupBy = "employee_number";
var minGroupCount = 2;
var transformFn = function(ga, groupCount) {
  return {
    "employee_number": ga.getValue("employee_number"),
    "group_count": groupCount
  };
};
var countOutput = getGroupCount(
  table, encodedQuery, groupBy, minGroupCount, transformFn
);
gs.info('Output is ' + JSON.stringify(countOutput, null, 4));
```
## Example Result
```json
[
  {
    "employee_number": "000051",
    "group_count": "2"
  },
  {
    "employee_number": "000055",
    "group_count": "2"
  },
  {
    "employee_number": "000058",
    "group_count": "3"
  }
]
```
Folder Name:

  - ./GlideAggregate/Group Count
    - # Group Count
Sometimes you need to filter a list by group count (e.g. finding duplicates) unfortunately as of now the UI(16) doesn't provide a way to filter records based on group count. This function should help with that.

## Example Script
```javascript
var table = "sys_user";
var encodedQuery = "employee_numberISNOTEMPTY";
var groupBy = "employee_number";
var minGroupCount = 2;
var transformFn = function(ga, groupCount) {
  return {
    "employee_number": ga.getValue("employee_number"),
    "group_count": groupCount
  };
};
var countOutput = getGroupCount(
  table, encodedQuery, groupBy, minGroupCount, transformFn
);
gs.info('Output is ' + JSON.stringify(countOutput, null, 4));
```
## Example Result
```json
[
  {
    "employee_number": "000051",
    "group_count": "2"
  },
  {
    "employee_number": "000055",
    "group_count": "2"
  },
  {
    "employee_number": "000058",
    "group_count": "3"
  }
]
```
Folder Name:

  - ./GlideAggregate/Using addHaving
    - **GlideAggregate**

Script which shows how to use addHaving() function, which allows adding conditions on aggregate functions. In this example, the script will show which users have more than 35 roles assignments in sys_user_has_role table. You can use it also in different scenarios, modifying the table and other conditions.



Function addHaving() can not be used in Scoped Applications!

**Example execution logs**

![Logs](ScreenShot_1.PNG)
Folder Name:

  - ./Processors/Dynamic Sitemap
    - 
Folder Name:

  - ./Attachments/Convert KnowledgePage to PDF
    - # Convert Knowledge Page HTML to PDF and attach it.
* Create PDF using GeneralPDF.
* Try it from a simple HTML conversion.
* It seems that the conversion fails if the HTML contains image files.
* See the Script Include GeneralPDF for details. 
* GeneralPDF is already in Script Include, but it may not exist in some environments

```javascript
var grKnow = new GlideRecord('kb_knowledge');
// Get a simple HTML KnowledgePage
if(grKnow.get('<KnowledgePage sys_id>') && grKnow.getValue('text')){
    // Create PDF Document.
    var pdfDoc = new GeneralPDF.Document(null, null, null, null, null, null);
    var document = new GeneralPDF(pdfDoc);
    document.startHTMLParser();
    document.addHTML(grKnow.getValue('text'));
    document.stopHTMLParser();
    // Create PDF Attachment.
    var att = new GeneralPDF.Attachment();
    att.setTableName(grKnow.getTableName());
    att.setTableId(grKnow.getValue('sys_id'));
    // Attached file name. 
    att.setName('TestPDF.pdf');
    att.setType('application/pdf');
    att.setBody(document.get());
    // Attachment creation
    GeneralPDF.attach(att);
}
```
Folder Name:

  - ./Attachments/Base 64 to Attachment
    - This could be used to convert base 64 content into an attachment in ServiceNow. This is mainly used for integrating attachments from external systems to read and convert the base 64 content into an attachment.

Sample Usage - Attaching and xls file on a incident record.

var attachment = convertBase64ToAttachment("0M8R4KGxGuEAAAAAAAAAAAAAAAAAAAAAOwADAP7/CQAGAAAAAAAAAAAAAAABAAAAAAAAAAAAAAAAEAAABwAAAAEAAAD+////AAAAAAgAAAD///////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////9SAG8AbwB0ACAARQBuAHQAcgB5AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAFgAFAf//////////AQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACgTKHLiKDGAQEAAABACgAAAAAAAFcAbwByAGsAYgBvAG8AawAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAASAAIB////////////////AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABgKAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAIAAAD///////////////8AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAgAAAP///////////////wAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAkIEAAABgUA0xDMB0EAAAAGAAAA4QACALAEwQACAAAA4gAAAFwAcAALAABCb3cgUnVnZ2VyaSAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgQgACALAEYQECAAAAPQECAAAAnAACAA4AGQACAAAAEgACAAAAEwACAAAArwECAAAAvAECAAAAPQASAGgBDgFcOr4jOAAAAAAAAQBYAkAAAgAAAI0AAgAAACIAAgAAAA4AAgABALcBAgAAANoAAgAAADEAGgDIAAAA/3+QAQAAAAAAAAUBQQByAGkAYQBsADEAGgDIAAAA/3+QAQAAAAAAAAUBQQByAGkAYQBsADEAGgDIAAAA/3+QAQAAAAAAAAUBQQByAGkAYQBsADEAGgDIAAAA/3+QAQAAAAAAAAUBQQByAGkAYQBsADEAGgDIAAAA/3+8AgAAAAAAAAUBQQByAGkAYQBsAB4EHAAFABcAACIkIiMsIyMwXyk7XCgiJCIjLCMjMFwpHgQhAAYAHAAAIiQiIywjIzBfKTtbUmVkXVwoIiQiIywjIzBcKR4EIgAHAB0AACIkIiMsIyMwLjAwXyk7XCgiJCIjLCMjMC4wMFwpHgQnAAgAIgAAIiQiIywjIzAuMDBfKTtbUmVkXVwoIiQiIywjIzAuMDBcKR4ENwAqADIAAF8oIiQiKiAjLCMjMF8pO18oIiQiKiBcKCMsIyMwXCk7XygiJCIqICItIl8pO18oQF8pHgQuACkAKQAAXygqICMsIyMwXyk7XygqIFwoIywjIzBcKTtfKCogIi0iXyk7XyhAXykeBD8ALAA6AABfKCIkIiogIywjIzAuMDBfKTtfKCIkIiogXCgjLCMjMC4wMFwpO18oIiQiKiAiLSI/P18pO18oQF8pHgQ2ACsAMQAAXygqICMsIyMwLjAwXyk7XygqIFwoIywjIzAuMDBcKTtfKCogIi0iPz9fKTtfKEBfKR4EGACkABMAAHl5eXkvbW0vZGQgaGg6bW06c3PgABQAAAAAAPX/IAAAAAAAAAAAAAAAwCDgABQAAQAAAPX/IAAA9AAAAAAAAAAAwCDgABQAAQAAAPX/IAAA9AAAAAAAAAAAwCDgABQAAgAAAPX/IAAA9AAAAAAAAAAAwCDgABQAAgAAAPX/IAAA9AAAAAAAAAAAwCDgABQAAAAAAPX/IAAA9AAAAAAAAAAAwCDgABQAAAAAAPX/IAAA9AAAAAAAAAAAwCDgABQAAAAAAPX/IAAA9AAAAAAAAAAAwCDgABQAAAAAAPX/IAAA9AAAAAAAAAAAwCDgABQAAAAAAPX/IAAA9AAAAAAAAAAAwCDgABQAAAAAAPX/IAAA9AAAAAAAAAAAwCDgABQAAAAAAPX/IAAA9AAAAAAAAAAAwCDgABQAAAAAAPX/IAAA9AAAAAAAAAAAwCDgABQAAAAAAPX/IAAA9AAAAAAAAAAAwCDgABQAAAAAAPX/IAAA9AAAAAAAAAAAwCDgABQAAAAAAAEAIAAAAAAAAAAAAAAAwCDgABQAAQArAPX/IAAA+AAAAAAAAAAAwCDgABQAAQApAPX/IAAA+AAAAAAAAAAAwCDgABQAAQAsAPX/IAAA+AAAAAAAAAAAwCDgABQAAQAqAPX/IAAA+AAAAAAAAAAAwCDgABQAAQAJAPX/IAAA+AAAAAAAAAAAwCDgABQAAACkAAEAAAAAAAAACAQIBAAAwCDgABQAAAAAAAEACAAAEAAACAQIBAAAwCDgABQABQAAAAEAIAAACAAACAQIBAAAwCCTAgQAEIAD/5MCBAARgAb/kwIEABKABP+TAgQAE4AH/5MCBAAAgAD/kwIEABSABf9gAQIAAACFAA4AxwYAAAAABgBQYWdlIDGMAAQAAQABAPwA1wAcAAAAEgAAAAYAAE51bWJlcggAAENhdGVnb3J5CAAAUHJpb3JpdHkOAABJbmNpZGVudCBzdGF0ZQoAAEVzY2FsYXRpb24RAABTaG9ydCBkZXNjcmlwdGlvbgsAAEFzc2lnbmVkIHRvCAAASU5DMTAwMTYOAABJbnF1aXJ5IC8gSGVscAcAADQgLSBMb3cGAABBY3RpdmUGAABOb3JtYWwPAABLZXlib2FyZCBzdGlua3MAAAAIAABJTkMxMDAxNwMAAEJvdwgAAElOQzEwMDE5BAAAQm93K/8AGgAIANYFAAAMAAAAQAYAAHYAAACTBgAAyQAAAAoAAAAJCBAAAAYQALsNzAfBAAAABgAAAA0AAgABAAwAAgBkAA8AAgABABEAAgAAABAACAD8qfHSTWJQP18AAgABACoAAgAAACsAAgAAAIIAAgABAIAACAAAAAAAAAAAACUCBAAAAP8AgQACAMEEGwACAAAAGgACAAAAFAAAABUAAACDAAIAAACEAAIAAAChACIAAQBkAAEAAQABAAIALAEsAQAAAAAAAOA/AAAAAAAA4D8AAFUAAgAIAH0ADAAAAAAAAAoPAAYAAAB9AAwAAQABAAAKDwAGAAAAfQAMAAIAAgAACg8ABgAAAH0ADAADAAMAAA4PAAYAAAB9AAwABAAEAAAKDwAGAAAAfQAMAAUABQAAEQ8ABgAAAH0ADAAGAAYAAAsPAAYAAAAAAg4AAAAAAAMAAAAAAAcAAAD9AAoAAAAAABcAAAAAAP0ACgAAAAEAFwABAAAA/QAKAAAAAgAXAAIAAAD9AAoAAAADABcAAwAAAP0ACgAAAAQAFwAEAAAA/QAKAAAABQAXAAUAAAD9AAoAAAAGABcABgAAAP0ACgABAAAAFgAHAAAA/QAKAAEAAQAWAAgAAAD9AAoAAQACABYACQAAAP0ACgABAAMAFgAKAAAA/QAKAAEABAAWAAsAAAD9AAoAAQAFABYADAAAAP0ACgABAAYAFgANAAAA/QAKAAIAAAAWAA4AAAD9AAoAAgABABYACAAAAP0ACgACAAIAFgAJAAAA/QAKAAIAAwAWAAoAAAD9AAoAAgAEABYACwAAAP0ACgACAAUAFgAPAAAA/QAKAAIABgAWAA0AAAD9AAoAAwAAABYAEAAAAP0ACgADAAEAFgAIAAAA/QAKAAMAAgAWAAkAAAD9AAoAAwADABYACgAAAP0ACgADAAQAFgALAAAA/QAKAAMABQAWABEAAAD9AAoAAwAGABYADQAAAAgCEAAAAAAABgD/AAAAAAAAAAAACAIQAAEAAAAGAP8AAAAAAAAAAAAIAhAAAgAAAAYA/wAAAAAAAAAAAAgCEAADAAAABgD/AAAAAAAAAAAAPgISAL4HAAAAAEAAAAAAAAAAAAAAAEEACgAAAAEAAQBAAAIAHQAPAAIAAAAAAAABAAAAAAAAABIAAgAAAAoAAAD//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////wEAAAACAAAAAwAAAAQAAAAFAAAABgAAAAcAAAAIAAAACQAAAAoAAAALAAAADAAAAA0AAAAOAAAADwAAABAAAAARAAAAEgAAABMAAAAUAAAAFQAAABYAAAAXAAAAGAAAABkAAAAaAAAAGwAAABwAAAAdAAAAHgAAAB8AAAAgAAAAIQAAACIAAAAjAAAAJAAAACUAAAAmAAAAJwAAACgAAAD+/////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////v///wIAAAADAAAABAAAAAUAAAAGAAAA/v////7////+//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////8=", "incident.xls", "application/vnd.ms-excel", "incident", "71e0fa504750210042bd757f2ede2730");

//gs.info("Attachment: " + attachment);
Folder Name:

  - ./Attachments/CSVParser
    - The script parses through a CSV attachment accessed from the instance and reads each data row by row and column by column. You could also specify the required separator and quote character to escape them.

Sample Usage:  

parseCSVFile("sys_id=76fc711f2f0b7050809e51172799b685");
Folder Name:

  - ./Attachments/Attachment to Base64
    - # Base64 file encoder

Convert attachment to Base64
Folder Name:

  - ./Attachments/Calculate attachment hash code
    - This is example of recalculate the hash code using the glide digest getSHA256HexFromInputStream method.

GlideDigest() -
    This class provides methods for creating a message digest from strings or input streams using MD5, SHA1, or SHA256 hash algorithms.

Docs link: https://developer.servicenow.com/dev.do#!/reference/api/tokyo/server/no-namespace/c_GlideDigestScopedAPI#r_SGDigest-GlideDigest

getSHA256HexFromInputStream - function takes GlideScriptableInputStream input stream as parameter.
Folder Name:

  - ./Attachments/attachmentToXMLParse
    - 
Folder Name:

  - ./Attachments/ExportRecordsAnyFormat
    - The snippet can be used to export records from any table and then attach on another record. You could export records in any of the these formats (CSV, XLS, XLSX, PDF, JSON, XML, XSD, SCHEMA, RSS) from any table view based on an encoded query. If required, the attachment can be send out to users through a notification (with check include attachments).

Sample Usage:

//Export all active incidents from the ESS view into XLSX format 

gs.print(exportRecords('incident', 'b3f076504750210042bd757f2ede273f', 'active=true', 'ess', 'XLSX', 'Active Incidents.xlsx'));

//Export all active incident from the defaut view in JSON format

gs.print(exportRecords('incident', 'b3f076504750210042bd757f2ede273f', 'active=true', '', 'JSONv2', 'Active Incidents.json'));

//Export a record into PDF

gs.print(exportRecords('incident', 'b3f076504750210042bd757f2ede273f', 'sys_id=b3f076504750210042bd757f2ede273f', '', 'PDF', 'record.pdf'));
Folder Name:

  - ./Attachments/Delete RITM Attachment
    - The Delete RITM attachment business rule will automatically deletes the attachment on RITM, when the attachment is deleted on SCTASK.
Folder Name:

  - ./Attachments/Attachment to base64 in scope
    - Encode attachment to base64 for scoped applications. Uses the GlideSysAttachment API. 
Place of use: creating a spoke/integration where you need to send an attachment via REST.
Folder Name:

  - ./Attachments/ExportAttachmentsToMidServer
    - The snippet can be used to export all attachments within any record in ServiceNow to the mid server. You could specify a relative file path within the server's agent folder and it will copy them into it.

Sample Usage

exportAttachmentsToMid("66a4daff2f9ff810ba1b52492799b6f1", "\\Incident\\INC00293930", "Mid Server 01");
Folder Name:

  - ./Record Producer/Create Records By Import Set
    - 
Folder Name:

  - ./Scripted REST Api/Retrieve all variables from RITM
    - # Retrieve all variables (including multi-row) from any Request Item or Catalog Task - and push JSON for use in a Scripted REST API
It's really not that hard to do using existing APIs, but if you want to pull a list of variables and their values, it gets a little messy. 
If you want values from a Multi-Row Variable Set, it gets even messier.  So, we set about building a Scripted REST API our partners can use. 

 1. [Build a Scripted REST API- resource configuration in the comments of the script](scripted_rest_api.js) 
 2. [Build a script include (the one referenced in the resource script above)](CHVarUtils_ScriptInclude.js)
 3. [Sample Output return in JSON format](output_example.js)
Folder Name:

  - ./Scripted REST Api/Retrieve all variables from RITM
    - # Retrieve all variables (including multi-row) from any Request Item or Catalog Task - and push JSON for use in a Scripted REST API
It's really not that hard to do using existing APIs, but if you want to pull a list of variables and their values, it gets a little messy. 
If you want values from a Multi-Row Variable Set, it gets even messier.  So, we set about building a Scripted REST API our partners can use. 

 1. [Build a Scripted REST API- resource configuration in the comments of the script](scripted_rest_api.js) 
 2. [Build a script include (the one referenced in the resource script above)](CHVarUtils_ScriptInclude.js)
 3. [Sample Output return in JSON format](output_example.js)
Folder Name:

  - ./Scripted REST Api/Retrieve all variables from RITM
    - # Retrieve all variables (including multi-row) from any Request Item or Catalog Task - and push JSON for use in a Scripted REST API
It's really not that hard to do using existing APIs, but if you want to pull a list of variables and their values, it gets a little messy. 
If you want values from a Multi-Row Variable Set, it gets even messier.  So, we set about building a Scripted REST API our partners can use. 

 1. [Build a Scripted REST API- resource configuration in the comments of the script](scripted_rest_api.js) 
 2. [Build a script include (the one referenced in the resource script above)](CHVarUtils_ScriptInclude.js)
 3. [Sample Output return in JSON format](output_example.js)
Folder Name:

  - ./Scripted REST Api/Approval APIs
    - Approval API to Approve / Reject the Approval Record 

* Approve API

Request :
HTTP Method / URI
POST https://<instance name>.service-now.com/api/sr_approvals/<approval record sysid>/approve
  
Headers :
Acceptapplication/json
Content-Typeapplication/json
  
Request Body : 
{
'comment' : 'Please approve this record'
}
  
Response :
Status code : 200 OK 
  
 Response Body
{
  "result": "Record has been Approved!"
}
  
* Reject API
  
Request :
HTTP Method / URI
POST https://<instance name>.service-now.com/api/sr_approvals/<approval record sysid>/reject
  
Headers : 
Acceptapplication/json
Content-Typeapplication/json
  
Request Body : 
{
'comment' : 'Please reject this record'
}
  
Response :
Status code : 200 OK 
  
 Response Body
{
  "result": "Record has been Rejected!"
}
Folder Name:

  - ./Scripted REST Api/Approval APIs
    - Approval API to Approve / Reject the Approval Record 

* Approve API

Request :
HTTP Method / URI
POST https://<instance name>.service-now.com/api/sr_approvals/<approval record sysid>/approve
  
Headers :
Acceptapplication/json
Content-Typeapplication/json
  
Request Body : 
{
'comment' : 'Please approve this record'
}
  
Response :
Status code : 200 OK 
  
 Response Body
{
  "result": "Record has been Approved!"
}
  
* Reject API
  
Request :
HTTP Method / URI
POST https://<instance name>.service-now.com/api/sr_approvals/<approval record sysid>/reject
  
Headers : 
Acceptapplication/json
Content-Typeapplication/json
  
Request Body : 
{
'comment' : 'Please reject this record'
}
  
Response :
Status code : 200 OK 
  
 Response Body
{
  "result": "Record has been Rejected!"
}
Folder Name:

  - ./Scripted REST Api/Approval APIs
    - Approval API to Approve / Reject the Approval Record 

* Approve API

Request :
HTTP Method / URI
POST https://<instance name>.service-now.com/api/sr_approvals/<approval record sysid>/approve
  
Headers :
Acceptapplication/json
Content-Typeapplication/json
  
Request Body : 
{
'comment' : 'Please approve this record'
}
  
Response :
Status code : 200 OK 
  
 Response Body
{
  "result": "Record has been Approved!"
}
  
* Reject API
  
Request :
HTTP Method / URI
POST https://<instance name>.service-now.com/api/sr_approvals/<approval record sysid>/reject
  
Headers : 
Acceptapplication/json
Content-Typeapplication/json
  
Request Body : 
{
'comment' : 'Please reject this record'
}
  
Response :
Status code : 200 OK 
  
 Response Body
{
  "result": "Record has been Rejected!"
}
Folder Name:

  - ./Scripted REST Api/Promise API Call
    - Allows you to make async/await promise API Calls using Request
Folder Name:

  - ./Service Portal Widgets/Clickable SVG Image
    - # Can clickable svg image
## main used echarts.js


## *step1*
Prepare a svg image, focus, you need set name for every root you want to click from svg image. there is a example svg image source code.
```html
<g name="7G" id="g19657">
    <path fill="#cccccc" stroke="#000000" d="m 225.8,250.9 h -11.9 c -1.7,0 -3.1,-1.4 -3.1,-3.1 V 239 c 0,-1.7 1.4,-3.1 3.1,-3.1 h 11.9 c 1.7,0 3.1,1.4 3.1,3.1 v 8.9 c -0.1,1.6 -1.4,3 -3.1,3 z" id="path19653" />
    <path fill="#cccccc" stroke="#000000" d="m 231.4,248.3 h -2.6 v -9.8 h 2.6 c 0.9,0 1.6,0.7 1.6,1.6 v 6.5 c 0.1,0.9 -0.7,1.7 -1.6,1.7 z" id="path19655" />
</g>

<g name="8G" id="g19663">
    <path fill="#cccccc" stroke="#000000" d="m 256,250.9 h -11.9 c -1.7,0 -3.1,-1.4 -3.1,-3.1 V 239 c 0,-1.7 1.4,-3.1 3.1,-3.1 H 256 c 1.7,0 3.1,1.4 3.1,3.1 v 8.9 c 0,1.6 -1.4,3 -3.1,3 z" id="path19659" />
    <path fill="#cccccc" stroke="#000000" d="m 261.7,248.3 h -2.6 v -9.8 h 2.6 c 0.9,0 1.6,0.7 1.6,1.6 v 6.5 c 0,0.9 -0.7,1.7 -1.6,1.7 z" id="path19661" />
</g>

<g name="9G" id="g19669">
    <path fill="#cccccc" stroke="#000000" d="m 286.2,250.9 h -11.9 c -1.7,0 -3.1,-1.4 -3.1,-3.1 V 239 c 0,-1.7 1.4,-3.1 3.1,-3.1 h 11.9 c 1.7,0 3.1,1.4 3.1,3.1 v 8.9 c 0,1.6 -1.4,3 -3.1,3 z" id="path19665" />
    <path fill="#cccccc" stroke="#000000" d="m 291.9,248.3 h -2.6 v -9.8 h 2.6 c 0.9,0 1.6,0.7 1.6,1.6 v 6.5 c 0.1,0.9 -0.7,1.7 -1.6,1.7 z" id="path19667" />
</g>

<g name="10G" id="g19675">
    <path fill="#cccccc" stroke="#000000" d="m 316.5,250.9 h -11.9 c -1.7,0 -3.1,-1.4 -3.1,-3.1 V 239 c 0,-1.7 1.4,-3.1 3.1,-3.1 h 11.9 c 1.7,0 3.1,1.4 3.1,3.1 v 8.9 c 0,1.6 -1.4,3 -3.1,3 z" id="path19671" />
    <path fill="#cccccc" stroke="#000000" d="m 322.1,248.3 h -2.6 v -9.8 h 2.6 c 0.9,0 1.6,0.7 1.6,1.6 v 6.5 c 0.1,0.9 -0.6,1.7 -1.6,1.7 z" id="path19673" />
</g>

```
Just focus the g tag, every set a unique name.

## *step2*
Go to your instance and direct to *System UI > Images*， upload your svg image here, and remember the name you typed.

## *step3*
Uing the image in your widget.
```javascript
$.get('example.svg', function(svg) {

		echarts.registerMap('demo', {
			svg: svg
		});

		var takenSeatNames = ['B2-001','B2-020','B2-003','B2-009','B2-031'];

		option = {
			tooltip: {},
			geo: {
				map: 'demo',
				roam: true,
				selectedMode: 'single',
				layoutCenter: ['50%', '50%'],
				layoutSize: '95%',
				tooltip: {
					show: true
				},
				itemStyle: {
					color: '#fff'
				},
				emphasis: {
					itemStyle: {
						color: null,
						borderColor: 'green',
						borderWidth: 2
					},
					label: {
						show: false
					}
				},
				select: {
					itemStyle: {
						//color: '#fff'
					},
					label: {
						show: false,
						textBorderColor: '#fff',
						textBorderWidth: 2
					}
				},
				regions: makeTakenRegions(takenSeatNames)
			}
		};

		function makeTakenRegions(takenSeatNames) {
			var regions = [];
			for (var i = 0; i < takenSeatNames.length; i++) {
				regions.push({
					name: takenSeatNames[i],
					silent: true,
					itemStyle: {
						color: '#bf0e08'
					},
					emphasis: {
						itemStyle: {
							borderColor: '#aaa',
							borderWidth: 1
						}
					},
					select: {
						itemStyle: {
							//color: '#bf0e08'
						}
					}
				});
			}
			return regions;
		}
```

## *step4*
add echarts.js to your widget dependencies.

# Now you can use it.
Folder Name:

  - ./Service Portal Widgets/Clickable SVG Image
    - # Can clickable svg image
## main used echarts.js


## *step1*
Prepare a svg image, focus, you need set name for every root you want to click from svg image. there is a example svg image source code.
```html
<g name="7G" id="g19657">
    <path fill="#cccccc" stroke="#000000" d="m 225.8,250.9 h -11.9 c -1.7,0 -3.1,-1.4 -3.1,-3.1 V 239 c 0,-1.7 1.4,-3.1 3.1,-3.1 h 11.9 c 1.7,0 3.1,1.4 3.1,3.1 v 8.9 c -0.1,1.6 -1.4,3 -3.1,3 z" id="path19653" />
    <path fill="#cccccc" stroke="#000000" d="m 231.4,248.3 h -2.6 v -9.8 h 2.6 c 0.9,0 1.6,0.7 1.6,1.6 v 6.5 c 0.1,0.9 -0.7,1.7 -1.6,1.7 z" id="path19655" />
</g>

<g name="8G" id="g19663">
    <path fill="#cccccc" stroke="#000000" d="m 256,250.9 h -11.9 c -1.7,0 -3.1,-1.4 -3.1,-3.1 V 239 c 0,-1.7 1.4,-3.1 3.1,-3.1 H 256 c 1.7,0 3.1,1.4 3.1,3.1 v 8.9 c 0,1.6 -1.4,3 -3.1,3 z" id="path19659" />
    <path fill="#cccccc" stroke="#000000" d="m 261.7,248.3 h -2.6 v -9.8 h 2.6 c 0.9,0 1.6,0.7 1.6,1.6 v 6.5 c 0,0.9 -0.7,1.7 -1.6,1.7 z" id="path19661" />
</g>

<g name="9G" id="g19669">
    <path fill="#cccccc" stroke="#000000" d="m 286.2,250.9 h -11.9 c -1.7,0 -3.1,-1.4 -3.1,-3.1 V 239 c 0,-1.7 1.4,-3.1 3.1,-3.1 h 11.9 c 1.7,0 3.1,1.4 3.1,3.1 v 8.9 c 0,1.6 -1.4,3 -3.1,3 z" id="path19665" />
    <path fill="#cccccc" stroke="#000000" d="m 291.9,248.3 h -2.6 v -9.8 h 2.6 c 0.9,0 1.6,0.7 1.6,1.6 v 6.5 c 0.1,0.9 -0.7,1.7 -1.6,1.7 z" id="path19667" />
</g>

<g name="10G" id="g19675">
    <path fill="#cccccc" stroke="#000000" d="m 316.5,250.9 h -11.9 c -1.7,0 -3.1,-1.4 -3.1,-3.1 V 239 c 0,-1.7 1.4,-3.1 3.1,-3.1 h 11.9 c 1.7,0 3.1,1.4 3.1,3.1 v 8.9 c 0,1.6 -1.4,3 -3.1,3 z" id="path19671" />
    <path fill="#cccccc" stroke="#000000" d="m 322.1,248.3 h -2.6 v -9.8 h 2.6 c 0.9,0 1.6,0.7 1.6,1.6 v 6.5 c 0.1,0.9 -0.6,1.7 -1.6,1.7 z" id="path19673" />
</g>

```
Just focus the g tag, every set a unique name.

## *step2*
Go to your instance and direct to *System UI > Images*， upload your svg image here, and remember the name you typed.

## *step3*
Uing the image in your widget.
```javascript
$.get('example.svg', function(svg) {

		echarts.registerMap('demo', {
			svg: svg
		});

		var takenSeatNames = ['B2-001','B2-020','B2-003','B2-009','B2-031'];

		option = {
			tooltip: {},
			geo: {
				map: 'demo',
				roam: true,
				selectedMode: 'single',
				layoutCenter: ['50%', '50%'],
				layoutSize: '95%',
				tooltip: {
					show: true
				},
				itemStyle: {
					color: '#fff'
				},
				emphasis: {
					itemStyle: {
						color: null,
						borderColor: 'green',
						borderWidth: 2
					},
					label: {
						show: false
					}
				},
				select: {
					itemStyle: {
						//color: '#fff'
					},
					label: {
						show: false,
						textBorderColor: '#fff',
						textBorderWidth: 2
					}
				},
				regions: makeTakenRegions(takenSeatNames)
			}
		};

		function makeTakenRegions(takenSeatNames) {
			var regions = [];
			for (var i = 0; i < takenSeatNames.length; i++) {
				regions.push({
					name: takenSeatNames[i],
					silent: true,
					itemStyle: {
						color: '#bf0e08'
					},
					emphasis: {
						itemStyle: {
							borderColor: '#aaa',
							borderWidth: 1
						}
					},
					select: {
						itemStyle: {
							//color: '#bf0e08'
						}
					}
				});
			}
			return regions;
		}
```

## *step4*
add echarts.js to your widget dependencies.

# Now you can use it.
Folder Name:

  - ./Service Portal Widgets/ApplyCSSDynamically
    - The widget demonstrates how CSS can be dynamically applied on the HTML attributes via client controller. Inorder to demonstrate, a color picker dropdown has been placed in the HTML. Upon selecting a color option, the corresponding CSS is applied on an HTML text to color it with the same.
Folder Name:

  - ./Service Portal Widgets/ApplyCSSDynamically
    - The widget demonstrates how CSS can be dynamically applied on the HTML attributes via client controller. Inorder to demonstrate, a color picker dropdown has been placed in the HTML. Upon selecting a color option, the corresponding CSS is applied on an HTML text to color it with the same.
Folder Name:

  - ./Service Portal Widgets/Client side pagination
    - This code can be used to add client side pagination to the widget. 
if there are a lot of records on a customized widget and you prefer using client side pagination instead of server side pagination, use this method me
Folder Name:

  - ./Service Portal Widgets/Portal widgets Performance Test
    - 
Folder Name:

  - ./Service Portal Widgets/Create diagram using GoJS library
    - # Creating productionProcess using gojs
## Introduction
In this snippet you will create a custom process using a custom page and populating data using GoJS native library

## Step 1: Create a new Widget
***Go to Service Portal > Widget > Click New***
- Name: Custom productionProcess
- Id: custom-gojs-productionProcess
- Click on `submit`

***Body HTML template***
- Copy and paste below `HTML Code` in Widget's HTML Template section
```HTML
<div id="myDiagramDiv" style="border: solid 1px black; width:70%; height:550px; display: inline-block; vertical-align: top"></div>
```

***CSS/SCSS***
- Copy and paste below `CSS` in Widget's CSS/SCSS Section
```CSS
#infobox {
  width: 256px;
  background: #757575;
  color: #FFF;
  padding: 20px;
}

#myDiagramDiv * {
  outline: none;
  -webkit-tap-highlight-color: rgba(255, 255, 255, 0); /* mobile webkit */
}
```
***Client Side Scripts***
- Copy and Paste below `Script` in Widget's Client Side Section
```javascript
// build GraphObject
  var $ = go.GraphObject.make;  // for conciseness in defining templates
  myDiagram = $(go.Diagram, "myDiagramDiv",  // create a Diagram for the DIV HTML element
    {
      maxSelectionCount: 1, // users can select only one part at a time
      "toolManager.hoverDelay": 10,  // how quickly tooltips are shown
      initialAutoScale: go.Diagram.Uniform,  // scale to show all of the contents
      "ChangedSelection": onSelectionChanged, // view additional information
    });

  function infoString(obj) {
    var part = obj.part;
    if (part instanceof go.Adornment) part = part.adornedPart;
    var msg = "";
    if (part instanceof go.Link) {
      msg = "";
    } else if (part instanceof go.Node) {
      msg = part.data.text + ":\n\n" + part.data.description;
    }
    return msg;
  }

  var colors = {
    "red": "#be4b15",
    "green": "#52ce60",
    "blue": "#6ea5f8",
    "lightred": "#fd8852",
    "lightblue": "#afd4fe",
    "lightgreen": "#b9e986",
    "pink": "#faadc1",
    "purple": "#d689ff",
    "orange": "#fdb400",
  };

  // A data binding conversion function. Given an name, return the Geometry.
  // If there is only a string, replace it with a Geometry object, which can be shared by multiple Shapes.
  function geoFunc(geoname) {
    var geo = icons[geoname];
    if (typeof geo === "string") {
      geo = icons[geoname] = go.Geometry.parse(geo, true);
    }
    return geo;
  }

  myDiagram.nodeTemplate =
    $(go.Node, "Spot",
      {
        locationObjectName: 'main',
        locationSpot: go.Spot.Center,
        toolTip:
          $(go.Adornment, "Auto",
            $(go.Shape, { fill: "#CCFFCC" }),
            $(go.TextBlock, { margin: 4, width: 140 }, //https://gojs.net/latest/intro/toolTips.html
              new go.Binding("text", "", infoString).ofObject()))
        /*toolTip:
          $("ToolTip",
            $(go.TextBlock, { margin: 4, width: 140 }, //https://gojs.net/latest/intro/toolTips.html
              new go.Binding("text", "", infoString).ofObject())
          )*/
      },
      new go.Binding("location", "pos", go.Point.parse).makeTwoWay(go.Point.stringify),
      // The main element of the Spot panel is a vertical panel housing an optional icon,
      // plus a rectangle that acts as the port
      $(go.Panel, "Vertical",
        $(go.Shape, {
          name: 'icon',
          width: 1, height: 1,
          stroke: null, strokeWidth: 0,
          fill: colors.blue
        },
          new go.Binding("fill", "color", function (c) { return colors[c]; }),
          new go.Binding("width", "iconWidth"),
          new go.Binding("height", "iconHeight"),
          new go.Binding("geometry", "icon", geoFunc)),
        $(go.Shape, {
          name: 'main',
          width: 40, height: 40,
          margin: new go.Margin(-1, 0, 0, 0),
          portId: "",
          stroke: null, strokeWidth: 0,
          fill: colors.blue
        },
          new go.Binding("fill", "color", function (c) { return colors[c]; }),
          new go.Binding("width", "portWidth"),
          new go.Binding("height", "portHeight"))
      ),

      $(go.TextBlock, {
        font: "Bold 14px Lato, sans-serif",
        textAlign: "center",
        margin: 3,
        maxSize: new go.Size(100, NaN),
        alignment: go.Spot.TopCenter,
        alignmentFocus: go.Spot.BottomCenter
      },
        new go.Binding("text"))

    );

  // Some links need a custom to or from spot
  function spotConverter(dir) {
    if (dir === "left") return go.Spot.LeftSide;
    if (dir === "right") return go.Spot.RightSide;
    if (dir === "top") return go.Spot.TopSide;
    if (dir === "bottom") return go.Spot.BottomSide;
    if (dir === "rightsingle") return go.Spot.Right;
  }

  myDiagram.linkTemplate =
    $(go.Link, {
      toShortLength: -2,
      fromShortLength: -2,
      layerName: "Background",
      routing: go.Link.Orthogonal,
      corner: 15,
      fromSpot: go.Spot.RightSide,
      toSpot: go.Spot.LeftSide
    },
      // make sure links come in from the proper direction and go out appropriately
      new go.Binding("fromSpot", "fromSpot", function (d) { return spotConverter(d); }),
      new go.Binding("toSpot", "toSpot", function (d) { return spotConverter(d); }),

      new go.Binding("points").makeTwoWay(),
      // mark each Shape to get the link geometry with isPanelMain: true
      $(go.Shape, { isPanelMain: true, stroke: colors.lightblue, strokeWidth: 10 },
        new go.Binding("stroke", "color", function (c) { return colors[c]; })),
      $(go.Shape, { isPanelMain: true, stroke: "white", strokeWidth: 3, name: "PIPE", strokeDashArray: [20, 40] })
    );


  // build model
  var model = $(go.GraphLinksModel);

  model.nodeDataArray =
    [
      {
        key: 1,
        pos: '-180 -57',
        icon: 'natgas',
        iconWidth: 30,
        iconHeight: 60,
        portHeight: 20,
        text: 'Gas\nCompanies',
        description: 'Provides natural gas liquids (NGLs).',
        caption: 'Gas Drilling Well',
        imgsrc: 'https://upload.wikimedia.org/wikipedia/commons/thumb/5/5d/BarnettShaleDrilling-9323.jpg/256px-BarnettShaleDrilling-9323.jpg'
      },
      {
        key: 2,
        pos: '-180 100',
        icon: 'oil',
        iconWidth: 40,
        iconHeight: 60,
        portHeight: 20,
        text: 'Oil\nCompanies',
        description: 'Provides associated petroleum gas (APG). This type of gas used to be released as waste from oil drilling, but is now commonly captured for processing.',
        caption: 'Offshore oil well',
        imgsrc: 'https://upload.wikimedia.org/wikipedia/commons/thumb/a/ab/Oil_platform_P-51_%28Brazil%29.jpg/512px-Oil_platform_P-51_%28Brazil%29.jpg'
      },
      {
        key: 3,
        pos: '-80 100',
        icon: 'gasprocessing',
        iconWidth: 40,
        iconHeight: 40,
        text: 'Gas Processing',
        description: 'APG processing turns associated petrolium gas into natural gas liquids (NGLs) and stable natural gas (SGN).',
        caption: 'Natural gas plant',
        imgsrc: 'https://upload.wikimedia.org/wikipedia/commons/thumb/6/68/Solohiv_natural_gas_plant_-_fragment.jpg/256px-Solohiv_natural_gas_plant_-_fragment.jpg'
      },
      {
        key: 4,
        pos: '30 -50',
        icon: 'fractionation',
        iconWidth: 40,
        iconHeight: 60,
        text: 'Gas Fractionation',
        description: 'Natural gas liquids are separated into individual hydrocarbons like propane and butanes, hydrocarbon mixtures (naphtha) and liquefied petroleum gases (LPGs).',
        caption: 'Gas Plant',
        imgsrc: 'https://upload.wikimedia.org/wikipedia/commons/thumb/2/20/Gasblok.jpg/256px-Gasblok.jpg'
      },
      {
        key: 5,
        pos: '130 -50',
        icon: 'pyrolysis',
        iconWidth: 40,
        iconHeight: 40,
        color: 'orange',
        text: 'Pyrolysis (Cracking)',
        description: 'Liquefied petroleum gases (LPGs) are transformed into Ethylene, propylene, benzene, and other by-products.',
        caption: 'Pyrolysis plant',
        imgsrc: 'https://upload.wikimedia.org/wikipedia/commons/6/6c/Guelph.jpg'
      },
      {
        key: 6,
        pos: '330 -140',
        icon: 'polymerization',
        iconWidth: 40,
        iconHeight: 40,
        portHeight: 12,
        color: 'red',
        text: 'Basic Polymers',
        description: 'Ethylene and propylene (monomers) are processed into end products using various methods (polymerization).',
        caption: 'Plastics engineering-Polymer products',
        imgsrc: 'https://upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Plastics_engineering-Polymer_products.jpg/256px-Plastics_engineering-Polymer_products.jpg'
      },
      {
        key: 7,
        pos: '330 -55',
        icon: 'polymerization',
        iconWidth: 40,
        iconHeight: 40,
        portHeight: 12,
        color: 'green',
        text: 'Plastics',
        description: 'Polymerization produces PET, glycols, alcohols, expandable polystyrene, acrylates, BOPP-films and geosynthetics.',
        caption: 'Lego Color Bricks',
        imgsrc: 'https://upload.wikimedia.org/wikipedia/commons/thumb/3/32/Lego_Color_Bricks.jpg/256px-Lego_Color_Bricks.jpg'
      },
      {
        key: 8,
        pos: '330 40',
        icon: 'polymerization',
        iconWidth: 40,
        iconHeight: 40,
        portHeight: 12,
        color: 'lightgreen',
        text: 'Synthetic Rubbers',
        description: 'Polymerization produces commodity and specialty rubbers and thermoplastic elastomers.',
        caption: 'Sheet of synthetic rubber coming off the rolling mill at the plant of Goodrich',
        imgsrc: 'https://upload.wikimedia.org/wikipedia/commons/thumb/2/23/Sheet_of_synthetic_rubber_coming_off_the_rolling_mill_at_the_plant_of_Goodrich.jpg/512px-Sheet_of_synthetic_rubber_coming_off_the_rolling_mill_at_the_plant_of_Goodrich.jpg'
      },
      {
        key: 9,
        pos: '330 115',
        color: 'orange',
        portHeight: 22,
        text: 'Intermediates',
        description: 'Produced Ethylene, Propylene, Butenes, Benzene, and other by-products.',
        caption: 'Propylene Containers',
        imgsrc: 'https://upload.wikimedia.org/wikipedia/commons/thumb/2/2e/XVJ-12_Propylene_%288662385917%29.jpg/256px-XVJ-12_Propylene_%288662385917%29.jpg'
      },
      {
        key: 10,
        pos: '330 205',
        icon: 'finishedgas',
        iconWidth: 30,
        iconHeight: 30,
        portHeight: 15,
        text: 'LPG, Naphtha,\nMTBE',
        description: 'Propane, butane, and other general purpose fuels and byproducts.',
        caption: 'Liquid Petroleum Gas Truck',
        imgsrc: 'https://upload.wikimedia.org/wikipedia/commons/thumb/5/52/LPG_Truck.jpg/256px-LPG_Truck.jpg'
      },
      {
        key: 11,
        pos: '330 280',
        icon: 'finishedgas',
        iconWidth: 30,
        iconHeight: 30,
        portHeight: 15,
        text: 'Natural Gas, NGLs',
        description: 'Used for heating, cooking, and electricity generation',
        caption: 'Natural Gas Flame',
        imgsrc: 'https://upload.wikimedia.org/wikipedia/commons/thumb/0/03/%22LPG_flame%22.JPG/512px-%22LPG_flame%22.JPG'
      }
    ];

  model.linkDataArray = [
    {
      from: 1,
      to: 4
    },
    {
      from: 2,
      to: 3,
      label: 'APG'
    },
    {
      from: 3,
      to: 4
    },
    {
      from: 3,
      to: 5,
      toSpot: 'bottom'
    },
    {
      from: 4,
      to: 5
    },
    {
      from: 4,
      to: 5
    },
    {
      from: 3,
      to: 11,
      fromSpot: 'bottom'
    },
    {
      from: 4,
      to: 10,
      fromSpot: 'bottom'
    },
    {
      from: 5,
      to: 6,
      fromSpot: 'rightsingle',
      color: 'orange'
    },
    {
      from: 5,
      to: 7,
      fromSpot: 'rightsingle',
      color: 'orange'
    },
    {
      from: 5,
      to: 8,
      fromSpot: 'rightsingle',
      color: 'orange'
    },
    {
      from: 5,
      to: 9,
      fromSpot: 'rightsingle',
      color: 'orange'
    }
  ];

  myDiagram.model = model;

  loop();  // animate some flow through the pipes

  var opacity = 1;
  var down = true;
  function loop() {
    var diagram = myDiagram;
    setTimeout(function () {
      var oldskips = diagram.skipsUndoManager;
      diagram.skipsUndoManager = true;
      diagram.links.each(function (link) {
        var shape = link.findObject("PIPE");
        var off = shape.strokeDashOffset - 3;
        // animate (move) the stroke dash
        shape.strokeDashOffset = (off <= 0) ? 60 : off;
        // animte (strobe) the opacity:
        if (down) opacity = opacity - 0.01;
        else opacity = opacity + 0.003;
        if (opacity <= 0) { down = !down; opacity = 0; }
        if (opacity > 1) { down = !down; opacity = 1; }
        shape.opacity = opacity;
      });
      diagram.skipsUndoManager = oldskips;
      loop();
    }, 60);
  }

  function onSelectionChanged(e) {
    var node = e.diagram.selection.first();
    if (!(node instanceof go.Node)) return;
    var data = node.data;
    var image = document.getElementById('Image');
    var title = document.getElementById('Title');
    var description = document.getElementById('Description');

    if (data.imgsrc) {
      image.src = data.imgsrc;
      image.alt = data.caption;
    } else {
      image.src = "";
      image.alt = "";
    }
    title.textContent = data.text;
    description.textContent = data.description;

  }
```

## Step 2: Add native GoJS library to your widget as widget dependencies
***Go to Service Portal > Widget ***
- Search for your previous widget created "Custom productionProcess" (custom-gojs-productionProcess) and open the record. 
- On the related tab Dependencies, click on `Edit` button.
- Search for gojs and add to your list
- Click on `Save` button to save the change. 

## Step 3: Create a new Page
***Go to Service Portal > Page > Click New***
- Name: productionProcess - Test Page
- ID: productionProcess
- Click on `Submit` button.
- Once submitted, Click on `Open in Page Designer` related link
- In Page designer, Place `custom-gojs-productionProcess` widget inside a container > row > Column at top location.
- View paget from following link `http://instance-name.service-now.com/sp?id=productionProcess`. 

## Sources
***Any of following links are not under my surveilance or maintenance***

https://github.com/NorthwoodsSoftware/GoJS/blob/master/samples/productionProcess.html
https://gojs.net/latest/intro/toolTips.html
http://g-mops.net/epica_gojs/api/symbols/Diagram.html
Folder Name:

  - ./Service Portal Widgets/Record process flow
    - # Creating Process flow in service portal
## Introduction
In this snippet you will create a custom process flow with a custom page and populated with standard widgets.

## Step 1: Create a new Widget
***Go to Service Portal > Widget > Click New***
- Name: Process Flow
- Id: process-flow
- Click on `submit`

***Body HTML template***
- Copy and paste below `HTML Code` in Widget's HTML Template section
```HTML
<div class="container">
  <div class="process">
    <div class="process-row">
      <div class="process-step" ng-repeat="stateItem in data.processFlow.items">
        <button type="button" disabled="disabled" class="btn btn-default btn-circle" ng-if="c.data.currentValue!=stateItem"><i class="fa fa-check fa-3x" aria-hidden="true"></i></button>
        <button type="button" disabled="disabled" class="btn btn-success btn-circle" ng-if="c.data.currentValue==stateItem"><i class="fa fa-check fa-3x" aria-hidden="true"></i></button>  
        <p>{{stateItem.label}}</p>       	
      </div>
    </div>
  </div>
 </div>
```

***CSS/SCSS***
- Copy and paste below `CSS` in Widget's CSS/SCSS Section
```CSS
.btn-circle {
  width: 40px;
  height: 40px;
  text-align: center;
  padding: 6% 0;
  font-size: 6px;
  line-height: 0.6;
  border-radius: 100%;
}

.process-row {
    display: table-row;
}

.process {
    display: table;     
    width: 100%;
    position: relative;
}

.process-step button[disabled] {
    opacity: 1 !important;
    filter: alpha(opacity=100) !important;
}

.process-row:before {
    top: 20px;
    bottom: 0;
    position: absolute;
    content: " ";
    width: 100%;
    height: 1px;
    background-color: #ccc;
    z-order: 0;
    
}

.process-step {    
    display: table-cell;
    text-align: center;
    position: relative;
    padding-left: 0%;
    padding-right: 5%;
}

.process-step p {
    margin-top:10px;
    
}

.btn-circle.active {
    border: 2px solid #cc0;
}

```

***Server Side Scripts***
- Copy and Paste below `Server-Side Script` in Widget's Server Side Section
```javascript
(function() {
  /* populate the 'data' object */
  /* e.g., data.table = $sp.getValue('table'); */

	data.table  = $sp.getParameter("table");
	data.sys_id = $sp.getParameter("sys_id");

	var gr = new GlideRecord(data.table);
  gr.get(data.sys_id);
  
	var spUtils = new PortalUtils();
  spUtils.getProcessFlows(data,data.table,(data.sys_id == -1),gr);
  
```

## Step 2: Create a Script Include
***Go to Script Includes (System Definition) > Click New***
- Name: PortalUtils
- Accessible from: This application scope only
- Copy and Paste below Server-Side Script in Script Section:
```javascript

  var PortalUtils = Class.create();
  PortalUtils.prototype = Object.extendsObject(PortalUtilsBase, {
	initialize: function() {
	},
	type: 'PortalUtils'
});
```
- Click on `Submit` button.

***Go to Script Includes (System Definition) > Click New***
- Name: PortalUtilsBase
- Accessible from: This application scope only
- Copy and Paste below Server-Side Script in Script Section:
```javascript
var PortalUtilsBase = Class.create();
PortalUtilsBase.prototype = {
	initialize: function() {
  },

getProcessFlows: function(data,table,newRecord, grRecord){
		data.processFlow = {show:false, items:[]};
		
		var grProcessStates = new GlideRecord('sys_process_flow');
		grProcessStates.addQuery("table", table);
		grProcessStates.addQuery("active",true);
		grProcessStates.orderByDesc('order');
		grProcessStates.query();
		
		var matchingFound = false;
		
		while(grProcessStates.next()) {
			data.processFlow.show = true;
			
			var item = {};
			
			item.label = grProcessStates.getValue("label");
			
			if(newRecord){
				item.class_name = "disabled";
			}else if(GlideFilter.checkRecord(grRecord,grProcessStates.getValue("condition"))){
				item.class_name = "completed active";
				matchingFound = true;
			}else{
				if(matchingFound)
					item.class_name = "completed active";
				else
					item.class_name = "disabled";
			}
			
			data.processFlow.items.unshift(item);
		}
		
		if(newRecord && data.processFlow.show && data.processFlow.items.length > 0){
			data.processFlow.items[0].class_name = "active";
		}
 	},

  	type: 'PortalUtilsBase'
};
```
- Click on `Submit` button.

## Step 3: Create a new Page
***Go to Service Portal > Page > Click New***
- Name: process_flow - Test Page
- ID: process_flow
- Click on `Submit` button.
- Once submitted, Click on `Open in Page Designer` related link
- In Page designer, Place `Process Flow` widget inside a container > row > Column at top location.
- View paget from following link `http://instance-name.service-now.com/sp?id=process_flow`. 
Folder Name:

  - ./Service Portal Widgets/Record process flow
    - # Creating Process flow in service portal
## Introduction
In this snippet you will create a custom process flow with a custom page and populated with standard widgets.

## Step 1: Create a new Widget
***Go to Service Portal > Widget > Click New***
- Name: Process Flow
- Id: process-flow
- Click on `submit`

***Body HTML template***
- Copy and paste below `HTML Code` in Widget's HTML Template section
```HTML
<div class="container">
  <div class="process">
    <div class="process-row">
      <div class="process-step" ng-repeat="stateItem in data.processFlow.items">
        <button type="button" disabled="disabled" class="btn btn-default btn-circle" ng-if="c.data.currentValue!=stateItem"><i class="fa fa-check fa-3x" aria-hidden="true"></i></button>
        <button type="button" disabled="disabled" class="btn btn-success btn-circle" ng-if="c.data.currentValue==stateItem"><i class="fa fa-check fa-3x" aria-hidden="true"></i></button>  
        <p>{{stateItem.label}}</p>       	
      </div>
    </div>
  </div>
 </div>
```

***CSS/SCSS***
- Copy and paste below `CSS` in Widget's CSS/SCSS Section
```CSS
.btn-circle {
  width: 40px;
  height: 40px;
  text-align: center;
  padding: 6% 0;
  font-size: 6px;
  line-height: 0.6;
  border-radius: 100%;
}

.process-row {
    display: table-row;
}

.process {
    display: table;     
    width: 100%;
    position: relative;
}

.process-step button[disabled] {
    opacity: 1 !important;
    filter: alpha(opacity=100) !important;
}

.process-row:before {
    top: 20px;
    bottom: 0;
    position: absolute;
    content: " ";
    width: 100%;
    height: 1px;
    background-color: #ccc;
    z-order: 0;
    
}

.process-step {    
    display: table-cell;
    text-align: center;
    position: relative;
    padding-left: 0%;
    padding-right: 5%;
}

.process-step p {
    margin-top:10px;
    
}

.btn-circle.active {
    border: 2px solid #cc0;
}

```

***Server Side Scripts***
- Copy and Paste below `Server-Side Script` in Widget's Server Side Section
```javascript
(function() {
  /* populate the 'data' object */
  /* e.g., data.table = $sp.getValue('table'); */

	data.table  = $sp.getParameter("table");
	data.sys_id = $sp.getParameter("sys_id");

	var gr = new GlideRecord(data.table);
  gr.get(data.sys_id);
  
	var spUtils = new PortalUtils();
  spUtils.getProcessFlows(data,data.table,(data.sys_id == -1),gr);
  
```

## Step 2: Create a Script Include
***Go to Script Includes (System Definition) > Click New***
- Name: PortalUtils
- Accessible from: This application scope only
- Copy and Paste below Server-Side Script in Script Section:
```javascript

  var PortalUtils = Class.create();
  PortalUtils.prototype = Object.extendsObject(PortalUtilsBase, {
	initialize: function() {
	},
	type: 'PortalUtils'
});
```
- Click on `Submit` button.

***Go to Script Includes (System Definition) > Click New***
- Name: PortalUtilsBase
- Accessible from: This application scope only
- Copy and Paste below Server-Side Script in Script Section:
```javascript
var PortalUtilsBase = Class.create();
PortalUtilsBase.prototype = {
	initialize: function() {
  },

getProcessFlows: function(data,table,newRecord, grRecord){
		data.processFlow = {show:false, items:[]};
		
		var grProcessStates = new GlideRecord('sys_process_flow');
		grProcessStates.addQuery("table", table);
		grProcessStates.addQuery("active",true);
		grProcessStates.orderByDesc('order');
		grProcessStates.query();
		
		var matchingFound = false;
		
		while(grProcessStates.next()) {
			data.processFlow.show = true;
			
			var item = {};
			
			item.label = grProcessStates.getValue("label");
			
			if(newRecord){
				item.class_name = "disabled";
			}else if(GlideFilter.checkRecord(grRecord,grProcessStates.getValue("condition"))){
				item.class_name = "completed active";
				matchingFound = true;
			}else{
				if(matchingFound)
					item.class_name = "completed active";
				else
					item.class_name = "disabled";
			}
			
			data.processFlow.items.unshift(item);
		}
		
		if(newRecord && data.processFlow.show && data.processFlow.items.length > 0){
			data.processFlow.items[0].class_name = "active";
		}
 	},

  	type: 'PortalUtilsBase'
};
```
- Click on `Submit` button.

## Step 3: Create a new Page
***Go to Service Portal > Page > Click New***
- Name: process_flow - Test Page
- ID: process_flow
- Click on `Submit` button.
- Once submitted, Click on `Open in Page Designer` related link
- In Page designer, Place `Process Flow` widget inside a container > row > Column at top location.
- View paget from following link `http://instance-name.service-now.com/sp?id=process_flow`. 
Folder Name:

  - ./Service Portal Widgets/Record process flow
    - # Creating Process flow in service portal
## Introduction
In this snippet you will create a custom process flow with a custom page and populated with standard widgets.

## Step 1: Create a new Widget
***Go to Service Portal > Widget > Click New***
- Name: Process Flow
- Id: process-flow
- Click on `submit`

***Body HTML template***
- Copy and paste below `HTML Code` in Widget's HTML Template section
```HTML
<div class="container">
  <div class="process">
    <div class="process-row">
      <div class="process-step" ng-repeat="stateItem in data.processFlow.items">
        <button type="button" disabled="disabled" class="btn btn-default btn-circle" ng-if="c.data.currentValue!=stateItem"><i class="fa fa-check fa-3x" aria-hidden="true"></i></button>
        <button type="button" disabled="disabled" class="btn btn-success btn-circle" ng-if="c.data.currentValue==stateItem"><i class="fa fa-check fa-3x" aria-hidden="true"></i></button>  
        <p>{{stateItem.label}}</p>       	
      </div>
    </div>
  </div>
 </div>
```

***CSS/SCSS***
- Copy and paste below `CSS` in Widget's CSS/SCSS Section
```CSS
.btn-circle {
  width: 40px;
  height: 40px;
  text-align: center;
  padding: 6% 0;
  font-size: 6px;
  line-height: 0.6;
  border-radius: 100%;
}

.process-row {
    display: table-row;
}

.process {
    display: table;     
    width: 100%;
    position: relative;
}

.process-step button[disabled] {
    opacity: 1 !important;
    filter: alpha(opacity=100) !important;
}

.process-row:before {
    top: 20px;
    bottom: 0;
    position: absolute;
    content: " ";
    width: 100%;
    height: 1px;
    background-color: #ccc;
    z-order: 0;
    
}

.process-step {    
    display: table-cell;
    text-align: center;
    position: relative;
    padding-left: 0%;
    padding-right: 5%;
}

.process-step p {
    margin-top:10px;
    
}

.btn-circle.active {
    border: 2px solid #cc0;
}

```

***Server Side Scripts***
- Copy and Paste below `Server-Side Script` in Widget's Server Side Section
```javascript
(function() {
  /* populate the 'data' object */
  /* e.g., data.table = $sp.getValue('table'); */

	data.table  = $sp.getParameter("table");
	data.sys_id = $sp.getParameter("sys_id");

	var gr = new GlideRecord(data.table);
  gr.get(data.sys_id);
  
	var spUtils = new PortalUtils();
  spUtils.getProcessFlows(data,data.table,(data.sys_id == -1),gr);
  
```

## Step 2: Create a Script Include
***Go to Script Includes (System Definition) > Click New***
- Name: PortalUtils
- Accessible from: This application scope only
- Copy and Paste below Server-Side Script in Script Section:
```javascript

  var PortalUtils = Class.create();
  PortalUtils.prototype = Object.extendsObject(PortalUtilsBase, {
	initialize: function() {
	},
	type: 'PortalUtils'
});
```
- Click on `Submit` button.

***Go to Script Includes (System Definition) > Click New***
- Name: PortalUtilsBase
- Accessible from: This application scope only
- Copy and Paste below Server-Side Script in Script Section:
```javascript
var PortalUtilsBase = Class.create();
PortalUtilsBase.prototype = {
	initialize: function() {
  },

getProcessFlows: function(data,table,newRecord, grRecord){
		data.processFlow = {show:false, items:[]};
		
		var grProcessStates = new GlideRecord('sys_process_flow');
		grProcessStates.addQuery("table", table);
		grProcessStates.addQuery("active",true);
		grProcessStates.orderByDesc('order');
		grProcessStates.query();
		
		var matchingFound = false;
		
		while(grProcessStates.next()) {
			data.processFlow.show = true;
			
			var item = {};
			
			item.label = grProcessStates.getValue("label");
			
			if(newRecord){
				item.class_name = "disabled";
			}else if(GlideFilter.checkRecord(grRecord,grProcessStates.getValue("condition"))){
				item.class_name = "completed active";
				matchingFound = true;
			}else{
				if(matchingFound)
					item.class_name = "completed active";
				else
					item.class_name = "disabled";
			}
			
			data.processFlow.items.unshift(item);
		}
		
		if(newRecord && data.processFlow.show && data.processFlow.items.length > 0){
			data.processFlow.items[0].class_name = "active";
		}
 	},

  	type: 'PortalUtilsBase'
};
```
- Click on `Submit` button.

## Step 3: Create a new Page
***Go to Service Portal > Page > Click New***
- Name: process_flow - Test Page
- ID: process_flow
- Click on `Submit` button.
- Once submitted, Click on `Open in Page Designer` related link
- In Page designer, Place `Process Flow` widget inside a container > row > Column at top location.
- View paget from following link `http://instance-name.service-now.com/sp?id=process_flow`. 
Folder Name:

  - ./Service Portal Widgets/Change Notification Preferences
    - ## Notification Preference by Category widget

Portal Widget that shows user notification preferences for a certain category (changed within the options). User can switch his notification on or off. The notification description gets displayed under the notification name.
Folder Name:

  - ./Service Portal Widgets/Change Notification Preferences
    - ## Notification Preference by Category widget

Portal Widget that shows user notification preferences for a certain category (changed within the options). User can switch his notification on or off. The notification description gets displayed under the notification name.
Folder Name:

  - ./Service Portal Widgets/Change Notification Preferences
    - ## Notification Preference by Category widget

Portal Widget that shows user notification preferences for a certain category (changed within the options). User can switch his notification on or off. The notification description gets displayed under the notification name.
Folder Name:

  - ./Service Portal Widgets/Guest Login Modal
    - 
Folder Name:

  - ./Service Portal Widgets/Guest Login Modal
    - 
Folder Name:

  - ./Service Portal Widgets/Export table in portal
    - This widget can be used to download/export a table based on the given query and list view from a button click on the widget
Folder Name:

  - ./Service Portal Widgets/Custom Greetings in portal homepage
    - This code snippet will help you to provide customize greetings to end user when they login to the portal. And the time will be reflected as browser's time zone. By default javascript uses browser's time zone and which is further converted into hours as per the method I used in my clint script code. Below steps needs to be performed to achive this.
1. Clone Homepage-search widget of portal.
2. Update the client script of the cloned widget as per the code prvided in homepage-search-clint.js.
3. Update the HTML as per homepage-search.html.
4. Replace the Homepage-search widget with Custom Homepage-search widget from portal home page by going to Page in designer.
Folder Name:

  - ./Service Portal Widgets/Redirect to different portals based on browser
    - ## Widget to Redirect to different portals based on browser

This widget can be used to redirect users to different portals based on the browsers being used. Simply drop this widget anywhere into the homepage of the portal where you want a redirection to occur(for example */sp*) and you're done. Currently it's having conditions for Internet explorer and Chrome but we can more as and for required. 
Folder Name:

  - ./Service Portal Widgets/Check if user has specific role inside the widget
    - # Check if user has a role within the widget code

Use this code to check inside widget client code to see if user has a role or not. Can be used in scenarios where you want to hide to show part of the widget UI.
Folder Name:

  - ./Service Portal Widgets/ImportXml
    - This widget can be used to import XML files into Servicenow instance.
This is done via portal into an existing table
Folder Name:

  - ./Service Portal Widgets/g_form on SP
    - 
Folder Name:

  - ./Service Portal Widgets/g_form on SP
    - 
Folder Name:

  - ./Service Portal Widgets/Floater Feedback Widget
    - ## Floater Feedback Widget

The attached widget can be used to have a floating link widget on the portal homepage when clicks opens a specific catalog item or a record producer. 
This can be used to gather feedback using a catalog item or create incidents from the portal.

Simply add this widget to the portal homepage anywhere and you can find this present on the side of the homepage. Refer screenshot.

![A test image](demo.JPG)


*Note: You need to update the sys_id of your catalog item. Refer HTML in the .js widget file.*
Folder Name:

  - ./Service Portal Widgets/RecordPickerForListReference
    - The widget is an example record picker that can be used as reference or list field. The field is referring to user table and upon change, the new values are passed to the server side for processing any business logic.
Folder Name:

  - ./Service Portal Widgets/RecordPickerForListReference
    - The widget is an example record picker that can be used as reference or list field. The field is referring to user table and upon change, the new values are passed to the server side for processing any business logic.
Folder Name:

  - ./Service Portal Widgets/iFrame
    - # iFrame Widget
A flexible and reusable widget to display content in an iFrame.

## Configurable Instance Options

The following instance options allow this widget to show external content in a variety of predefined sizes and can update the Service Portal navigation breadcrumb widget and Portal page title.

1. URL

The URL of the external page to embed

2. Size

A selectable list of available size and aspect ratios. These map to css classes defined in the widget.

3. Label

Description text used to support assistive readers and update the ServiceNow breadcrumb widget if it is present on the same page.

4. Set Page Title

A checkbox to override the page title with the Label field.


## Setup the widget

> The entire widget and a demo page has been provided in an update set, `Service Portal - iFrame Widget.xml`, but the follow the steps below to set up the widget from scratch

1. Create a new widget and set **Name** to **iFrame**
2. Copy the contents of `template.html` to the **Body HTML template** window
3. Copy the contents of `style.scss` to the **CSS** window
4. Copy the contents of `server.js` to the **Server script** window
5. Copy the contents of `client.js` to the **Client controller** window
6. Copy the contents of `optionSchema.json` to the **Option schema** window
7. Drag the newly created widget onto any Service Portal page
8. Add the URL of the external content to the Widget instance options

## External content requirements

Displaying an external site in an iFrame is subject to Cross Origin Resource Sharing (CORS) policies. These are enforced by the web browser and configured by the external site. You must ensure that the site you are trying to embed allows it.

You may test the iFrame widget using [Wikipedia](https://en.wikipedia.org/) which does allow embedding.
Folder Name:

  - ./Service Portal Widgets/iFrame
    - # iFrame Widget
A flexible and reusable widget to display content in an iFrame.

## Configurable Instance Options

The following instance options allow this widget to show external content in a variety of predefined sizes and can update the Service Portal navigation breadcrumb widget and Portal page title.

1. URL

The URL of the external page to embed

2. Size

A selectable list of available size and aspect ratios. These map to css classes defined in the widget.

3. Label

Description text used to support assistive readers and update the ServiceNow breadcrumb widget if it is present on the same page.

4. Set Page Title

A checkbox to override the page title with the Label field.


## Setup the widget

> The entire widget and a demo page has been provided in an update set, `Service Portal - iFrame Widget.xml`, but the follow the steps below to set up the widget from scratch

1. Create a new widget and set **Name** to **iFrame**
2. Copy the contents of `template.html` to the **Body HTML template** window
3. Copy the contents of `style.scss` to the **CSS** window
4. Copy the contents of `server.js` to the **Server script** window
5. Copy the contents of `client.js` to the **Client controller** window
6. Copy the contents of `optionSchema.json` to the **Option schema** window
7. Drag the newly created widget onto any Service Portal page
8. Add the URL of the external content to the Widget instance options

## External content requirements

Displaying an external site in an iFrame is subject to Cross Origin Resource Sharing (CORS) policies. These are enforced by the web browser and configured by the external site. You must ensure that the site you are trying to embed allows it.

You may test the iFrame widget using [Wikipedia](https://en.wikipedia.org/) which does allow embedding.
Folder Name:

  - ./Service Portal Widgets/Incident Sound Alerts
    - ## Incident Sound Alerts Widget

This widget can be used to get sound alerts whenever a incident is created can be a major incident/high priority incident or a incident assigned to a particular group. We can place this widget on a portal page(which is open on a monitoring screen or system) and whenever the conditions are it will generate a sound alert.  Note: Currently the widget is configured to geneate alerts for Major incidents accepted. 
Folder Name:

  - ./Service Portal Widgets/Spiderman Animation
    - To use this widget, follow the below steps:

1. Create a new widget and copy the html, style and client script in the widget.
2. Upload the 2 images- Green goblin image and Spiderman Image, in the image table. Also, upload the audio in audio table.Use the same name given in the tables in the widget
3. Create a page and add the widget to it(12 GRID LAYOUT).
4. Change the width of `.card-overlay` class accordingly.
5. (Optional) On the portal page of this widget , open - Edit container background and change the width to fluid. 

Here is Page Content structure

### Page Content
##### Page: Marvel

    Marvel - Container1
	    Row1
		    Column1
			    Instance: (Spiderman)
Folder Name:

  - ./Service Portal Widgets/Upload Files
    - # Service Portal Widget - "Add attachments" form

This widget is using the 'Attachment API - POST /now/attachment/file' to upload multiple files on form submit.

The result will appear in the console or check directly the record.
Folder Name:

  - ./Service Portal Widgets/Upload Files
    - # Service Portal Widget - "Add attachments" form

This widget is using the 'Attachment API - POST /now/attachment/file' to upload multiple files on form submit.

The result will appear in the console or check directly the record.
Folder Name:

  - ./Service Portal Widgets/Card Image Link
    - # Card Image Link Widget

Provides an easy to use and nice looking card widget to add to Service Portal pages

# Set up 
![Image of Card set up](doc/card_setup.png)

# End Result
![Image of Card result](doc/card_result.png)
Folder Name:

  - ./Service Portal Widgets/Card Image Link
    - # Card Image Link Widget

Provides an easy to use and nice looking card widget to add to Service Portal pages

# Set up 
![Image of Card set up](doc/card_setup.png)

# End Result
![Image of Card result](doc/card_result.png)
Folder Name:

  - ./Service Portal Widgets/Set Variables By Url
    - ## Use case
Sometimes you want to share a link to a catalog item on the portal and you want to pre-set some variables.  Like when you make documentation and you want to pre-categorize a ticket with information but you dont show all that.

So you build your link `https://{{instance}}/sp?id=sc_cat_item&sys_id={{itemSysID}}&description=I'cant%20access%20ServiceNow`

Which would set the description variable to "I can't access ServiceNow"

## Set up

1.  Create the widget
2.  Goto the https://{{instance}}/nav_to.do?uri=sp_page.do?sysparm_query=id=sc_cat_item
3.  Click the "Open in Designer" link at the bottom
4.  Add your widget anywhere as it has no html it will not render any elements.
Folder Name:

  - ./Service Portal Widgets/Create diagram using Highcharts library
    - # Creating spider web using Highcharts
## Introduction
In this snippet you will create a custom spider web using a custom page and populating data using Highcharts native library

## Step 1: Create a new Widget
***Go to Service Portal > Widget > Click New***
- Name: Custom productionProcess
- Id: custom-gojs-productionProcess
- Click on `submit`

***Body HTML template***
- Copy and paste below `HTML Code` in Widget's HTML Template section
```HTML
<div>  
	<!-- chart -->
    <div id="container"></div>
    <p class="highcharts-description">
        A spiderweb chart or radar chart is a variant of the polar chart.
        Spiderweb charts are commonly used to compare multivariate data sets,
        like this demo using six variables of comparison.
    </p>
</div>
```

***CSS/SCSS***
- Copy and paste below `CSS` in Widget's CSS/SCSS Section
```CSS
/* to be completed */
```
***Client Side Scripts***
- Copy and Paste below `Script` in Widget's Client Side Section
```javascript
api.controller=function($rootScope, $scope, $window, $interval, spUtil) {
  /* widget controller */
	var c = this;

	/** Chart source: https://www.highcharts.com/demo/polar-spider*/
	var options = {
        credits: {
            enabled: false
        },

        chart: {
            renderTo: 'container', // change chart_id if needed
            polar: true,
            type: 'line'
        },

    accessibility: {
        description: 'A spiderweb chart compares the allocated budget against actual spending within an organization. The spider chart has six spokes. Each spoke represents one of the 6 departments within the organization: sales, marketing, development, customer support, information technology and administration. The chart is interactive, and each data point is displayed upon hovering. The chart clearly shows that 4 of the 6 departments have overspent their budget with Marketing responsible for the greatest overspend of $20,000. The allocated budget and actual spending data points for each department are as follows: Sales. Budget equals $43,000; spending equals $50,000. Marketing. Budget equals $19,000; spending equals $39,000. Development. Budget equals $60,000; spending equals $42,000. Customer support. Budget equals $35,000; spending equals $31,000. Information technology. Budget equals $17,000; spending equals $26,000. Administration. Budget equals $10,000; spending equals $14,000.'
    },

    title: {
        text: 'Budget vs spending',
        x: -80
    },

    pane: {
        size: '80%'
    },

    xAxis: {
        categories: ['Sales', 'Marketing', 'Development', 'Customer Support',
            'Information Technology', 'Administration'],
        tickmarkPlacement: 'on',
        lineWidth: 0
    },

    yAxis: {
        gridLineInterpolation: 'polygon',
        lineWidth: 0,
        min: 0
    },

    tooltip: {
        shared: true,
        pointFormat: '<span style="color:{series.color}">{series.name}: <b>${point.y:,.0f}</b><br/>'
    },

    legend: {
        align: 'right',
        verticalAlign: 'middle',
        layout: 'vertical'
    },

    series: [{
        name: 'Allocated Budget',
        data: [43000, 19000, 60000, 35000, 17000, 10000],
        pointPlacement: 'on'
    }, {
        name: 'Actual Spending',
        data: [50000, 39000, 42000, 31000, 26000, 14000],
        pointPlacement: 'on'
    }],

    responsive: {
        rules: [{
            condition: {
                maxWidth: 500
            },
            chartOptions: {
                legend: {
                    align: 'center',
                    verticalAlign: 'bottom',
                    layout: 'horizontal'
                },
                pane: {
                    size: '70%'
                }
            }
        }]
    }
};
	
  /*Generate chart*/
	var chart = new Highcharts.Chart(options);
  
  /* improvements: next step would be to have a ng-selector in HTML and use record watcher to keep data up do date */
	
};
```

## Step 2: Add native Highcharts library to your widget as widget dependencies
***Go to Service Portal > Widget ***
- Search for your previous widget created "Custom Spider Web" (custom-spider-web) and open the record. 
- On the related tab Dependencies, click on `Edit` button.
- Search for PA Widget (4fbe3df5673322002c658aaad485ef29) and add to your list.
- Click on `Save` button to save the change. 

## Step 3: Create a new Page
***Go to Service Portal > Page > Click New***
- Name: spiderweb - Test Page
- ID: spiderweb
- Click on `Submit` button.
- Once submitted, Click on `Open in Page Designer` related link
- In Page designer, Place `custom-spider-web` widget inside a container > row > Column at top location.
- View paget from following link `http://instance-name.service-now.com/sp?id=spiderweb`. 

## Sources
***Any of following links are not under my surveilance or maintenance***

https://github.com/NorthwoodsSoftware/GoJS/blob/master/samples/productionProcess.html
https://gojs.net/latest/intro/toolTips.html
http://g-mops.net/epica_gojs/api/symbols/Diagram.html
Folder Name:

  - ./Service Portal Widgets/Konami Code Easter Egg
    - # Konami Code Easter Egg

Put this code in the client controller of a widget to listen for the Konami Code. By default it just opens a modal notifying the user that the konami code as activated. Modify to do whatever fun things you want.
Folder Name:

  - ./Service Portal Widgets/Batman Animation
    - In order to use the widget, follow the below steps:

1.Create a new widget and copy the html, style and client script in the widget.

2.Upload the 2 images (Batman logo and Batman Background Image) in the image table.

3.Update the widget html with the correct image names.

4.Create a page and add the widget to it(12 GRID LAYOUT) and also add the below styling to page CSS.

****section {
  background-image: url('Batman.jpg');
  background-size: cover;
  background-repeat: unset;
}**
**

Here is Page Content structure


![image](https://user-images.githubusercontent.com/28950517/135977861-16358193-2df6-460a-ba6c-094c5ba3955d.png)
Folder Name:

  - ./Service Portal Widgets/Open in Platform
    - Widget will create a button that will only be visable to users with the itil role that will take them to the same record in platform. will work with the form and standard ticket pages (or anywhere with the table and sysId in the url.

see also [on Share](https://developer.servicenow.com/connect.do#!/share/contents/6592535_open_in_platform_widget?t=PRODUCT_DETAILS)
Folder Name:

  - ./Service Portal/sp-modal
    - This script is used to generate a popup on the Service Portal page, you can update the html based on your need.

If a callback is needed, use the .then() part of the spModal and add any functions/statements to it as required.
Folder Name:

  - ./Service Portal/sn-watchlist
    - # sn-watchlist

`sn-watchlist` is a custom directive that you can use to create a watchlist like field within your widgets.

![watchlist in action](sn-watchlist.gif)

| Property    | Description                                                                                                  |
| ----------- | ------------------------------------------------------------------------------------------------------------ |
| placeholder | specify a placeholder for the input                                                                          |
| label       | specify a label                                                                                              |
| ngModel     | allows to bind a model holding a list of seleted users. the user object has properties `sys_id, name, email` |
| ngChange    | expression to execute when the model is changed element                                                      |

## Installation

1. create an angular provider with the name `snWatchlist`
2. paste the content of `snWatchListDirective.js` into the client script field
3. associate the angular provider with the widget where you would like to use it
4. you can now use it as described within [example usage](#example-usage)

> :information_source: for more info visit [docs](https://docs.servicenow.com/bundle/rome-servicenow-platform/page/build/service-portal/task/angular-providers.html)

## Example usage

**HTML Template**

```html
<sn-watchlist
  label="Users watchlist"
  placeholder="Search from list or type in an email"
  ng-model="c.watchlist"
  ng-change="c.watchlistChanged()"
></sn-watchlist>
```

**Client controller**

```javascript
api.controller = function () {
  /* widget controller */
  var c = this;

  c.$oninit = function () {
    c.watchlist = [];
  };

  c.watchlistChanged = function () {
    var watchList = c.watchlist
      .map(function (user) {
        return user.sys_id || user.email;
      })
      .join(",");

    console.log(watchList);
  };
};
```
Folder Name:

  - ./Service Portal/spGlideAjax
    - # spGlideAjax

This is a demo of promise like service which allows to make a GlideAjax call directly from the controller function.
The service has a single method called `getAnswer` which returns a promise, which is then resolved directly to the answer attribute from the XML response.
The method accepts 3 parameters:
* `processor` - name of the client callable script include
* `name` - method name you would like to execute
* `params` - object containing additional parameters

## Installation

1. create an angular provider with the name `spGlideAjax`
2. paste the content of `spGlideAjaxService.js` into the client script field
3. associate the angular provider with the widget where you would like to use it
4. you can now use it as described within [example usage](#example-usage)

> :information_source: for more info visit [docs](https://docs.servicenow.com/bundle/rome-servicenow-platform/page/build/service-portal/task/angular-providers.html)

## Example usage

```javascript
api.controller = function (spGlideAjax) {
  /* widget controller */
  var c = this;

  c.getGlideDateTime = function (ms) {
    spGlideAjax
      .getAnswer("DateTimeUtils", "msToGlideDateTime", {
        sysparm_value: ms,
      })
      .then(
        function (resp) {
          console.log(resp);
        },
        function (error) {
          console.error(error);
        }
      );
  };
};
```
Folder Name:

  - ./Service Portal/dark-mode-switcher
    - # Dark mode switcher ☀️/🌑

This is a simple demonstration of achieving a dark mode switcher for Employee Center portal. The switcher itself allows user to quickly toggle between multiple color modes:

* OS Default - uses the color scheme based on OS settings
* Dark - uses the dark color scheme ignoring OS settings
* Light - uses the light color scheme ignoring OS setting

![A quick demo of a dark mode in action](demo.gif)

This implementation doesn't need to clone any widget 🤯 and was originally build for Tokyo release 🗼 of Employee Center portal. Before trying to use it in your environment consider the following 👇:
* it was built just for fun 🎉 and as a personal challenge
* not all colors have been adjusted for dark mode, I even barely tested the homepage 🦄
* it might break in any upcoming releases 🐛
* finding the right color balance with good contrast ratio for all pages might require some additional effort and patience 
* consider how all of your images will look on both color schemes (you might even end with providing 2 color variants)
* let's hope that the nextgen portal will have this built-in OOTB 🤞

## Implementations Details

### user preference
For storing the user's preference of color scheme I created a user preference with the name `preferred_color_scheme`. I suggest to create a global one with the value `os-default`.

### Angular Providers
The following angular providers need to be created and attached to the `Employee Center Header` widget. You can create those via `m2m_sp_ng_pro_sp_widget` table.

[themeSwitcherMenu](themeSwitcherMenu.js) - a directive that will allow user to change color scheme

[avatarDropDown](avatarDropDown.js) - a "hacky" directive that will inject our theme switcher into the portal header next to the avatar profile menu

### Portal Theme

[EC Theme](portal_theme.scss) - just put this into your portal theme

### CSS Include

[EC Dark Mode](dark_mode.scss) - put this into your theme as a CSS Include

Folder Name:

  - ./Service Portal/dark-mode-switcher
    - # Dark mode switcher ☀️/🌑

This is a simple demonstration of achieving a dark mode switcher for Employee Center portal. The switcher itself allows user to quickly toggle between multiple color modes:

* OS Default - uses the color scheme based on OS settings
* Dark - uses the dark color scheme ignoring OS settings
* Light - uses the light color scheme ignoring OS setting

![A quick demo of a dark mode in action](demo.gif)

This implementation doesn't need to clone any widget 🤯 and was originally build for Tokyo release 🗼 of Employee Center portal. Before trying to use it in your environment consider the following 👇:
* it was built just for fun 🎉 and as a personal challenge
* not all colors have been adjusted for dark mode, I even barely tested the homepage 🦄
* it might break in any upcoming releases 🐛
* finding the right color balance with good contrast ratio for all pages might require some additional effort and patience 
* consider how all of your images will look on both color schemes (you might even end with providing 2 color variants)
* let's hope that the nextgen portal will have this built-in OOTB 🤞

## Implementations Details

### user preference
For storing the user's preference of color scheme I created a user preference with the name `preferred_color_scheme`. I suggest to create a global one with the value `os-default`.

### Angular Providers
The following angular providers need to be created and attached to the `Employee Center Header` widget. You can create those via `m2m_sp_ng_pro_sp_widget` table.

[themeSwitcherMenu](themeSwitcherMenu.js) - a directive that will allow user to change color scheme

[avatarDropDown](avatarDropDown.js) - a "hacky" directive that will inject our theme switcher into the portal header next to the avatar profile menu

### Portal Theme

[EC Theme](portal_theme.scss) - just put this into your portal theme

### CSS Include

[EC Dark Mode](dark_mode.scss) - put this into your theme as a CSS Include

Folder Name:

  - ./Transform Map Scripts/Conditional Coalesce
    - **Conditional Coalesce on Trasnform Maps**

When you have more than one field you want to coalesce based on some conditions, you can create a field mapping where source is a script and target field is SYS_ID.
You can put your conditional logic in the source script to do a conditional coalesce. Return the sys_id of the matched record for the transform to update it. Return -1 when there is not a match and you want to create a new record.

**Example configuration**

![Configuration](conditional_coalesce.png)
Folder Name:

  - ./Transform Map Scripts/Verify headers of a CSV attached file
    - 
Folder Name:

  - ./Transform Map Scripts/Choice Field Validator
    - # **Choice Field Validator**

Function that returns the value of a choice by its display value. Initially created to be used in field map scripts.
Used to return the choice even if the instance is in different language.


## *Important points*
- It is imperative that the display value in the transform map table exists in the instance
- It is possible to validate the values of choices dependent on other choices
- To get the dependent choice you need set and static value or run the function for the first choice and then with the dependent choice (as in the second example).


## **Example configuration**

1. Category validation:
![categoryvalidation](choice_validador1.png)

2. Category and subcategory validation:
![categorysubcategoryvalidation](choice_validador1.png)


In these previous cases we used the validator because some users use Portuguese language and all options in the excel are in English. With the functions we don't need to worry about the different languagues.
Folder Name:

  - ./Server Side/Create Tiny Url with API's
    - we can turn any servicenow url to tiny url with the code attached.

it just need a user authentication details, any user who dont even have any roles also fine, the user just need to able to login to instance.

example:
We can turn this url :
https://devxxxx.service-now.com/incident_list.do?sysparm_query=caller_id%3D681ccaf9c0a8016400b98a06818d57c7%5Epriority%3D1%5Estate%3D2%5Esys_updated_by%3Dadmin%5Eshort_description%3DManager%20can%27t%20access%20SAP%20Controlling%20application&sysparm_first_row=1&sysparm_view=


To this:
https://devxxxx.service-now.com/incident_list.do?sysparm_tiny=cb4c40e12fd61d10c083d0ccf699b62a
Folder Name:

  - ./Server Side/Restart a workflow via any server side script
    - Use this to attach a new workflow to your old records.
Folder Name:

  - ./Server Side/DiscoveryDeviceHistory
    - 
Folder Name:

  - ./Server Side/ExecuteWorkOnMidServer
    - The snippet can be used to dynamically execute any work on the mid server. You could run any commands on a server, powershell scripts, LDAP queries and other functions depending on the output probes which are supported by ServiceNow. You need to be aware of the ECC queue output and input structure used by ServiceNow to issue these commands. To get these formats, you could execute the same functionality and monitor the ECC queue for its structure. 

Sample Usage.

For eg, inorder to query on LDAP for all users whose name is starting with A. You could call the following function.

```
var outputId = executeWorkOnMid('Mid-Server-01', 'LDAPQuery', 'LDAPBrowseProbe', 'fdc4cd3fdb6a8f003a339e04db96199d',  '<?xml version="1.0" encoding="UTF-8"?><parameters><parameter name="type" value=""/><parameter name="value" value="(&amp;(objectClass=person)(cn=A*))"/><parameter name="chars" value="*"/></parameters>'));
```
```
The payload argument contains the LDAP query as (&amp;(objectClass=person)(cn=A*)) which would return the results in an input ECC queeue
```
The outputId can then be passed to the second function to fetch the response as an XML object. The ECC queue works asynchronously, so may need to wait for few seconds until the response is received in the input queue.

```
gs.sleep(5000);
var xmlResponse = fetchResponseFromMid(outputId);
//gs.print(xmlResponse);
```
Folder Name:

  - ./Server Side/getUserGroupMembers
    - Script to get members of groups which our users also belongs to.

example: added Abel to 2 HR groups and then printing the names of members who belong to those groups.

![image](https://user-images.githubusercontent.com/46869542/193464977-53b613db-650b-452c-ac72-fbee5196605f.png)
Folder Name:

  - ./Server Side/Update Variable Choices
    - Programatically update add a new choice for a service catalog variable and reorder all choices alphabetically. Can be helpful as part of a workflow where a fulfiller chooses logic to "update the list" variable, such as a small product or category list that may require ongoing updates as a result of fulfilling the request. Often unlisted choices are handled with an "Other" option and a text field to include the unlisted option. This script will take the value from the "Other" variable and add it to the choice list in the workflow.
Folder Name:

  - ./Server Side/CreateUpdateCIThroughIRE
    - ServiceNow CMDB should be updated through the Identification and Reconciliation Engine. There are several legacy ways of populating CMDB and the most commonly used ways are via transform maps or through any external integration scripts. Whenver data is added to the CMDB, it should go through the IRE as it helps you maintain the quality of your CI data by avoiding duplicates and ensuring that only authorized source can updated the data in your CMDB. The code snippet allows you to update CMDB through IRE thereby reducing the maintanance effort required on your CMDB. You could call it from a transform map script, integration scripts or via any other scripted methods used to integrate.

Sample Usage
````
//This has the list of all CIs and its related CI that need to be added to CMDB
var items = [{
        "className": 'cmdb_ci_win_server',
        "values": {
            "name": 'xServerV1',
            "serial_number": "12342-drrrcf-3332dd-2222",
            "ip_address": "10.20.30.40",
            "mac_address": "ZFSTFS-XXJSDD-QWWJES-AJDH2D",
            "ram": "4096",
            "os": "Windows 2016 Datacenter"
        }
    },
    {
        "className": 'cmdb_ci_app_server_tomcat',
        "values": {
            "name": 'Tomcat@ip-10.20.30.40:8005',
            "version": '7.0.42',
            "install_directory": "sdd",
            "running_process_key_parameters": "ss",
            "server_port": "8005"
        }
    }
];

//This defines the relationship between the CIs mentioned in the items array and created the same in cmdb_rel_ci table
var relations = [{
    "child": 0,
    "parent": 1,
    "type": "Runs on::Runs"
}];

createOrUpdateCIThroughIRE(items, relations, "ServiceNow");
````````
Folder Name:

  - ./Server Side/Get all variables of catalog item
    - sometimes we need to get all varibles related to Catalog item / record producer, but as some varibles are placed in variable set its not that easy to get all.

for this we can use addJoinQuery of GlideRecord. so we can get all varibles related to Catalog item / record producer with attached script.

example output:

![image](https://user-images.githubusercontent.com/46869542/193516504-901c2456-8fb4-46b2-ac64-b236976f258b.png)
Folder Name:

  - ./Server Side/Get all Catalog items associated to variable set
    - Use this script to get List of Catalog Items associated to the Variable set.
Folder Name:

  - ./Server Side/User Criteria
    - Use this script to determine if a user passes an array of user criterias


userID - String of a sys_user sys_id

userCriteria - Array of user_criteria sys_ids to check again
Folder Name:

  - ./Server Side/Restart Flow on RITM
    - Restart a flow designer flow on a Requested Item.  I use this in a UI Action, but it could also be modified and used in a background script if needed.
Folder Name:

  - ./Server Side/CheckTableExtension
    - The snippet validates whether a child table is extended from a parent table. You could provide both the table names as input and it would respond back with a boolean output.

Sample Usage

gs.info(isTableExtended("cmdb_ci", "cmdb_ci_win_server"));  //true

gs.info(isTableExtended("cmdb_ci", "cmdb_ci_hardwares"));   //false
Folder Name:

  - ./Server Side/Decrypt Password2 Field
    - decrypterPassword2.js will dycrpt a password2 field
Folder Name:

  - ./Server Side/Create Admin Users
    - # Purpose
After first login to a freshly provisioned ServiceNow instance it is recommended creating personalized admin accounts. The following script will do the job for you. Just pass the most important properties to the method and a new user is being created with some preconfigured values such as roles and preferences.
# Usage
```javascript
var strUserSysID = createAdminUser(
  'john.doe',
  'John',
  'Doe',
  'john.doe@example.com'
);

if (strUserSysID != null) {
    //user has been created successfully
}
```
Folder Name:

  - ./Server Side/Random Password generator
    - This script is used to generate a random password, you can update the length parameter to adjust the length of password.
Folder Name:

  - ./Server Side/Phone Number formating(US Region)
    - Use this script to format Phone Number in standard format 3-3-4 example if phone is  1234567891  then output will be 123-456-7891
