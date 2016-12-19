# osgi-test
OSGI test parent is a maven multi module project which contains the maven module osgi-test-provider and osgi-test-consumer

### Compile and Build Jar
mvn clean install

### Karaf installation
feature:repo-add mvn:biz.neustar.osgi/osgi-test/1.1.1/xml/features
feature:install osgi-test (This will start printing Hello World)

### Development commands
Create a Feature maven project
1. To create a maven features module:
mvn archetype:generate -DarchetypeGroupId=org.apache.karaf.archetypes   -DarchetypeArtifactId=karaf-feature-archetype -DarchetypeVersion=4.0.7 -DgroupId=biz.neustar.osgi -DartifactId=osgi-test-features -Dversion=1.0.1
