## Logback JSON BOM
Bill of materials for Logback JSON.

## Usage
In your parent POM or project POM, add the BOM to the `dependencyManagement` section:
```
<dependencyManagement>
    <dependencies>
        ...
        <dependency>
            <groupId>com.eoniantech.build</groupId>
            <artifactId>logback-json-bom</artifactId>
            <version>0.1.5</version>
            <type>pom</type>
            <scope>import</scope>
        </dependency> 
        ...
    </dependencies> 
<dependencyManagement>
```

Then, in the `dependencies` section of your project POM, depend on specific Logback JSON components without the version:

```
<dependencies>
    ....
    <dependency>
        <groupId>ch.qos.logback.contrib</groupId>
        <artifactId>logback-json-classic</artifactId>
    </dependency>
    <dependency>
        <groupId>ch.qos.logback.contrib</groupId>
        <artifactId>logback-jackson</artifactId>
    </dependency> 
    ...
</dependencies>   
