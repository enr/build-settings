# Build settings

[![](https://jitpack.io/v/enr/build-settings.svg)](https://jitpack.io/#enr/build-settings)

Java build settings.

Add the JitPack repositories to your build file

```xml
<repositories>
  <repository>
    <id>jitpack.io</id>
    <url>https://jitpack.io</url>
  </repository>
</repositories>
<pluginRepositories>
  <pluginRepository>
    <id>jitpack.io</id>
    <url>https://jitpack.io</url>
  </pluginRepository>
</pluginRepositories>
```

Add the dependency:

```xml
<dependency>
  <groupId>com.github.enr</groupId>
  <artifactId>build-settings</artifactId>
  <version>1.2.0</version>
</dependency>
```

Usage with `net.revelc.code.formatter:formatter-maven-plugin`:

```xml
<plugin>
  <groupId>net.revelc.code.formatter</groupId>
  <artifactId>formatter-maven-plugin</artifactId>
  <version>2.23.0</version>
  <dependencies>
    <dependency>
      <groupId>com.github.enr</groupId>
      <artifactId>build-settings</artifactId>
      <version>1.2.0</version>
    </dependency>
  </dependencies>
  <configuration>
    <!-- paths in build-settings jar -->
    <configFile>fmt/eclipse-formatter-config.xml</configFile>
    <configXmlFile>fmt/xml.properties</configXmlFile>
    <!-- ... -->
  </configuration>
</plugin>
```
