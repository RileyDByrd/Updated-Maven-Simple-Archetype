# Updated-Maven-Simple-Archetype
The Maven Simple Archetype updated to the latest Java version and JUnit version with required properties, driver class, and tester class.


# Getting the Archetype 
The easiest way to get the archetype with an I.D.E. like Eclipse or IntelliJ is to add this U.R.L. to your list of Maven catalogs, `https://github.com/WhiteHatHacker1/Updated-Maven-Simple-Archetype/raw/master/archetype-catalog.xml`. Alternatively, if this link isn't working for you, you may try this one, `https://raw.githubusercontent.com/WhiteHatHacker1/Updated-Maven-Simple-Archetype/master/archetype-catalog.xml`.

JAR files are also available for the one who prefers to do it himself. The following command will install the archetype and update the local catalog.

`mvn install:install-file archetype:update-local-catalog -Dfile=path/to/Updated-Maven-Simple-<version>.jar -DpomFile=path/to/pom.xml -f path/to/pom.xml`


# Deploying the Repo
Deploy the repo with `mvn deploy -DaltDeploymentRepository=local::default::file:.` from the project's root directory.


# Updating the Catalog
Update the catalog with `mvn archetype:crawl -Drepository=.` from the project's root directory.
