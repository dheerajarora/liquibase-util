liquibase-util
==============

This project is created to use very few(only one) functionality of liquibase i.e., to generate changelog file with and without table data but there is always a scope to extend the functionality to perform more operations of liquibase through maven.

### Functionality:

There is a properties file in resources, liquibase.properties having some properties required by liquibase to generate change logs:

`url=jdbc:mysql://localhost:3306/<<DB SCHEMA NAME>>`
`username=<<DB USERNAME>>`
`password=<<DB PASSOWRD>>`
`driver=com.mysql.jdbc.Driver`
`verbose=true`
`emptyPassword=false`

And thats it! just run the maven build with clean install. It will generate the change log files for you in main/resources folder.