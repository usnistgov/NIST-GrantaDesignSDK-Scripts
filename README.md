
# README.md

The scripts and programs in "NIST-GrantaDesignSDK-Scripts" are utility programs developed in the NIST Center for Automotive Lightweighting (NCAL) to interact with a Granta Design materials information system. These scripts use the MI:Scripting Toolkit for Python provided by Granta Design.

These programs were developed by Olivier Marie-Rose (olivier.marie-rose@nist.gov). Questions regarding these scripts may be directed to Adam Creuziger (adam.creuziger@nist.gov)

While readable as a plain text, this README.md file uses Markdown formatting.

For more information about Granta Design, the Granta Design materials information management system "MI", or the Python Software development kit (SDK) "MI:Scripting Toolkit" see:
 - http://www.grantadesign.com
 - http://www.grantadesign.com/products/mi/index.htm
 - http://support.grantadesign.com/resources/miscriptingtoolkit/python/1.4/index.htm

## NIST Disclaimers

Certain commercial equipment, instruments, or materials are identified in order to specify the experimental and computational procedure adequately. Such identification is not intended to imply recommendation or endorsement by the National Institute of Standards and Technology, nor is it intended to imply that the materials or equipment identified are necessarily the best available for the purpose.

## These scripts should be cited as:

O. Marie-Rose, A. Creuziger, "NIST-GrantaDesignSDK-Scripts", https://github.com/usnistgov/NIST-GrantaDesignSDK-Scripts

The commit hash and list of programs used should be included if applicable.

## NIST License

 See LICENSE.TXT

# Creation Date and Key Updates
 Date | File | Release type
 --- | --- | ---
 2018 May 08 | ImportSingleImage.ipynb | New
 2018 May 08 | ImportMultipleImages.ipynb | New

  - Scripts with extension .ipynb have been implemented as Jupyter notebooks.

# Prerequisites and use

## Prerequisities
 - Active Granta Design license and database
 - Windows or linux workstation. Currently the SDK is limited to Windows and some Linux operating systems.  **Mac operating systems will not be unable to use these scripts.**
 - Workstation Prerequisites:
  - Python Software development kit (SDK) from Granta Design, version 1.4 or later. For NCAL users, this is available at http://wsancalp01.nist.gov/NCAL/UpdatePackages/.  All other users will need to contact Granta Design.
  - Python 3.5 or later
  - Package Dependencies (included as a conda .yml file "NIST-GrantaDesignSDK_.yml")
  - Jupyter Notebook
  - Local copy of the script you would like to use

We have used the conda and anaconda package management system and environment management system, but these are not required. The following links may be useful for assistance in installing conda and/or anaconda.
- https://conda.io/docs/user-guide/install/index.html
- https://docs.anaconda.com/anaconda/install/

If you are using anaconda, a new environment can be created by importing the .yml file (import button under the "Environments" tab in Anaconda Navigator).

## ImportSingleImage.ipynb Use
 - Open and run the file through Jupyter notebook
 - Example filenames are included in the script. You will need to modify these for your use.
  - Identify the **database key** for your installation of Granta Design MI ("MI_NIST_NCAL" in this example).
  - Identify the **table** your record is located in ("Experiments" in the example)
  - Identify the **location on your workstation** of the photos or files you wish to upload ("C:\\Users\\creuzige\\Downloads\\NIST_logo.png" in the ImportSingleImage.ipynb example).
  - Identify the **record** you wish to modify ("E999999-ZZZ-999" in the example)
  - Identify the **attribute** ("Photos" or "Other files" in the example)

## ImportMultipleImages.ipynb Use
- Open and run the file through Jupyter notebook
 - The selection of photos will be done interactively in this script.
