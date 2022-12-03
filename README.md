# JavaFX / JLink / JPackage Gradle Template

Gradle template for quick start developing GUI applications using `JavaFX`, automatic image creation with `JLink` and simple packaging with `JPackage`.

![jpackage output](/images/output.png)

---

## Setup

Change some values in the following files to customize the project  
(all places of changes are supplemented by comments):
- settings.gradle
- build.gradle
- module-info.java
- group and artifact-id inside the `/src/main/java` folder

Also delete `/images` folder

---

### Packaging to the JAR

    .\gradlew.bat jar

Packaged JAR will be available in `\build\libs`

### Creating Runtime Image

    .\gradlew.bat jlink

Created image will be available in `\build\image`

### Packaging for distribution

    .\gradlew.bat jpackage

Created executables will be available in `\build\jpackage`

#### NOTE: Java version 14 or higher is required to use jpackage and [WIX Toolset](https://wixtoolset.org/) must be installed to create `exe` or `msi` executable files.

---

## Final result

Final result after executing `.\gradlew.bat jpackage` command, installing and launching  

![jpackage output](/images/run.png)