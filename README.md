# h2o-flow-intro
Hands-on introduction to H2O flow

## Overview

![image](https://user-images.githubusercontent.com/5521243/127340885-830186d4-06fb-41f9-9bba-579f4ecaf647.png)

The lifecycle of a data science project has many parts, and often requires the coordinated work of an entire team. Today, we'll be examining one small, but very important part of the process--training and testing machine learning algorithms (Modeling and Assessment, above). 


## Installing h2o.ai 

Visit https://www.h2o.ai/, click "Open Source" and select "H2O Download Latest". On the next page, click on the Downlad Latest button. 

This will download a zip file.

Unzip the zip file (in Windows you can do this using your File Explorer), and on Mac, the it should automatically save as an unzipped folder where you downloaded it.

**h2o.ai needs Java to run**

## Installing Java

Java 8, 9, 10, 11, 12, 13, 14, 15 are all supported.

To run the H2O binary using either the command line, R, or Python packages, only 64-bit JRE is required.

As the most recent version of Java is unsupported by h2o, please either use a previous version of Java, or download Java SE 15 from the following link: https://www.oracle.com/java/technologies/javase/jdk15-archive-downloads.html

Note that you may need to sign in to or create a new Oracle account in order to download a previous version of Java. Follow the installation instructions given after downloading the right installer for your machine. 

To check which version of Java you have on your machine, write ```java --version``` in Terminal if you are on a Mac or ```java -version``` if you are using Windows. 

Downgrading from Java 16 to 15 can be challenging. One approach is to delete Java 16 where it is stored in your system files or follow the instructions at this link **at your own risk** https://www.java.com/en/download/help/uninstall_java.html. You may be unable to do this during the workshop. 

## Data

All of the data we will be using is at https://vanderbilt.box.com/s/jf1lpr0lm2tk071brdcgpn9uz7yce07m. 

## Starting H2O

Get started with H2O in 3 easy steps
1. Download H2O. This is a zip file that contains everything you need to get started.

2. From your terminal, run:

```cd ~/Downloads```

```unzip h2o-3.32.1.4.zip```

```cd h2o-3.32.1.4```

```java -jar h2o.jar```

Then, point your browser to http://localhost:54321

## Importing Your Data

In the H2O flow browser window, click on ImportFiles

Navigate to where your data is stored, and copy the location. On Mac, you can select the file and press option + right click (two finger click on a trackpad) to copy the file location as a pathname.

Paste this location into the Search field in the Import Fields cell. 
