# QAS Electronic Updates Metadata REST API Java Sample Integration Code

## Overview

This directory contains a Java application that can be used to determine what data files are available to download for an account, generate download URLs for the files and then download them onto the local file system.

Further documentation of the application is provided by the comments in the source code itself.

*This documentation describes the application as found in this [Git repository](https://github.com/experiandataquality/electronicupdates). It may no longer apply if you modify the sample code.*

## Prerequisites

### Compilation and Debugging

The following prerequisites are required to compile and debug the application:

 * [Java](https://java.com/en/download/) 1.7.0 (or later);
 * [Apache Ant](http://ant.apache.org/bindownload.cgi) 1.9.3 (or later);
 * [Eclipse](https://eclipse.org/downloads/) 3.8.1 (or later).

### Runtime

The following prerequisites are required to run the compiled application:

 * [Java](https://java.com/en/download/) 1.7.0 (or later).

## Compliation

To compile the application, you can do any of the following:

### Linux

 * Import the project into Eclipse;
 * Run ```./build.sh``` from the terminal.

### Windows

 * Import the project into Eclipse;
 * Run ```Build.cmd``` from the command prompt.

## Setup

To set up the application, set your credentials in the ```QAS_ElectronicUpdates_UserName``` and ```QAS_ElectronicUpdates_Password``` environment variables just before running the application.

Other approaches for loading the credentials are possible but are considered outside the scope of this documentation.

## Usage

To run the application, execute the following command from the directory containing the compiled JAR file:

### Linux

```sh
java -jar MetadataWebApi.jar
```

### Windows

```batchfile
java -jar MetadataWebApi.jar
```

## Example Usage

Below is an example set of commands that could be run on Linux to download all the latest data files from QAS Electronic Updates onto the local machine into a ```QASData``` directory in the same directory as the application

```sh
export QAS_ElectronicUpdates_UserName=MyUserName
export QAS_ElectronicUpdates_Password=MyPassword
java -jar MetadataWebApi.jar
```

## Compatibility

This application has been compiled and tested on the following platforms:

 * Java 1.7.0_79 (x64), Eclipse 3.8.1 and Apache Ant 1.9.3 on Ubuntu 14.04.2 LTS;
 * Java 1.8.0_45 (x64), Eclipse Luna SR2 (4.4.2) and Apache Ant 1.9.4 on Windows 8.1 (Build 9600).
