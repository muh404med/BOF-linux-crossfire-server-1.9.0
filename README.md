# BOF-linux-crossfire-server-1.9.0

Three Python scripts showcasing different aspects of exploiting a buffer overflow vulnerability in "crossfire-server" version 1.9.0. The scripts demonstrate offset fuzzing, bad character identification, and a remote code execution exploit.

## Install Vulnerable Service

To install the vulnerable service, follow these steps:

1. Download the crossfire-server package:

sudo wget www.offensive-security.com/crossfire.tar.gz


2. Extract the package:

sudo tar -zxf crossfire.tar.gz


3. Copy the extracted files to the appropriate directory:

sudo cp -r crossfire /usr/games/


## Run Vulnerable Service

To run the vulnerable service, follow these steps:

1. Change to the crossfire-server directory:

sudo cd /usr/games/crossfire/bin/


2. Run the server:

sudo ./crossfire


## Scripts

This repository contains the following scripts:

1. `offset_fuzzing.py`: This script demonstrates how to fuzz the offset to find the correct buffer size to overwrite the EIP.

2. `BadCharsDiscover.py`: This script demonstrates how to identify bad characters that cannot be used in the payload.

3. `remote_code_execution.py`: This script demonstrates the final exploit that triggers the buffer overflow and achieves remote code execution.
