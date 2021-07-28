# h2o-flow-intro
Hands-on introduction to H2O flow

## Overview

![image](https://user-images.githubusercontent.com/5521243/127340885-830186d4-06fb-41f9-9bba-579f4ecaf647.png)

The lifecycle of a data science project has many parts, and often requires the coordinated work of an entire team. Today, we'll be examining one small, but very important part of the process--training and testing machine learning algorithms (Modeling and Assessment, above). 

In this workshop, we'll start with a brief overview of machine learning. *Note that we are not following best practices today.*

We'll tackle the problem of how to find evidence of where toolmakers from stone-age societies plied their craft by analyzing individual particles in soil samples! See https://www.tandfonline.com/doi/abs/10.1080/01977261.2020.1860351 for background on the particle analysis approach. 

Outline:
- Installing software, downloading data
- Ancient Artifacts problem
- Breakout room 1: How would you identify 200 particles in a million?? (follow instructions at https://docs.google.com/document/d/1K1HJMNj7HZgxrqzV3FI6MlgyLfQcfC8LyMQneV5IZSU/edit?usp=sharing)
- Hands-on Ancient Artifact Machine Learning approach
- Breakout room 2: Trying out different models
- Assessing how well our model works


## Installing h2o.ai 

Visit https://www.h2o.ai/, click "Open Source" and select "H2O Download Latest". On the next page, click on the Downlad Latest button. 

This will download a zip file.

Unzip the zip file (in Windows you can do this using your File Explorer), and on Mac, the it should automatically save as an unzipped folder where you downloaded it.

**h2o.ai needs Java to run**

## Installing Java

Java 8, 9, 10, 11, 12, 13, 14, 15 are all supported. **Note the that latest version, Java 16, is not supported.**

Only 64-bit JRE is required.

As the most recent version of Java is unsupported by h2o, please either use a previous version of Java, or download Java SE 15 from the following link: https://www.oracle.com/java/technologies/javase/jdk15-archive-downloads.html

Note that you may need to sign in to or create a new Oracle account in order to download a previous version of Java. Follow the installation instructions given after downloading the right installer for your machine. 

To check which version of Java you have on your machine, write ```java --version``` in Terminal if you are on a Mac or ```java -version``` if you are using Windows. 

Downgrading from Java 16 to 15 can be challenging. One approach is to delete Java 16 where it is stored in your system files or follow the instructions at this link **at your own risk** https://www.java.com/en/download/help/uninstall_java.html. You may be unable to do this during the workshop. 

## Data

All of the data we will be using is at https://vanderbilt.box.com/s/jf1lpr0lm2tk071brdcgpn9uz7yce07m. Browse to the shared folder, and download each file by hovering over the name, then clicking on the three-dot menu, "More Options". Select "Download".

![image](https://user-images.githubusercontent.com/5521243/127345107-a7454cb5-7d73-4531-897c-f7c8b9c9a7e2.png)


## Starting H2O

Get started with H2O in 3 easy steps
1. Download H2O. This is a zip file that contains everything you need to get started.
2. Extract the files using File Explorer
3. From your terminal, run:

```cd ~/Downloads/h2o-3.32.1.4```

```java -jar h2o.jar```

Then, point your browser to http://localhost:54321

## Importing Your Data

First, you'll want to 

In the H2O flow browser window, click on ImportFiles

Navigate to where your data is stored, and copy the location. 

On Windows, open File Explorer (you can right-click on Start and selece File Explorer). Navigate to your Downloads folder, and right-click on the "ancient_artifact.csv", and select "Properties". Copy the location in "Location:"

Mac, you can select the file and press option + right click (two finger click on a trackpad) to copy the file location as a pathname.

Paste this location into the Search field in the Import Fields cell. 
