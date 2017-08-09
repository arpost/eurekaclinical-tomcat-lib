${project.name} ${project.version} -- An ETL Tool for Loading Data into
i2b2.  Department of Biomedical Informatics, ${project.organization.name}

OVERVIEW

${project.description}

WHAT'S NEW

Version 2.0 <need to fill in>

Version 1.9 includes an update to the UI, now using Bootstrap 3, 
to make the application more usable on mobile devices.  It also 
includes support for i2b2 1.7.  A new feature to allow usage of 
BioPortal for ontologies was added.  The codebase was also updated 
to utilize Java 7.  A data element search functionality was 
added to the phenotype editor and job submission screens.  Eureka! 
can now utilize OAuth as an authentication mechanism, allowing 
the use of services like Facebook, Twitter, Google Plus, and other 
to log into the system.  Finally, many improvements were made 
to ease the process of installing and configuring the software.

Version 1.8.2 includes minor bug-fixes. 

Version 1.8.1 includes minor bug-fixes.

Version 1.8 provides the following changes:

- Ability to directly connect to databases and data warehouses as sources of
patient data
- Improvements to the phenotype editor

Version 1.7 added Liquibase support for database migrations and additional data
element editor features. You can specify frequencies of consecutive data elements
 for any data element now. You also can specify value thresholds that are 
specific to a disease or condition.

Version 1.6 extended the rudimentary data element editing support
provided in version 1.5 to provide a complete data element editor. You
can specify a relatively complete set of the temporal patterns that
can be specified in the underlying Protempa software.

REQUIREMENTS

The current version is known to work with Oracle Java 8. It is
expected to work with OpenJDK 8 as well. 

INSTALLATION

Once downloaded and unpacked, please see http://eurekaclinical.org/ for 
documentation on installation and usage.

To compile from source, make sure JDK 8 and Maven >= 3.2.5 are installed.
You also need an Oracle Technology Network account because the build 
process pulls a copy of the Oracle JDBC driver from Oracle's servers. 
Once you have an account, add the following to your ~/.m2/settings.xml file:

<settings>
...
  <servers>
    ...
    <server>
      <id>maven.oracle.com</id>
      <username>your_username</username>
      <password>your_password</password>
      <configuration>
        <basicAuthScope>
         <host>ANY</host>
         <port>ANY</port>
         <realm>OAM 11g</realm>
        </basicAuthScope>
        <httpConfiguration>
          <all>
            <params>
              <property>
                <name>http.protocol.allow-circular-redirects</name>
                <value>%b,true</value>
              </property>
            </params>
          </all>
        </httpConfiguration>
      </configuration>
    </server>
    ...
  </servers>
  ...
</settings>

See http://docs.oracle.com/middleware/1213/core/MAVEN/config_maven_repo.htm#MAVEN9010
for more information.

CONTACTING US

Please send an email to help@eurekaclinical.org for support or questions.

LICENSING

${project.name} is freely available as open source under
the Apache License, Version 2.0. A copy of the license is in the
LICENSE file provided in this distribution.

${project.name} is Copyright (C) ${project.inceptionYear}-2015 ${project.organization.name}.

MORE INFORMATION

Please see ${aiw.site.url} for more information and
${project.url} for technical
documentation.
