# OpenCV Java Bindings for Maven

OpenCV Java bindings packaged with native libraries to be imported as Maven dependecy.

```xml
<project>
  
  <!-- ... -->
  
  <dependencies>
    
    <!-- ... -->
    
    <dependency>
      <!-- OpenCV API -->
      <groupId>com.davidmiguel</groupId>
      <artifactId>opencvjar</artifactId>
      <version>3.1.0</version>
    </dependency>
    
    <dependency>
      <!-- OpenCV API -->
      <groupId>com.davidmiguel</groupId>
      <artifactId>opencvjar</artifactId>
      <version>3.1.0</version>
    </dependency>
    
    <!-- ... -->
    
  </dependencies>
  
  <!-- ... -->
  
  <repositories>
      <repository>
          <id>opencv-maven-repo</id>
          <url>https://raw.github.com/davidmigloz/opencv-java-maven-repo/master</url>
      </repository>
  </repositories>
</project>
```


```xml
<repositories>
    <repository>
        <id>opencv-maven-repo</id>
        <url>https://raw.github.com/davidmigloz/opencv-java-maven-repo/master</url>
    </repository>
</repositories>
```

## Versions supported

- OpenCV 3.0.0
- OpenCV 3.1.0

## Platforms supported

OS | Architecture
--- | ---
Windows | natives-windows-x86
Windows | natives-windows-x86_64
