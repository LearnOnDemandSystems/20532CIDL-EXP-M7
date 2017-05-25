
<!---
Version: 1.0 
-->
# Exercise 1: Implementing Azure Storage Blobs
## INTRODUCTION MESSAGE
In this exercise, you will:  
  
Create a blob container by using the Portal.  
Add blob files to the container.  
Access the blob files in the container.  
  
The main tasks for this exercise are as follows:  
Sign in to the Azure Portal.  
Create a container by using the Portal.  
Add and access blob files in your container.
## COMPLETION MESSAGE
Results: After completing this exercise, you will have created a blob container by using the Portal and viewed the blobs in the container.
### Login as Student
Login as Student with a password of Pa$$w0rd.

#### :bulb: KNOWLEDGE
You can use the Commands menu and choose Ctrl\+Alt\+Delete then click Student and enter Pa$$w0rd and press Enter. You can also use the Command menu and choose Paste/Paste Password instead of typing the password manually.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666558.jpg
>* ShowAutomatically = No





### On the Start screen, click Internet Explorer
On the Start screen, click the Internet Explorer tile

#### :bulb: KNOWLEDGE
Ignore updates to OneDrive

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666559.jpg
>* ShowAutomatically = No





### Go to the new Azure Portal
Go to https://portal.azure.com. Enter the email address of your Microsoft account associated with your Azure subscription. Then enter the password for your Microsoft account. Check Keep me signed in. Click Sign In.

#### :bulb: KNOWLEDGE
Before starting this lab, you must have completed the lab in Module 2. All work in this lab is done within vm20532 created in the lab in Module 2. Start and Connect via Azure Portal.  
  
If you see a pop-up for Skype for Business click Don't Enable.  
  
Ignore any updates to OneDrive

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666560.jpg
>* ShowAutomatically = No



#### :calling: COMMAND
```TypeText
https://portal.azure.com
```


### Browse Virtual Machines
In the navigation pane on the left side of the Azure Portal, click Virtual Machines.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666561.jpg
>* ShowAutomatically = No





### Start the VM
Click the vm20532 VM that was created in the lab in Module 2 for development. In the Overview blade, if the VM is stopped, click Start and wait for the VM to start up. This may take a few minutes.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666562.jpg
>* ShowAutomatically = No





### Connect to the VM via RDP
When the vm20532 VM has started, click Connect.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666563.jpg
>* ShowAutomatically = No





### Allow pop-ups
If presented with a message box that shows a pop-up has been blocked, select Options for this site and choose Always Allow. Then click Connect again.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/672214.jpg





### Click Open
When presented with the RDP download popup at the bottom of the screen, click Open.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/672215.jpg





### In the Remote Desktop Connection dialog box:
In the Remote Desktop Connection dialog box, perform the following steps:  
a. Click Don’t ask me again for connections to this computer to prevent this dialog box from displaying again.  
b. Click Connect.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666564.jpg
>* ShowAutomatically = No





### In the Windows Security dialog box:
In the Windows Security dialog box, perform the following steps:  
a. For the User name dialog box, provide the value, Student.  
b. For the Password dialog box, provide the value, AzurePa$$w0rd.  
c. Click OK.

#### :bulb: KNOWLEDGE
Note: If you computer is on a domain, you may need to add a backslash before the username to "escape" the domain.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666565.jpg
>* ShowAutomatically = No





### In the Remote Desktop Connection dialog box:
In the Remote Desktop Connection dialog box, perform the following steps:  
a. Verify if the Remote certificate name matches the name of your virtual machine.  
b. Click Don’t ask me again for connections to this computer to prevent this dialog box from displaying again.  
c. Click Yes.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666566.jpg
>* ShowAutomatically = No





### Close Server Manager, if necessary
If you just started the VM, Server Manager will start automatically after 30 seconds. When it starts, you can close it.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666567.jpg
>* ShowAutomatically = No





### On the Start screen, open Internet Explorer
On the Start screen, click the Internet Explorer tile.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666568.jpg
>* ShowAutomatically = No





### Sign in to the Azure Portal
Sign in to the Azure Portal at https://portal.azure.com.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666569.jpg
>* ShowAutomatically = No



#### :calling: COMMAND
```TypeText
https://portal.azure.com
```


### Browse Storage Accounts
In the Browse blade, click Storage accounts. In the Storage accounts blade that displays, view the list of Storage instances.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666570.jpg





### Open storage account with the prefix stor20532
In the list of Storage instances, locate the storage account with the prefix stor20532. Click the name of the storage account to go to its Overview blade.





### View the list of your Blob containers.
In the stor20532\[Your Name Here\] blade that displays, click the Blobs tile.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666572.jpg





### View the list of your containers, Add a new one:
In the Blob service blade that displays, view the list of your containers. At the top of the blade, click the \+ Container button

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666573.jpg





### In the New container blade that displays:
In the New container blade that displays, perform the following steps:  
a. In the Name box, type example.  
b. In the Access Type list, select Container.  
c. Click the Create button to create your container.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666574.jpg





### Verify the new container
Verify the new container and close the Blob blade.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666576.jpg





### Select the Access keys option
In the Storage account blade, select the Access keys option.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666575.jpg





### Select the View connection string option
In the Access keys blade, locate a key that you wish to use. For the access key you selected, click the three ellipsis \)...) button to the right of the key. Once clicked, select the View connection string option.

#### :bulb: KNOWLEDGE
Note: you can use any of the keys listed for this lab.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666577.jpg





### Copy your connection string
In the View connection string dialog, copy your connection string for the access key you selected

#### :bulb: KNOWLEDGE
Note: This connection string will be used in various parts of this lab.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666578.jpg





### Paste to Notepad
Click the Start button and type Notepad then click to open Notepad. Choose Edit/Paste to paste the access key to Notepad. You will use this to copy the key several times. Select the Format/Word Wrap option to see the whole key.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/672217.jpg





### Start Visual Studio 2015
On the Start screen, locate and click the Visual Studio 2015 tile.

#### :bulb: KNOWLEDGE
Note: You might have to use the down arrow to locate the Visual Studio 2015 tile on your Start screen. Also, it may take a while to load initially.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666579.jpg





### On the View menu, click Cloud Explorer:
On the View menu, click Cloud Explorer.

#### :bulb: KNOWLEDGE
Note: If you have not previously indicated that you want Visual Studio to remember your credentials, you will be prompted to enter your Microsoft account username and password to continue.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666580.jpg





### View the container just created
Expand the Storage Accounts node under your Azure account \)not Local). Expand the stor20532\[Your Name\] account node under the Storage node. Expand the Blob Containers node under your storage account’s node. Double-click example.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666581.jpg





### Click the Upload Blob button
In the example \[Container\] tab, click the Upload Blob button.  
           

#### :bulb: KNOWLEDGE
Note: The icon on the upload button includes an arrow that is pointing upward to a horizontal line.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666582.jpg





### In the Upload New File dialog box:
In the Upload New File dialog box, perform the following steps:  
a. Click the Browse button.  
b. Go to the \)F):\\Mod07\\LabFiles\\Starter\\ directory.  
c. Click the samplefile text document.  
d. Click Open.  
e. Leave the folder option set to it's default \)blank) value.  
e. Click the OK button to complete the dialog.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666583.jpg





### Verify upload successful
Verify upload successful. Close Visual Studio.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666584.jpg





### Access file via Internet Explorer
Switch to the Internet Explorer window. In a new tab, type the following URL by replacing \[storage account\] with the name of your storage account:  
https://\[\*storage account\*\].blob.core.windows.net/example/samplefile.txt  
Verify that the text This is your sample file! displays in the browser.

#### :bulb: KNOWLEDGE
Note: In Visual Studio, you can also right click the samplefile.txt file and select Copy URL and paste it in your new tab.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666585.jpg



#### :calling: COMMAND
```TypeText
https://[*storage account*].blob.core.windows.net/example/samplefile.txt
```



# Exercise 2: Populating the Container with Files and Media
## INTRODUCTION MESSAGE
In this exercise, you will:  
  
Use the Azure Storage SDK to access blobs in your storage account.  
Use the Azure Storage SDK to create blobs in your storage account.  
  
The main tasks for this exercise are as follows:  
Open the blob helper in the Web App worker project.  
Add Word documents to the container after they are created.
## COMPLETION MESSAGE
Results: After completing this exercise, you will have used the Azure Storage SDK to manage blobs and containers in your storage account.
### Open solution Contoso.Events
On the taskbar, click File Explorer. In the Libraries window, go to Allfiles \)F):\\Mod07\\Labfiles\\Starter\\Contoso.Events, and then double-click Contoso.Events.sln.

#### :bulb: KNOWLEDGE
Note that Known file extensions \)such as .sln) may be hidden. See screenshot.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666586.jpg
>* ShowAutomatically = No





### Open the BlobStorageHelper.cs file
In the Solution Explorer pane, expand the Roles solution folder. In the Solution Explorer pane, expand the Contoso.Events.Worker project. Double-click the BlobStorageHelper.cs file.

#### :bulb: KNOWLEDGE
You can Auto Hide any windows not needed by clicking the push-pull pin on the window.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666587.jpg





### In the BlobStorageHelper class, find the method:
In the BlobStorageHelper class, find the method with the following signature:  
public Uri CreateBlob\)MemoryStream stream, string eventKey)

#### :bulb: KNOWLEDGE
Ignore Intellisense errors

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666588.jpg





### Remove the following single line of code:
Remove the following single line of code in the class:  
return null;

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666589.jpg





### Create a new CloudBlobContainer
At the end of the CreateBlob method and before the closing brace, create a new CloudBlobContainer for the signin container.  
CloudBlobContainer container = \_blobClient.GetContainerReference\)"signin");

#### :bulb: KNOWLEDGE
Ignore Intellisense errors

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666590.jpg



#### :calling: COMMAND
```TypeText
CloudBlobContainer container = _blobClient.GetContainerReference("signin");
```


### Call the CreateIfNotExists method:
Call the CreateIfNotExists method of the CloudBlobContainer variable to ensure that the container exists:  
container.CreateIfNotExists\));

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666591.jpg



#### :calling: COMMAND
```TypeText
container.CreateIfNotExists();
```


### Create a new variable named blobName:
At the end of the CreateBlob method and before the closing brace, create a new variable named blobName:  
string blobName;

#### :bulb: KNOWLEDGE
Ignore Intellisense errors

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666592.jpg



#### :calling: COMMAND
```TypeText
string blobName;
```


### Use the String.Format static method:
Use the String.Format static method to create a string, and then assign the string to the blobName variable:  
blobName = String.Format\)"\{0\}\_SignIn\_\{1:ddmmyyyss\}.docx", eventKey, DateTime.UtcNow);

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666593.jpg



#### :calling: COMMAND
```TypeText
blobName = String.Format("{0}_SignIn_{1:ddmmyyyss}.docx", eventKey, DateTime.UtcNow);
```


### Create a block blob reference:
At the end of the CreateBlob method and before the closing brace, create a block blob reference by using the GetBlockBlobReference method and the blobName variable as the parameter:  
ICloudBlob blob = container.GetBlockBlobReference\)blobName);

#### :bulb: KNOWLEDGE
Ignore Intellisense errors

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666594.jpg



#### :calling: COMMAND
```TypeText
ICloudBlob blob = container.GetBlockBlobReference(blobName);
```


### Use the Seek method:
Use the Seek method of the MemoryStream variable to set the position of the stream to the beginning and offset the position by the value of 0:  
stream.Seek\)0, SeekOrigin.Begin);

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666595.jpg



#### :calling: COMMAND
```TypeText
stream.Seek(0, SeekOrigin.Begin);
```


### Use the UploadFromStream method:
Use the UploadFromStream method of the ICloudBlob interface to upload the stream to the referenced blob:  
blob.UploadFromStream\)stream);

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666596.jpg



#### :calling: COMMAND
```TypeText
blob.UploadFromStream(stream);
```


### At the end of the CreateBlob method:
At the end of the CreateBlob method and before the closing brace, add the following statement:  
return blob.Uri;

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666597.jpg



#### :calling: COMMAND
```TypeText
return blob.Uri;
```



# Exercise 3: Retrieving Files and Media from the Container
## INTRODUCTION MESSAGE
In this exercise, you will:  
  
Retrieve blobs from your storage account by using the Azure Storage SDK.  
The main tasks for this exercise are as follows:  
  
Download documents from blob storage and stream to the client.  
Generate the Test Data.  
Download generated sign-in sheets from the blob storage.
## COMPLETION MESSAGE
Results: After completing this exercise, you will have downloaded blobs from your storage account by using the Azure Storage SDK.
### Open the DownloadViewModel.cs file
In the Solution Explorer pane, expand the Shared solution folder. Expand the Contoso.Events.ViewModels project. Double-click the DownloadViewModel.cs file.

#### :bulb: KNOWLEDGE
Ignore Intellisense errors

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666633.jpg
>* ShowAutomatically = No





### Find the method with the following signature:
In the DownloadViewModel class, find the method with the following signature:  
public async Task<DownloadPayload> GetStream\))

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666634.jpg





### Remove the following single line of code:
Remove the following single line of code in the class:  
return await Task.FromResult<DownloadPayload>\)null);

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666635.jpg





### Create a new CloudBlobClient variable:
At the end of the GetStream method and before the closing brace, create a new CloudBlobClient variable for the \_storageAccount variable:  
CloudBlobClient blobClient = \_storageAccount.CreateCloudBlobClient\));

#### :bulb: KNOWLEDGE
Ignore Intellisense errors

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666636.jpg



#### :calling: COMMAND
```TypeText
CloudBlobClient blobClient = _storageAccount.CreateCloudBlobClient();
```


### Create a new CloudBlobContainer instance:
Create a new CloudBlobContainer instance for the signin container by using the CloudBlobClient variable:  
CloudBlobContainer container = blobClient.GetContainerReference\)"signin");

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666637.jpg



#### :calling: COMMAND
```TypeText
CloudBlobContainer container = blobClient.GetContainerReference("signin");
```


### Call the CreateIfNotExists method:
Call the CreateIfNotExists method of the CloudBlobContainer variable to ensure that the container exists:  
container.CreateIfNotExists\));

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666638.jpg



#### :calling: COMMAND
```TypeText
container.CreateIfNotExists();
```


### Create a block blob reference:
At the end of the GetStream method and before the closing brace, create a block blob reference by using the GetBlockBlobReference method and the \_blobId variable as the parameter:  
ICloudBlob blob = container.GetBlockBlobReference\)\_blobId);

#### :bulb: KNOWLEDGE
Ignore Intellisense errors

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666639.jpg



#### :calling: COMMAND
```TypeText
ICloudBlob blob = container.GetBlockBlobReference(_blobId);
```


### Use the OpenReadAsync method:
Use the OpenReadAsync method of the ICloudBlob variable to create a Stream and store it in a variable:  
Stream blobStream = await blob.OpenReadAsync\));

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666640.jpg



#### :calling: COMMAND
```TypeText
Stream blobStream = await blob.OpenReadAsync();
```


### reate a new instance of the DownloadPayload class:
At the end of the GetStream method and before the closing brace, create a new instance of the DownloadPayload class:  
DownloadPayload payload = new DownloadPayload\));

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666641.jpg



#### :calling: COMMAND
```TypeText
DownloadPayload payload = new DownloadPayload();
```


### Assign the Stream variable:
Assign the Stream variable to the DownloadPayload variable’s Stream property:  
payload.Stream = blobStream;

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666642.jpg



#### :calling: COMMAND
```TypeText
payload.Stream = blobStream;
```


### Assign the ICloudBlob variable’s ContentType:
Assign the ICloudBlob variable’s Properties.ContentType value to the DownloadPayload variable’s ContentType property:  
payload.ContentType = blob.Properties.ContentType;

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666643.jpg



#### :calling: COMMAND
```TypeText
payload.ContentType = blob.Properties.ContentType;
```


### Return the DownloadPayload variable:
Return the DownloadPayload variable:  
return payload;

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666644.jpg



#### :calling: COMMAND
```TypeText
return payload;
```


### Open the app.config file in the project:
In the Solution Explorer pane, expand the Shared solution folder. Expand the Contoso.Events.Data.Generation project.  
Locate and open the app.config file in the project.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666645.jpg





### Locate the following configuration setting:
Within the app.config file, locate the following configuration setting:  
 <add key="StorageConnectionString" value="UseDevelopmentStorage=true" />

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666646.jpg





### Update connection string setting
Update the setting by replacing the value of the value attribute \)currently UseDevelopmentStorage=true) with your Storage Account's connection string. If necessary, you can switch back to Notepad and copy the connection string to the clipboard first.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666647.jpg





### Verify new connection string
Verify new connection string

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666648.jpg





### Debug Data.Generation project
In the Solution Explorer pane, right-click the Contoso.Events.Data.Generation project, point to Debug, and then click Start New Instance. Wait for debugging to complete \)when the console window closes).

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666649.jpg





### Verify Output
Verify that the debug session returned success with code 0 in the Output tab

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666650.jpg





### Open Contoso.Events solution Properties:
In the Solution Explorer pane, right-click the Contoso.Events solution, and then click Properties.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666651.jpg





### Select the Multiple startup projects option
Navigate to the Startup Project section located under the Common Properties header. In the Startup Project section, locate and select the Multiple startup projects option.   
Within the Multiple startup projects table, perform the following actions:  
a. Locate the Contoso.Events.Web entry and change it's Action from None to Start.  
b. Locate the Contoso.Events.Management entry and change it's Action from None to Start.  
c. Locate the Contoso.Events.Worker entry and change it's Action from None to Start.  
Click the OK button to close the Property dialog.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666652.jpg





### Open the web.config file
In the Solution Explorer pane, expand the Administration solution folder. Expand the Contoso.Events.Management project.  
Locate and open the web.config file in the project.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666653.jpg





### Locate the following configuration setting:
Within the web.config file, locate the following configuration setting:  
 <add key="Microsoft.WindowsAzure.Storage.ConnectionString" value="UseDevelopmentStorage=true" />

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666654.jpg





### Update the connection string setting:
Update the setting by replacing the value of the value attribute \)currently UseDevelopmentStorage=true) with your Storage Account's connection string.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666655.jpg





### Open the web.config file:
In the Solution Explorer pane, expand the Roles solution folder. Expand the Contoso.Events.Web project. Locate and open the web.config file in the project.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666656.jpg





### Locate the following configuration setting:
Within the web.config file, locate the following configuration setting:  
 <add key="Microsoft.WindowsAzure.Storage.ConnectionString" value="UseDevelopmentStorage=true" />

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666657.jpg





### Update the connection string setting:
Update the setting by replacing the value of the value attribute \)currently UseDevelopmentStorage=true) with your Storage Account's connection string.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666658.jpg





### Locate and open the app.config file in the project
In the Solution Explorer pane, expand the Contoso.Events.Worker project. Locate and open the app.config file in the project.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666659.jpg





### Within the app.config file, locate the following:
Within the app.config file, locate the following configuration setting:  
 <add name="AzureWebJobsStorage" connectionString="UseDevelopmentStorage=true" />

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666660.jpg





### Update the connection string setting
Update the setting by replacing the value of the connectionString attribute \)currently UseDevelopmentStorage=true) with your Storage Account's connection string.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666661.jpg





### Within the app.config file, locate the following:
Within the app.config file, locate the following configuration setting:  
 <add name="AzureWebJobsDashboard" connectionString="UseDevelopmentStorage=true" />

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666662.jpg





### Update the connection string setting
Update the setting by replacing the value of the connectionString attribute \)currently UseDevelopmentStorage=true) with your Storage Account's connection string.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666663.jpg





### Within the app.config file, locate the following:
Within the app.config file, locate the following configuration setting:  
 <add key="StorageConnectionString" value="UseDevelopmentStorage=true" />

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666664.jpg





### Update the connection string setting
Update the setting by replacing the value of the value attribute \)currently UseDevelopmentStorage=true) with your Storage Account's connection string.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666665.jpg





### On the Debug menu, click Start Debugging.
On the Debug menu, click Start Debugging. Note that two web sites will launch in Internet Explorer in different tabs: Web\)Upcoming Events) and Management \)Administration).

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666666.jpg





### Switch to Contoso Events Administration web app:
On the home page for the Contoso Events Administration web application, click the Go to Events List button to view the list of events. You may have to switch tabs in Internet Explorer from the Web\)Upcoming Events) app to the Management\)Administration) app.

#### :bulb: KNOWLEDGE
Note that two web sites will launch in different tabs: Web\)Upcoming Events) and Management \)Administration).

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666667.jpg





### Click the Sign-In Sheet button for any event:
Click the Sign-In Sheet button for any event in the list.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666668.jpg





### Sign-in sheet is being generated message:
View the sign-in page that notifies you that a sign-in sheet is being generated.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666669.jpg





### Wait for one to two minutes, and then refresh:
Wait for one to two minutes, and then refresh the sign-in sheet page.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666670.jpg





### Click Sign-In Sheet to download the sign-in sheet:
Click Sign-In Sheet to download the sign-in sheet from the server. Click Open at the download dialog to open the sign-in sheet in WordPad.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666671.jpg





### View the Sign-in sheet in WordPad
 View the Sign-in sheet in WordPad. Close WordPad.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666672.jpg






# Exercise 4: Specifying Permissions for the Container
## INTRODUCTION MESSAGE
In this exercise, you will:  
  
Use the Visual Studio 2015 Cloud Explorer to modify a container.  
Generate a SAS token by using the Azure Storage SDK.  
  
The main tasks for this exercise are as follows:  
Modify Container Access using Cloud Explorer.  
Generate temporary SAS tokens by using the SDK.  
Download documents from a protected container by using the SAS token.
## COMPLETION MESSAGE
Results: After completing this exercise, you will have modified the permissions of the containers and generated SAS tokens for the containers.
### In Visual Studio,  choose Stop Debugging:
On the desktop, click the Contoso.Events - Visual Studio 2015 window. On the Debug menu, click Stop Debugging

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666605.jpg





### Open Cloud Explorer, view container
On the View menu, click Cloud Explorer. Expand the Storage Accounts node. Expand the node for the storage account used in this lab under the Storage Accounts node. Expand the Blob Containers node. Select the signin container, and then click Properties Tab below.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666606.jpg





### Verify Public Read Access property is set to Off:
In the Properties pane, locate Public Read Access. Ensure that the value of the Public Read Access property is set to Off.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666607.jpg





### Open the DownloadViewModel.cs file.
In the Solution Explorer pane, expand the Shared solution folder. Expand the Contoso.Events.ViewModels project. Double-click the DownloadViewModel.cs file.

#### :bulb: KNOWLEDGE
You can Auto Hide the Cloud Explorer by pushing the push-pull pin in the window to make more room for the text editor.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666608.jpg





### Find the method with the following signature:
In the DownloadViewModel class, find the method with the following signature:  
public async Task<string> GetSecureUrl\))

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666609.jpg





### Remove the single line of code in the class:
Remove the single line of code in the class:  
return await Task.FromResult<string>\)String.Empty);

#### :bulb: KNOWLEDGE
Ignore Intellisense errors

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666610.jpg





### Create a new CloudBlobClient:
At the end of the GetSecureUrl method and before the closing brace, create a new CloudBlobClient for the \_storageAccount variable.  
CloudBlobClient blobClient = \_storageAccount.CreateCloudBlobClient\));

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666611.jpg



#### :calling: COMMAND
```TypeText
CloudBlobClient blobClient = _storageAccount.CreateCloudBlobClient();
```


### Create a new CloudBlobContainer:
Create a new CloudBlobContainer for the signin container by using the CloudBlobClient variable.  
CloudBlobContainer container = blobClient.GetContainerReference\)"signin");

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666612.jpg



#### :calling: COMMAND
```TypeText
CloudBlobContainer container = blobClient.GetContainerReference("signin");
```


### Call the CreateIfNotExists method:
Call the CreateIfNotExists method of the CloudBlobContainer variable to ensure that the container exists:  
container.CreateIfNotExists\));

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666613.jpg



#### :calling: COMMAND
```TypeText
container.CreateIfNotExists();
```


### Create new instance of the SharedAccessBlobPolicy:
At the end of the GetSecureUrl method and before the closing brace, create a new instance of the SharedAccessBlobPolicy class:  
SharedAccessBlobPolicy blobPolicy = new SharedAccessBlobPolicy\));

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666614.jpg



#### :calling: COMMAND
```TypeText
SharedAccessBlobPolicy blobPolicy = new SharedAccessBlobPolicy();
```


### Set SharedAccessExpiryTime property:
Set the SharedAccessBlobPolicy variable’s SharedAccessExpiryTime property to 15 minutes from the current time:  
blobPolicy.SharedAccessExpiryTime = DateTime.Now.AddHours\)0.25d);

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666615.jpg



#### :calling: COMMAND
```TypeText
blobPolicy.SharedAccessExpiryTime = DateTime.Now.AddHours(0.25d);
```


### Set Permissions property to Read:
Set the SharedAccessBlobPolicy variable’s Permissions property to SharedAccessBlobPermissions.Read:  
blobPolicy.Permissions = SharedAccessBlobPermissions.Read;

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666616.jpg



#### :calling: COMMAND
```TypeText
blobPolicy.Permissions = SharedAccessBlobPermissions.Read;
```


### Create new instance of BlobContainerPermissions:
At the end of the GetSecureUrl method and before the closing brace, create a new instance of the BlobContainerPermissions class:  
BlobContainerPermissions blobPermissions = new BlobContainerPermissions\));

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666617.jpg



#### :calling: COMMAND
```TypeText
BlobContainerPermissions blobPermissions = new BlobContainerPermissions();
```


### Add the newly created SharedAccessBlobPolicy:
Add the newly created SharedAccessBlobPolicy to the BlobContainerPermissions variable’s SharedAccessPolicy with the key “ReadBlobPolicy”:  
blobPermissions.SharedAccessPolicies.Add\)"ReadBlobPolicy", blobPolicy);

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666618.jpg



#### :calling: COMMAND
```TypeText
blobPermissions.SharedAccessPolicies.Add("ReadBlobPolicy", blobPolicy);
```


### Set the BlobContainerPermissions:
Set the BlobContainerPermissions variable’s PublicAccess property to BlobContainerPublicAccessType.Off:  
blobPermissions.PublicAccess = BlobContainerPublicAccessType.Off;

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666619.jpg



#### :calling: COMMAND
```TypeText
blobPermissions.PublicAccess = BlobContainerPublicAccessType.Off;
```


### Call asynchronous SetPermissionsAsync method:
At the end of the GetSecureUrl method and before the closing brace, call the asynchronous SetPermissionsAsync method of the CloudBlobContainer variable by using the BlobContainerPermissions variable as the parameter:  
await container.SetPermissionsAsync\)blobPermissions);

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666620.jpg



#### :calling: COMMAND
```TypeText
await container.SetPermissionsAsync(blobPermissions);
```


### Invoke the GetSharedAccessSignature method:
Invoke the GetSharedAccessSignature method of the CloudBlobContainer variable by using a new instance of the SharedAccessBlobPolicy class as the first parameter and the “ReadBlobPolicy” key as the second parameter:  
string sasToken = container.GetSharedAccessSignature\)new SharedAccessBlobPolicy\)), "ReadBlobPolicy");

#### :bulb: KNOWLEDGE
If you get an Intellisense error on this line of code, make sure the text has been entered correctly.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666621.jpg



#### :calling: COMMAND
```TypeText
string sasToken = container.GetSharedAccessSignature(new SharedAccessBlobPolicy(), "ReadBlobPolicy");
```


### Create a block blob reference:
At the end of the GetSecureUrl method and before the closing brace, create a block blob reference by using the GetBlockBlobReference method and the \_blobId variable as the parameter:  
ICloudBlob blob = container.GetBlockBlobReference\)\_blobId);

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666622.jpg



#### :calling: COMMAND
```TypeText
ICloudBlob blob = container.GetBlockBlobReference(_blobId);
```


### Store the Uri property in a variable:
Take the Uri property of the ICloudBlob variable and store it in a new Uri variable.  
Uri blobUrl = blob.Uri;

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666623.jpg



#### :calling: COMMAND
```TypeText
Uri blobUrl = blob.Uri;
```


### Concatenate the variables:
At the end of the GetSecureUrl method and before the closing brace, concatenate the AbsoluteUri of the Uri variable and the sasToken variable:  
string secureUrl = blobUrl.AbsoluteUri \+ sasToken;

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666624.jpg



#### :calling: COMMAND
```TypeText
string secureUrl = blobUrl.AbsoluteUri + sasToken;
```


### Return the string variable:
Return the string variable as the result of the method:  
return secureUrl;

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666625.jpg



#### :calling: COMMAND
```TypeText
return secureUrl;
```


### On the Debug menu, click Start Debugging
On the Debug menu, click Start Debugging. Note that two web sites will launch in Internet Explorer in different tabs: Web\)Upcoming Events) and Management \)Administration).

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666626.jpg





### Switch to Contoso Events Administration web app
On the home page for the Contoso Events Administration web application, click the Go to Events List button to view the list of events. You may have to switch tabs in Internet Explorer from the Web\)Upcoming Events) app to the Management\)Administration) app.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666627.jpg





### Click the Sign-In Sheet button for another event:
Click the Sign-In Sheet button for any event in the list. \)Choose a different event from before)

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666628.jpg





### Sign-in sheet is being generated message:
View the sign-in page that notifies you that a sign-in sheet is being generated.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666629.jpg





### Wait for one to two minutes, and then refresh:
Wait for one to two minutes, and then refresh the sign-in sheet page.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666630.jpg





### Click Sign-In Sheet to download the sign-in sheet:
Click Sign-In Sheet to download the sign-in sheet from the server. Click Open at the download dialog to open the sign-in sheet in WordPad.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666631.jpg





### View the Sign-in sheet in WordPad:
View the Sign-in sheet in WordPad. Close WordPad.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666632.jpg





### Close Internet Explorer
Close Internet Explorer





### Close Visual Studio 2015
Close Visual Studio 2015





### Close File Explorer
Close File Explorer





### Close Notepad without saving
Close Notepad without saving





### Close RDP session
Close RDP session and click OK to disconnect

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666601.jpg
>* ShowAutomatically = No





### Stop VM to save billing charges
If you are stopping labs for the day, on the vm2032 Overview page in the Azure Portal, click Stop to stop billing charges until you start labs again. When prompted, click Yes to stop the VM.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666602.jpg
>* ShowAutomatically = No





### Close Internet Explorer
Close Internet Explorer to end the lab

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666603.jpg
>* ShowAutomatically = No






