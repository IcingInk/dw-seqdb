# dw-seqdb
the vagrant-project is located here : https://bitbucket.org/aafc-mbb/seqdb-vagrant <br>
this is a docker-project, transforming the above vagrant-project (dev) to a docker-project. <br>

## tomcat, java and mysql
1. Tomcat version : 7.0.69
2. Java version, Oracle : 1.8.0_77
3. MySQL version : 5.6

##  2 files are missing ...
1. the sql-file
2. the seqdbweb.war

## in order to run.
1. Obtain the sql-file and the war-file
2. place the sql-file in the '/mysql_autoload/'-directory.
3. place the seqdbweb.war in the '/srv/releases/'-directory.

##  deploy seqdbweb.war
0. login : $ docker exec -it 'container-name' bash
1. deploy: $ cp ~/releases/seqdbweb.war ~/webapps

## run 
1. 'make'

## tomcat-logs are found in
1. the '/srv/logs'-directory
