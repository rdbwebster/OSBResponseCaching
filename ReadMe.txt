To deploy this example



Deploy the DepartmentDetails web service (dependency)
-----------------------------------------------------
The DepartmentDetails Service is available in a blog posting here -
https://blogs.oracle.com/bwb/resource/webservices/Create_a_simple_Web_Service_from_Java_Code_using_JDeveloper.html

The service can be developed by following the instructions or download the completed example from git hub.
See the link at the end of the article.


Load the OSB configuration
--------------------------
Zip the sbconfig folder into a archive named sbconfig.jar

Login the OSB console http://localhost:7001/sbconsole  (your server and port may vary)
-Click Create to create a new session or click Edit to enter an existing session.
-Select System Administration > Import Resources.
-Browse and select the sbconfig.jar file
-Check the include dependencies checkbox
-import the project.

After the import, activte the changes.

Then using a text editor, modify the endpoint uri for the deparmentdetails service using the
ALSBCustomization.xml file.
Edit the file and change the business service uri to match the url of the
DepartmentDetails service deployed on your server.

Then in the OSB console start a new session and select System
Administration > Customization > Execute Customization File
Browse to the ALSBCustomization.xml file and choose Next and Execute.
Then activate the session.


