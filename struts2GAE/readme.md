Para crear este proyecto, se debe utilizar maven (ver el log de mi consola al final del documento).

Una vez que fué creado el proyecto eclipse, se debe abrir eclipse e importar el proyecto.

En caso de obtener un error al correrlo, consultar este post http://www.mkyong.com/struts2/struts-2-hello-world-example/



sergio@ubuntu:~/workspace/struts2GAE$ mvn archetype:generate -DarchetypeCatalog=http://struts.apache.org/
[INFO] Scanning for projects...
[INFO]                                                                         
[INFO] ------------------------------------------------------------------------
[INFO] Building Maven Stub Project (No POM) 1
[INFO] ------------------------------------------------------------------------
[INFO] 
[INFO] >>> maven-archetype-plugin:2.2:generate (default-cli) @ standalone-pom >>>
[INFO] 
[INFO] <<< maven-archetype-plugin:2.2:generate (default-cli) @ standalone-pom <<<
[INFO] 
[INFO] --- maven-archetype-plugin:2.2:generate (default-cli) @ standalone-pom ---
[INFO] Generating project in Interactive mode
[INFO] No archetype defined. Using maven-archetype-quickstart (org.apache.maven.archetypes:maven-archetype-quickstart:1.0)
Choose archetype:
1: http://struts.apache.org/ -> org.apache.struts:struts2-archetype-blank (Struts 2 Archetypes - Blank)
2: http://struts.apache.org/ -> org.apache.struts:struts2-archetype-convention (Struts 2 Archetypes - Blank Convention)
3: http://struts.apache.org/ -> org.apache.struts:struts2-archetype-dbportlet (Struts 2 Archetypes - Database Portlet)
4: http://struts.apache.org/ -> org.apache.struts:struts2-archetype-plugin (Struts 2 Archetypes - Plugin)
5: http://struts.apache.org/ -> org.apache.struts:struts2-archetype-portlet (Struts 2 Archetypes - Portlet)
6: http://struts.apache.org/ -> org.apache.struts:struts2-archetype-starter (Struts 2 Archetypes - Starter)
Choose a number or apply filter (format: [groupId:]artifactId, case sensitive contains): : 2
Define value for property 'groupId': : com.frditlabs
Define value for property 'artifactId': : struts2GAE
Define value for property 'version':  1.0-SNAPSHOT: : 
Define value for property 'package':  com.frditlabs: : 
Confirm properties configuration:
groupId: com.frditlabs
artifactId: struts2GAE
version: 1.0-SNAPSHOT
package: com.frditlabs
 Y: : Y
[INFO] ----------------------------------------------------------------------------
[INFO] Using following parameters for creating project from Archetype: struts2-archetype-convention:2.3.16.3
[INFO] ----------------------------------------------------------------------------
[INFO] Parameter: groupId, Value: com.frditlabs
[INFO] Parameter: artifactId, Value: struts2GAE
[INFO] Parameter: version, Value: 1.0-SNAPSHOT
[INFO] Parameter: package, Value: com.frditlabs
[INFO] Parameter: packageInPathFormat, Value: com/frditlabs
[INFO] Parameter: package, Value: com.frditlabs
[INFO] Parameter: version, Value: 1.0-SNAPSHOT
[INFO] Parameter: groupId, Value: com.frditlabs
[INFO] Parameter: artifactId, Value: struts2GAE
[INFO] project created from Archetype in dir: /home/sergio/workspace/struts2GAE/struts2GAE
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time: 1:04.434s
[INFO] Finished at: Sat May 10 22:28:03 ART 2014
[INFO] Final Memory: 13M/109M
[INFO] ------------------------------------------------------------------------
sergio@ubuntu:~/workspace/struts2GAE$ cd struts2GAE/
sergio@ubuntu:~/workspace/struts2GAE/struts2GAE$ mvn eclipse:eclipse -Dwtpversion=2.0
[INFO] Scanning for projects...
[WARNING] 
[WARNING] Some problems were encountered while building the effective model for com.frditlabs:struts2GAE:war:1.0-SNAPSHOT
[WARNING] 'build.plugins.plugin.version' for org.apache.maven.plugins:maven-compiler-plugin is missing. @ line 80, column 21
[WARNING] 
[WARNING] It is highly recommended to fix these problems because they threaten the stability of your build.
[WARNING] 
[WARNING] For this reason, future Maven versions might no longer support building such malformed projects.
[WARNING] 
[INFO]                                                                         
[INFO] ------------------------------------------------------------------------
[INFO] Building struts2GAE 1.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO] 
[INFO] >>> maven-eclipse-plugin:2.9:eclipse (default-cli) @ struts2GAE >>>
[INFO] 
[INFO] <<< maven-eclipse-plugin:2.9:eclipse (default-cli) @ struts2GAE <<<
[INFO] 
[INFO] --- maven-eclipse-plugin:2.9:eclipse (default-cli) @ struts2GAE ---
[INFO] Adding support for WTP version 2.0.
[INFO] Using Eclipse Workspace: /home/sergio/workspace
[INFO] no substring wtp server match.
[INFO] Using as WTP server : Google App Engine
[INFO] Adding default classpath container: org.eclipse.jdt.launching.JRE_CONTAINER/org.eclipse.jdt.internal.debug.ui.launcher.StandardVMType/J2SE-1.5
[INFO] Wrote settings to /home/sergio/workspace/struts2GAE/struts2GAE/.settings/org.eclipse.jdt.core.prefs
[INFO] Wrote Eclipse project for "struts2GAE" to /home/sergio/workspace/struts2GAE/struts2GAE.
[INFO] 
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time: 5.588s
[INFO] Finished at: Sat May 10 22:29:09 ART 2014
[INFO] Final Memory: 11M/109M
[INFO] ------------------------------------------------------------------------
sergio@ubuntu:~/workspace/struts2GAE/struts2GAE$ 

