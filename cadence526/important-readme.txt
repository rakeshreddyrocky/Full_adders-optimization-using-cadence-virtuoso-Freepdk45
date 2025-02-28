Overview

This document provides clear instructions on updating the cds.lib file to reflect the correct directory paths for library definitions in Cadence. This ensures that all required standard and custom libraries are accessible within the Cadence environment.

Steps to Update the cds.lib File

Locate the cds.lib File:

The cds.lib file is typically found in your Cadence working directory.

If unsure, use the command:

find ~ -name "cds.lib"

Open the file using a text editor:

nano cds.lib

or

vi cds.lib

Modify Directory Locations:

Update the DEFINE statements to reflect your directory structure.

Replace /u/kunduru/FreePDK45/ncsu_basekit/cdssetup/cadence526/ with your directory path where required.

Example of Updating Paths:

If your directory path is /u/your_username/FreePDK45/, modify lines accordingly:

DEFINE AND /u/your_username/FreePDK45/ncsu_basekit/cdssetup/cadence526/AND
DEFINE OR /u/your_username/FreePDK45/ncsu_basekit/cdssetup/cadence526/OR
DEFINE NAND /u/your_username/FreePDK45/ncsu_basekit/cdssetup/cadence526/NAND

Ensure all required libraries are correctly defined.

Comment Out Unused Definitions:

If a library is not needed, comment it out by adding # at the beginning of the line:

#DEFINE old_library /u/kunduru/FreePDK45/old_library

Save and Exit:

If using nano, press CTRL + X, then Y, and hit Enter.

If using vi, press ESC, type :wq, and hit Enter.

Verify Changes:

Restart Cadence and check if all libraries are loaded correctly.

If issues arise, check for typos or incorrect paths.

Notes

Always make a backup of the original cds.lib file before making changes:

cp cds.lib cds.lib.bak

Ensure you have the correct permissions to edit the file.

Coordinate with your team to maintain consistency across systems.

Conclusion

Following these steps ensures that your Cadence environment is correctly configured with the appropriate libraries. If any issues persist, consult the system administrator or check the Cadence documentation for troubleshooting tips.
