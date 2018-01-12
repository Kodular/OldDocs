# FusionTablesControl

A non-visible component that communicates with Google Fusion Tables. Fusion Tables let you store, share, query and visualize data tables; this component lets you query, create, and modify these tables.

This component uses the Fusion Tables API V2.0.

Applications using Fusion Tables must authenticate with Google's servers. There are two ways this can be done. The first way only uses an API Key which you (the developer) obtain. With this approach end-users must also login to access a Fusion Table.

The second approach is to use Service Authentication. With this approach you create credentials and a special "Service Account Email Address" which allows end-users to edit your Fusion Tables without logging in; your service account authenticates all access.

---

### Using the FusiontablesControl Component

#### Creating Fusion Tables

You will probably want to create your own Fusion Tables to experiment with as you are developing your apps. This is as easy as creating a Google document, if you are familiar with that process. Here are the steps:

On the web, login to your Gmail account or any other Google service (e.g., Drive, YouTube). Navigate to Google Drive.
Click the New button and navigate to More. If you do not see a Google Fusion Tables option, select Connect more apps and scroll through the page of Google services to find the Fusion Tables service and connect it to your Google Drive.
You may want to view some of the examples and work through a tutorial (e.g. Pizza Party Tutorial) to learn the basics.
Click the See my tables button (top right of the page). This will bring you to your own page.
You should see a list of your own tables or tables that have been shared with you (possibly none).
Use the Create button to create a new table. Give it some column names and save it.
Click on the Share button (top right) to modify the table's permissions.

#### Creating a Fusiontables App

When you drag the FusiontablesControl component onto the Designer, don't forget to set its ApiKey property, which is initially blank. You should copy this from your Google Developers Console and paste it into the property field.

To get an API key, follow these instructions.

Go to your Google Developers Console and login if necessary.
Under APIs & auth select the APIs item from the menu on the left.
Choose the Fusion Tables API from the list provided and turn it on.
On the left bar, select the Credentials item.
Under Public API access click Create new Key, choose Android key and click Create to generate an API key.
Your API key(s) will appear in the pane next to "Public API access". You must provide that key as the value for the ApiKey property in your Fusion Tables app.

Once you have an API key, set the value of the Query property to a valid Fusiontables SQL query and call SendQuery to execute the query. App Inventor will send the query to the Fusion Tables server and the GotResult block will fire when a result is returned from the server. Query results will be returned in CSV format, and can be converted to list format using the "list from csv table" or "list from csv row" blocks.

Note that you do not need to worry about UTF-encoding the query. But you do need to make sure the query follows the syntax described in the reference manual, which means that things like capitalization for names of columns matters, and that single quotes must be used around column names if there are spaces in them.

To set up Service Authentication for your Fusion Table, follow these additional steps:

In the Google APIs Console under APIs & auth select the APIs item from the menu on the left.
Click the Create new Client ID button. Select the Service account option, and click Create Client ID.
A file called the KeyFile (ends in extension .p12) will automatically download onto your computer. Save it in a place you will remember. Once the creation is complete, you will get a table with your Service Account information.
In the designer window of App Inventor, select the FusionTablesControl. In the properties pane, add the ServiceAccountEmail (from the table on the console), upload the KeyFile, and check the UseServiceAuthentication box.
Share the Fusion Table with your ServiceAccountEmail, and give it editing permissions, just like you would share any other Google Doc with an email address.

---

### Properties

#### ApiKey

Your Google API Key. See above for details on obtaining an API key.

#### KeyFile

Specifies the path of the private key file. This key file is used to get access to the FusionTables API through Service Authentication.

#### Query

The query to send to the Fusion Tables API.
For legal query formats and examples, see the Fusion Tables API v2.0 reference manual.

Note that you do not need to worry about UTF-encoding the query. You must make sure the query follows the syntax described in the reference manual. Note that capitalization for names of columns is necessary and that single quotes must be used around column names if there are spaces in them.

#### ServiceAccountEmail

The Service Account Email Address used for Service Authentication.

#### UseServiceAuthentication

Indicates whether a service account should be used for authentication.

---

### Events

#### GotResult(text result)

Indicates that the Fusion Tables query has finished processing and returned with a result. The result of the query will generally be returned in CSV format, and can be converted to list format using the "list from csv table" or "list from csv row" blocks.

---

### Methods

#### DoQuery()

DEPRECATED. This block is deprecated as of the end of 2012. Use SendQuery instead.

#### ForgetLogin()

Forget the end-user's login credentials. Has no effect on Service Authentication.

#### GetRows(text tableId, text columns)

Gets all the rows from a specified Fusion Table. The tableId field (required) is the id of the Fusion Table. The columns field is a comma-separated list of the columns to retrieve.

#### GetRowsWithConditions(text tableId, text columns, text conditions)

Gets all the rows from a Fusion Table that meet certain conditions. The tableId field (required) is the id of the Fusion Table. The columns field is a comma-separated list of the columns to retrieve. The conditions field specifies what rows to retrieve from the table (for example, the rows in which a particular column value is not null).

#### InsertRow(text tableId, text columns, text values)

Inserts a row into the specified Fusion Table. The tableId field is the id of the Fusion Table. The columns field is a comma-separated list of the columns into which to insert values. The values field specifies what values to insert into each column.

#### SendQuery()

Send the query to the Fusion Tables server.
