# h2o-flow-intro
Hands-on introduction to H2O flow

## Installing h2o.ai 

Visit https://www.h2o.ai/, click "Open Source" and select "H2O Download Latest". On the next page, click on the Downlad Latest button. 

This will download a zip file.

Unzip the zip file (in Windows you can do this using your File Explorer), and on Mac, the it should automatically save as an unzipped folder where you downloaded it.

**h2o.ai needs Java to run**

## Installing Java

Java 8, 9, 10, 11, 12, 13, 14, 15 are all supported.

To run the H2O binary using either the command line, R, or Python packages, only 64-bit JRE is required.

Both of these are available on the Java download page, http://www.oracle.com/technetwork/java/javase/downloads/index.html. 

## Data

All of the data we will be using is at https://vanderbilt.box.com/s/jf1lpr0lm2tk071brdcgpn9uz7yce07m. 

## Starting H2O

Get started with H2O in 3 easy steps
1. Download H2O. This is a zip file that contains everything you need to get started.

2. From your terminal, run:

cd ~/Downloads
unzip h2o-3.32.1.4.zip
cd h2o-3.32.1.4
java -jar h2o.jar
3. Point your browser to http://localhost:54321

## Importing Your Data

In the H2O flow browser window, click on ImportFiles

Navigate to where your data is stored, and copy the location.

Paste this location into the Search field in the Import Fields cell. 
