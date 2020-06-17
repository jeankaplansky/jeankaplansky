# Does it float?

    <?xml version="1.0" encoding="UTF-8"?>
    <project xmlns="http://maven.apache.org/POM/4.0.0"
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
            xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">

      <modelVersion>4.0.0</modelVersion>

      <groupId>com.deque</groupId>
      <artifactId>attest-java-examples-selenium2</artifactId>
      <version>0.0.1</version>
      <packaging>jar</packaging>

      <name>Attest Java Example - Selenium 2</name>
      <description>WorldSpace Attest automated testing for Java Example in JUnit</description>
      <url>https://bitbucket.org/samjonester/attest-java</url>

      <licenses>
        <license>
          <name>Mozilla Public License, Version 2.0</name>
          <url>https://www.mozilla.org/MPL/2.0/</url>
        </license>
      </licenses>

      <distributionManagement>
        <snapshotRepository>
          <id>ossrh</id>
          <url>https://oss.sonatype.org/content/repositories/snapshots</url>
        </snapshotRepository>
      </distributionManagement>

      <developers>
        <developer>
          <name>Deque Labs</name>
          <email>helpdesk@deque.com</email>
          <organization>Deque Labs</organization>
          <organizationUrl>http://www.deque.com</organizationUrl>
        </developer>

        <developer>
          <name>Test Double</>
          <email>hello@testdouble.com</email>
          <organization>Test Double</organization>
          <organizationUrl>http://testdouble.com</organizationUrl>
        </developer>
      </developers>

      <scm>
        <connection>scm:git@bitbucket.org:samjonester/attest-java.git</connection>
        <developerConnection>scm:git@bitbucket.org:samjonester/attest-java.git</developerConnection>
        <url>https://bitbucket.org/samjonester/attest-java</url>
      </scm>

      <properties>
        <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
     </properties>

      <repositories>
        <repository>
          <id>deque</id>
          <url>http://agora.dequecloud.com/artifactory/attest-java/</url>
        </repository>
      </repositories>

      <dependencies>
        <dependency>
          <groupId>com.deque</groupId>
          <artifactId>attest-java</artifactId>
          <version>3.0.0</version>
          <exclusions>
            <exclusion>
              <groupId>org.seleniumhq.selenium</groupId>
              <artifactId>selenium-java</artifactId>
            </exclusion>
          </exclusions>
        </dependency>

        <dependency>
          <groupId>org.seleniumhq.selenium</groupId>
          <artifactId>selenium-java</artifactId>
          <version>2.53.1</version>
        </dependency>

        <dependency>
          <groupId>junit</groupId>
          <artifactId>junit</artifactId>
          <version>4.12</version>
          <scope>test</scope>
        </dependency>
      </dependencies>
    </project>
