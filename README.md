# ResourcesTest


## feature/rs-filter

Working on understanding building using Profiles

  - Introduced filter files (local.properties, dev.properties)
  - Introduced profile tags. These are driven by appending '-P[profile id]' to the 'mvn clean install' command.
  
## master  

This is a test to see what the combination is needed for property variables to properly filter variables. Here are the requirements:

  - Spring-boot parent v1.4.2
  - 'resources' folder registered in pom.xml and marked with 'filtering' set to 'true'
  - create 'src/main/filters' folder and make sure it's on the buld path
  - Have file with real value in the 'filters' folder.
  - Use @****@ annotation when referencing variables in destination file (ie. resources/application.properties)


Markdown reference:
http://dillinger.io/