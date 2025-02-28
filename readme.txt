README: Setting Up FreePDK45 for Cadence

Overview

This document provides step-by-step instructions to download and set up FreePDK45 for use with Cadence.

Step 1: Download FreePDK45

Open a web browser and go to the following link:
FreePDK45 GitHub Repository

Click on the "Code" button and select "Download ZIP" to download the repository.

Once downloaded, extract the contents to your desired directory.

Step 2: Copy cadence526 to the Required Path

Navigate to the extracted FreePDK45 folder.

Locate the cadence526 directory.

Copy the cadence526 directory to the following path:

cp -r cadence526 /u/username/FreePDK45/ncsu_basekit/cdssetup/

Replace username with your actual system username.

Step 3: Verify the Setup

Ensure that the copied files are in the correct location:

ls /u/username/FreePDK45/ncsu_basekit/cdssetup/

You should see the cadence526 directory listed.


Step 4: Initiate Cadence Virtuoso

Navigate to the required directory:

cd /u/username/FreePDK45/ncsu_basekit/cdssetup/cadence526/

Run the following commands in the terminal:

tcsh
source setup.tcl
virtuoso &

Notes

Ensure that you have the necessary permissions to create and copy files in the destination directory.

If you encounter any issues, verify that the download and extraction processes were completed correctly.

Conclusion

Following these steps will ensure that FreePDK45 is properly set up for use in Cadence. If further configuration is needed, consult the project documentation or reach out for support.
