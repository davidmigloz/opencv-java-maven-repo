# OpenCV Java Bindings for Maven

OpenCV Java bindings packaged with native libraries to be imported as Maven dependecy.

## Usage

Add to your Maven project `pom.xml`:

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
      <!-- OpenCV native libs -->
      <groupId>com.davidmiguel</groupId>
      <artifactId>opencvjar-runtime</artifactId>
      <version>3.1.0</version>
      <classifier>natives-windows-x86_64</classifier>
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

And load OpenCV in your Java class:

```java
public class App {
    static{ System.loadLibrary(Core.NATIVE_LIBRARY_NAME); }

    public static void main(String[] args) {
        System.out.println("Welcome to OpenCV " + Core.VERSION);
    }
}
```

## Versions supported

- OpenCV 3.0.0
- OpenCV 3.1.0
- OpenCV 3.2.0

## Platforms supported

OS | Architecture
--- | ---
Windows | natives-windows-x86
Windows | natives-windows-x86_64

## License

[3-clause BSD License](https://github.com/opencv/opencv/blob/master/LICENSE)

Copyright (C) 2000-2016, Intel Corporation, all rights reserved.  
Copyright (C) 2009-2011, Willow Garage Inc., all rights reserved.  
Copyright (C) 2009-2016, NVIDIA Corporation, all rights reserved.  
Copyright (C) 2010-2013, Advanced Micro Devices, Inc., all rights reserved.  
Copyright (C) 2015-2016, OpenCV Foundation, all rights reserved.  
Copyright (C) 2015-2016, Itseez Inc., all rights reserved.  
Third party copyrights are property of their respective owners.

