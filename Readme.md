### Introduction

```xml
<dependency>
    <groupId>dev.xethh.libs.toolkits</groupId>
    <artifactId>bom-parent</artifactId>
    <version>1.0.1</version>
</dependency>
```

bom-parent is a centralized dependency group of maven bom for apply to maven project and used for maven archetype generation.
bom-parent is just the parent container for easy managing sub-projects such as bom and archetype.

```puml
bom-base
    -> bom-common
        -> bom-common-spring
            -> bom-common-spring-scala
            -> bom-common-spring-kotlin
```

#### bom-base  

```xml
<dependency>
    <groupId>dev.xethh.libs.toolkits</groupId>
    <artifactId>bom-base</artifactId>
    <version>1.0.1</version>
</dependency>
```
This is the base bom contains the maven plugin dependencies and plugins configuration for build java project.
This project also included the nexus plugin and gpg plugin for deploying open source to the repository.
  
  

#### bom-common
```xml
<dependency>
    <groupId>dev.xethh.libs.toolkits</groupId>
    <artifactId>bom-common</artifactId>
    <version>1.0.1</version>
</dependency>
```  
Bom common defined common libraries for all general use case and basic imported base dependency of junit, slf4j and DateUtils.  
#### bom-common-spring
```xml
<dependency>
    <groupId>dev.xethh.libs.toolkits</groupId>
    <artifactId>bom-common-spring</artifactId>
    <version>1.0.1</version>
</dependency>
```
Bom common for spring projects including fixed version of spring boot libraries and plugin.  

#### bom-common-spring-scala
```xml
<dependency>
    <groupId>dev.xethh.libs.toolkits</groupId>
    <artifactId>bom-common-spring-scala</artifactId>
    <version>1.0.1</version>
</dependency>
```
Bom common for spring, scala, and actor projects.

#### bom-common-spring-kotlin
```xml
<dependency>
    <groupId>dev.xethh.libs.toolkits</groupId>
    <artifactId>bom-common-spring-kotlin</artifactId>
    <version>1.0.1</version>
</dependency>
```
Bom common for spring and kotlin project.  
  

### Archetype
#### quickstart
```xml
<dependency>
    <groupId>dev.xethh.archetype</groupId>
    <artifactId>quickstart</artifactId>
    <version>1.0.1</version>
</dependency>
```
Maven archetype for generating java application project with basic libraries included in bom-common, the output is generally an executable jar.  


#### quickstart-lib
```xml
<dependency>
    <groupId>dev.xethh.archetype</groupId>
    <artifactId>quickstart-lib</artifactId>
    <version>1.0.1</version>
</dependency>
```
Maven archetype for generating java library project with basic libraries included in bom-common, the output is generally a non executable jar.  

#### quickstart-scala
```xml
<dependency>
    <groupId>dev.xethh.archetype</groupId>
    <artifactId>quickstart-scala</artifactId>
    <version>1.0.1</version>
</dependency>
```
Maven archetype for generating scala and java mixed application project with basic libraries included in bom-common-spring-scala, the output is generally an executable jar.  

#### quickstart-scala-lib
```xml
<dependency>
    <groupId>dev.xethh.archetype</groupId>
    <artifactId>quickstart-scala-lib</artifactId>
    <version>1.0.1</version>
</dependency>
```
Maven archetype for generating scala and java mixed library project with basic libraries included in bom-common-spring-scala, the output is generally a non executable jar.  
#### quickstart-kotlin
```xml
<dependency>
    <groupId>dev.xethh.archetype</groupId>
    <artifactId>quickstart-kotlin</artifactId>
    <version>1.0.1</version>
</dependency>
```
Maven archetype for generating kotlin and java mixed application project with basic libraries included in bom-common-spring-kotlin, the output is generally an executable jar.  
#### quickstart-kotlin-lib
```xml
<dependency>
    <groupId>dev.xethh.archetype</groupId>
    <artifactId>quickstart-kotlin-lib</artifactId>
    <version>1.0.1</version>
</dependency>
```
Maven archetype for generating kotlin and java mixed library project with basic libraries included in bom-common-spring-kotlin, the output is generally a non executable jar.  
