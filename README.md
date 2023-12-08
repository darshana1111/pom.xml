<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 https://maven.apache.org/xsd/maven-4.0.0.xsd">
	<modelVersion>4.0.0</modelVersion>
	<groupId>DemoBlazeAutomation</groupId>
	<artifactId>DemoBlazeAutomation</artifactId>
	<version>0.0.1-SNAPSHOT</version>


	<!-- Plug-ins required for executing Tests  -->
	<build>
		<plugins>
			<plugin>
				<groupId>org.apache.maven.plugins</groupId>
				<artifactId>maven-compiler-plugin</artifactId>
				<configuration>
					<source>1.7</source>
					<target>1.7</target>
				</configuration>
			</plugin>
			<plugin>
				<groupId>org.apache.maven.plugins</groupId>
				<artifactId>maven-surefire-plugin</artifactId>
				<version>2.18.1</version>
				<configuration>
					<testFailureIgnore>true</testFailureIgnore>
					<suiteXmlFiles>
						<!-- TestNG suite XML files -->
						<suiteXmlFile>testng.xml</suiteXmlFile>
					</suiteXmlFiles>
				</configuration>
			</plugin>

		</plugins>

	</build>


	<dependencies>
	
	<!-- Added this dependency to resolve java.lang.IllegalAccessError: class lombok.javac.apt.LombokProcessor error in maven  -->
		<dependency>
			<groupId>org.projectlombok</groupId>
			<artifactId>lombok</artifactId>
			<version>1.18.22</version>
		</dependency>


		<!-- https://mvnrepository.com/artifact/com.aventstack/extentreports -->
		<dependency>
			<groupId>com.aventstack</groupId>
			<artifactId>extentreports</artifactId>
			<version>5.0.9</version>
		</dependency>


		<!-- Dependency to generate random email address -->
		<!-- https://mvnrepository.com/artifact/org.apache.commons/commons-lang3 -->
		<dependency>
			<groupId>org.apache.commons</groupId>
			<artifactId>commons-lang3</artifactId>
			<version>3.12.0</version>
		</dependency>


		<dependency>
			<groupId>org.seleniumhq.selenium</groupId>
			<artifactId>selenium-java</artifactId>
			<version>4.1.1</version>
		</dependency>

		<dependency>
			<groupId>org.apache.poi</groupId>
			<artifactId>poi-ooxml</artifactId>
			<version>5.0.0</version>
		</dependency>


		<!-- https://mvnrepository.com/artifact/org.testng/testng -->
		<dependency>
			<groupId>org.testng</groupId>
			<artifactId>testng</artifactId>
			<version>7.1.0</version>
			<scope>compile</scope>
		</dependency>

		<!-- https://mvnrepository.com/artifact/log4j/log4j -->
		<dependency>
			<groupId>log4j</groupId>
			<artifactId>log4j</artifactId>
			<version>1.2.17</version>
		</dependency>


	</dependencies>


</project>
