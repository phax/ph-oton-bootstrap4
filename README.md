# ph-oton-bootstrap4

[![Maven Central](https://img.shields.io/maven-central/v/com.helger.photon/ph-oton-bootstrap4-parent-pom)](https://img.shields.io/maven-central/v/com.helger.photon/ph-oton-bootstrap4-parent-pom)
[![javadoc](https://javadoc.io/badge2/com.helger.photon/ph-oton-bootstrap4/javadoc.svg)](https://javadoc.io/doc/com.helger.photon/ph-oton-bootstrap4)

This set of Java libraries forms a package to build Java web applications.

Contained subprojects are:
* ph-oton-bootstrap4 - Java Wrapper for the Bootstrap 4 controls
* ph-oton-bootstrap4-uictrls - special UI controls for Bootstrap 4
* ph-oton-bootstrap4-pages - predefined UI pages with Bootstrap 4 styling
* ph-oton-bootstrap4-stub - Servlet stub for Bootstrap 4 web applications
* ph-oton-bootstrap4-demo - a standalone demo web application to be run in Tomcat or in provided Jetty

# Requirements

* Java 17+ is required for building 
* Application server requirement JakartaEE 10:
    * At least Tomcat 10.1
    * Jetty 12.x with AnnotationConfiguration enabled
      
## Maven usage

Replace `x.y.z` with the effective version number.

```xml
  <dependencyManagement>
    <dependencies>
      <dependency>
        <groupId>com.helger.photon</groupId>
        <artifactId>ph-oton-bootstrap4-parent-pom</artifactId>
        <version>x.y.z</version>
        <type>pom</type>
        <scope>import</scope>
      </dependency>
    </dependencies>
  </dependencyManagement>
```

### Bootstrap 4

To use Bootstrap 4 front end use:

```xml
  <dependencies>
    <dependency>
      <groupId>com.helger.photon</groupId>
      <artifactId>ph-oton-bootstrap4-stub</artifactId>
    </dependency>
  </dependencies>
```

See the submodule `ph-oton-bootstrap4-demo` for a working example project with Bootstrap 4 UI.

## News and noteworthy

v10.0.1 - work in progress
* Slightly improved the page with the scheduled actions

v10.0.0 - 2025-08-25
* Requires Java 17 as the minimum version
* Updated to ph-commons 12.0.0
* Updated to Jetty 12.1.0
* Extracted from ph-oton

---

My personal [Coding Styleguide](https://github.com/phax/meta/blob/master/CodingStyleguide.md) |
It is appreciated if you star the GitHub project if you like it.