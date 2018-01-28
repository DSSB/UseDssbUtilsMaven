# UseDssbUtilsMaven
Example of how to use dssb-utils in a Maven project.

It basically boiled down to adding dssb maven repository (hosted by github).

```xml
	<repositories>
		<repository>
			<id>DssbUtils-mvn-repo</id>
			<url>https://raw.githubusercontent.com/dssb/maven-repository/master/</url>
			<snapshots>
				<enabled>true</enabled>
				<updatePolicy>always</updatePolicy>
			</snapshots>
		</repository>
	</repositories>

	<dependencies>
		<dependency>
			<groupId>dssb-utils</groupId>
			<artifactId>dssb-utils-common</artifactId>
			<version>2.0.0</version>
		</dependency>
		<dependency>
			<groupId>junit</groupId>
			<artifactId>junit</artifactId>
			<version>4.11</version>
			<scope>test</scope>
		</dependency>
	</dependencies>
```
See the full code here: (pom.xml)[https://github.com/DSSB/UseDssbUtilsMaven/blob/master/UseDssbUtilsMaven/pom.xml]
