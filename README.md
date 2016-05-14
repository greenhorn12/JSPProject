# JSPProject

1. One way of executing this is by using the Eclipse IDE. If you don't have Eclipse, please download it from https://www.eclipse.org/downloads/packages/eclipse-ide-java-ee-developers/keplersr2.
2. Please download Apache Tomcat 7.0.69 from https://tomcat.apache.org/download-70.cgi.
3. Now, import the WAR file from to Eclipse using the instructions stated at http://help.eclipse.org/juno/index.jsp?topic=%2Forg.eclipse.wst.webtools.doc.user%2Ftopics%2Ftwimpwar.html
To quote the instructions,
 "   A Web Archive (WAR) file is a portable, packaged Web application that you can import into your workspace.
    
    Before importing a WAR file, you should first determine if the WAR file contains needed Java™ source files. When importing a WAR file into an existing Web project, the imported Web deployment descriptor files are either not changed or overwritten by the ones included in the imported WAR file, based on your response to the prompt that is provided. In either case, this action does not represent a merging of the two sets of deployment descriptors.
    
    To import the Web project resources in a WAR file into your workspace, complete the following steps:
    
    Select File > Import .
    In the Import dialog, select WAR file and then click Next.
    Locate the WAR file that you want to import using the Browse button.
    The wizard assumes you want to create a new Web project with the same name as the WAR file. If you accept this choice, the project will be created with the same servlet version as specified by the WAR file and in the same location. If you want to override these settings, you can click New and specify your new settings in the Dynamic Web Project wizard.
    Click Finish to populate the Web project."

4. Now, under JSPProject/WebContent/WEB-INF/ we have web.xml. Please open that file. Under the tag "<context-param>", you have "<param-value>". Please change the path under "<param-value>" to your desired location to store the uploaded file.
5. Now, you are set. In Project Explorer in Eclipse, right-click on JSPProject -> Run As -> Run on Server.
