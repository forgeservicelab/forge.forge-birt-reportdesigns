
## BI reports for FORGE 

Copyright (C) DIGILE Ltd 2015

Author Pasi Kivikangas

In order to use the report generation templates you need:

- Eclipse (Kepler) with Report Designer module and mysql and postgresql plugins
- Have access to the datasource at jdbc:postgresql://analytics.forgeservicelab.fi:5432/iaas
- Optionally you can use Tomcat with BIRT runtime to create reports and then Tomcat needs also to have access to the datasource

Assuming the previous requirements are satisfied then you should be able to
create a report straight from the Eclipse.

If you want to use Tomcat to create a report, you have to install BIRT
runtimes on Tomcat and copy report template into Tomcat as well. 
Note! Tomcat machine should also have access to the datasources.

Copy BIRT runtime to <TOMCATROOT>/webapps/birt-viewer
Copy report template to <TOMCATROOT>/webapps/birt-viewer/forge_stories_status.rptdesign

Following project names are excluded from the iaas reports

digile*
Digile*
forge*
Forge*
*test
test*
demo*
