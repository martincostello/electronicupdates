# QAS Electronic Updates Metadata REST API Python Script

## Overview

This directory contains a Python script that can be used to determine what data files are available to download for an account, generate download URLs for the files and then download them onto the local file system.

Further documentation of the script is provided by the comments in the Python script itself.

*This documentation describes the script as found in this [Git repository](https://github.com/experiandataquality/electronicupdates). It may no longer apply if you modify the sample code.*

## Prerequisites

 * [Python](https://www.python.org/downloads/) 2.7.6 (or later);
 * The [requests](http://docs.python-requests.org/en/latest/) Python module.

## Setup

To set up the script for usage you could either:

 1. Set your credentials in the ```QAS_ElectronicUpdates_UserName``` and ```QAS_ElectronicUpdates_Password``` environment variables just before running the script (**recommended**);
 1. Hard-code the credentials into the script. This approach is **not** recommended as the credentials are stored in plaintext and could represent a security risk.

Other approaches are possible but are considered outside the scope of this documentation.

To install the ```requests``` dependency if it is not already installed, execute the following command:

### Linux/OS X

```sh
pip install requests
```

or

```sh
sudo easy_install requests
```

## Usage

To run the script, execute the following command from the directory containing the script:

### Linux/OS X

```sh
./metadatawebapi.py
```

### Windows

```batchfile
py .\metadatawebapi.py
```

## Example Usage

Below is an example set of commands that could be run on Linux to download all the latest data files from QAS Electronic Updates onto the local machine into a ```QASData``` directory in the same directory as the script:

```sh
export QAS_ElectronicUpdates_UserName=MyUserName
export QAS_ElectronicUpdates_Password=MyPassword
./metadatawebapi.py
```

## Compatibility

This script was tested with the following Python versions and platforms:

 * Python 2.7.6 on Ubuntu 14.04.2 LTS;
 * Python 2.7.10 on OS X Yosemite (10.10.2);
 * Python 3.3.2 on Windows 8.1 (Build 9600).
