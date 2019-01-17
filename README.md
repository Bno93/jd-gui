# JD-GUI

JD-GUI, a standalone graphical utility that displays Java sources from CLASS files.

![App](http://jd.benow.ca/img/screenshot17.png)

- Java Decompiler projects home page: [http://jd.benow.ca](http://jd.benow.ca)
- Java Decompiler Wikipedia page: [http://en.wikipedia.org/wiki/Java_Decompiler](http://en.wikipedia.org/wiki/Java_Decompiler)
- JD-GUI source code: [https://github.com/java-decompiler/jd-gui](https://github.com/java-decompiler/jd-gui)

## Description

JD-GUI is a standalone graphical utility that displays Java source codes of
".class" files. You can browse the reconstructed source code with the JD-GUI
for instant access to methods and fields.

## How to build JD-GUI

Build Jar

```bash
> ./gradlew build
```

generate _"build/libs/jd-gui-x.y.z.jar"_

Build for OSX

```bash
> ./gradlew installOsxDist
```

generate _"build/install/jd-gui-osx/JD-GUI.app"_

Build for Windows

Downloas and unpack:

[http://sourceforge.net/projects/launch4j/files/launch4j-3/3.7/launch4j-3.7-win32.zip/download](http://sourceforge.net/projects/launch4j/files/launch4j-3/3.7/launch4j-3.7-win32.zip/download)

```bash
> gradlew.bat -DLAUNCH4J_HOME=.../path/to/launch4j-3.7-win32 installWindowsDist
```

generate _"build/install/jd-gui-windows/jd-gui.exe"_

Build for Ubuntu/Debian

```bash
> ./gradlew buildDeb
```

generate Ubuntu/Debian installer

Build for RedHat/CentOS/Fedora

```bash
> ./gradlew buildRpm
```

generate RedHat/CentOS/Fedora installer

## How to launch JD-GUI

- Double-click on _"jd-gui-x.y.z.jar"_
- Double-click on _"JD-GUI"_ application from Mac OSX
- Double-click on _"jd-gui.exe"_ application from Windows
- Execute _"java -jar jd-gui-x.y.z.jar"_ or _"java -classpath jd-gui-x.y.z.jar org.jd.gui.App"_

## How to use JD-GUI

- Open a file with menu "File > Open File..."
- Open recent files with menu "File > Recent Files"
- Drag and drop files from your file explorer

## How to extend JD-GUI

``` bash
> ./gradlew idea
```

generate Idea Intellij project

```bash
> ./gradlew eclipse
```

generate Eclipse project

```bash
> java -classpath jd-gui-x.y.z.jar;myextension1.jar;myextension2.jar org.jd.gui.App
```

launch JD-GUI with your extensions

## How to uninstall JD-GUI

- Java: Delete "jd-gui-x.y.z.jar" and "jd-gui.cfg".
- Mac OSX: Drag and drop "JD-GUI" application into the trash.
- Windows: Delete "jd-gui.exe" and "jd-gui.cfg".
