
## BIRT reports for FORGE Redmine

Copyright (C) DIGILE Ltd 2013
Author Pasi Kivikangas

In order to use the report generation templates you need:

- Eclipse with Report Designer module and mysql plugin
- SSH tunnel from your local machine (port 8888) to support.forgeservicelab.fi (port 3306)
- Optionally you can use Tomcat with BIRT runtime to create reports

$ ssh -L 8888:localhost:3306 pkivikan@support.forgeservicelab.fi

Then you should be able to create a report straight from the Eclipse.
If you want to use Tomcat to create a report, you have to install BIRT
runtimes on Tomcat and copy report template into Tomcat as well. 
Note! Tomcat machine should also have a ssh tunnel to support machine.

Copy BIRT runtime to <TOMCATROOT>/webapps/birt-viewer
Copy report template to <TOMCATROOT>/webapps/birt-viewer/forge_stories_status.rptdesign

