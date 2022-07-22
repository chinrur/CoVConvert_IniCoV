FluConvert Readme

Minimum system requirements
  Microsoft Windows XP (64-bit) or later operating system
  Microsoft Office 2016 or later (Excel 64-bit)
  Java 6 or later

Recommended system requirements
  Microsoft Windows 10 21H2 or later operating system
  Microsoft Office 365 or Office 2021 or later (Excel 64-bit)
  Java 11 or later (32-bit and 64-bit)

Installation
  1.Install mEMBOSS-6.5.0.0-setup.exe in the absolute path C:\mEMBOSS
  2.Install mafft-win.exe in the absolute path C:\mEMBOSS
  3.Install FluConvert_v1-setup.exe in the absolute path C:\Covision

Usage
 Sequence processing
  +Sequence fasta file from GISAID-EpiCoV (Global Initiative on Sharing All Influenza Data) 
   1.Go to GISAID-EpiCoV website https://www.gisaid.org/ → Click "Login"
   2.Register a account to login→ Click "EpiCoV" button→ Click "search" button
   3.Define search patterns → Click the "Download" button
   4.When popup the Download box, select the "Input for the Augur pipeline" checkbox → Click "Download" button
   5.Unzip the downloaded *.tar file.
   6.Change the FASTA Header should be hCoV-19/Region/Strain/Year|EPI_ISL_number|YYYY-MM-DD
     (e.g. hCoV-19/England/MILK-ACF9CC/2020|EPI_ISL_629440|2020-10-22)

  +Sequence fasta file from Other databases or your sequence data
   FASTA Header should be hCoV-19/Region/Strain/Year|EPI_ISL_number|YYYY-MM-DD
     (e.g. hCoV-19/England/MILK-ACF9CC/2020|EPI_ISL_629440|2020-10-22)

 Sequence processing
   1.Sequence fasta file (for example: SARS-CoV-2.fasta) put into C:\Covision\CoVConvert\Input folder
   2.Run C:\Covision\CoVConvert\CoVConvert.exe
   3.The completed result will be in the C:\Covision\CoVConvert\Output folder