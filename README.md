# maven-demo
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/maven-v4_0_0.xsd">
  <modelVersion>4.0.0</modelVersion>
  <groupId>com.ananthakumaran</groupId>
  <artifactId>maven-demo</artifactId>
  <packaging>jar</packaging>
  <version>1.2.7-SNAPSHOT</version>
  <name>maven-demo</name>
  <url>http://maven.apache.org</url>
  <dependencies>
    <dependency>
      <groupId>junit</groupId>
      <artifactId>junit</artifactId>
      <version>3.8.1</version>
      <scope>test</scope>
    </dependency>
  </dependencies>

  <scm>
    <connection>
      scm:git:http://github.com/ananthakumaran/maven-demo.git
    </connection>
    <developerConnection>
      scm:git:http://github.com/ananthakumaran/maven-demo.git
    </developerConnection>
    <url>
      http://github.com/ananthakumaran/maven-demo
    </url>
  </scm>

  <build>
    <plugins>
      <plugin>
	<artifactId>maven-release-plugin</artifactId>
	<configuration>
	  <localCheckout>true</localCheckout>
	</configuration>
      </plugin>
    </plugins>
  </build>

  <distributionManagement>
    <site>
      <id>maven-demo</id>
      <url>file:///${basedir}/../../../temp</url>
    </site>
    <repository>
      <id>maven-demo</id>
      <url>file:///${basedir}/../../../temp/maven2</url>
    </repository>
  </distributionManagement>	
</project>
