APIviz
A fork of the 1.3.x branch of Trustin Lee's APIviz project.

Changes

Convert the repository from Subversion to Git.
Add support for building with Java 8.
Switch to a fork of JDepend that supports class files compiled with Java 8.
Build as a normal jar, instead of a fat jar.
Tidy up and simplify the POM.
Installation

This project is available in the Maven Central Repository. Add the following to the Javadoc configuration in your pom.xml file to use it:

<doclet>org.jboss.apiviz.APIviz</doclet>
<docletArtifact>
  <groupId>com.grahamedgecombe.apiviz</groupId>
  <artifactId>apiviz</artifactId>
  <version>1.3.4</version>
</docletArtifact>
<additionalparam>
  -sourceclasspath ${project.build.outputDirectory}
</additionalparam>
The artifacts are signed with my personal GPG key.

License

APIviz is available under version 2.1 or later of the GNU LGPL. See the LICENSE.txt file for the full terms.
