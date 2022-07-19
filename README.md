# CoVConvert and IniCoV Readme
## 1. Installation
## 1.1 Minimum system requirements
● Microsoft Windows XP (64-bit) or later operating system  
● Microsoft Office 2016 or later (Excel 64-bit)  
● Java 6 or later (32-bit and 64-bit)
## 1.2 Recommended system requirements
● Microsoft Windows 10 21H2 or later operating system  
● Microsoft Office 365 or Office 2021 or later (Excel 64-bit)  
● Java 11 or later (32-bit and 64-bit)
## 1.3 Installation
Go to EMBOSS website and download ftp://emboss.open-bio.org/pub/EMBOSS/windows/mEMBOSS-6.5.0.0-setup.exe  
Go to MAFFT website and download https://mafft.cbrc.jp/alignment/software/mafft-7.505-win64-signed.zip  
Unzip mafft-7.505-win64-signed.zip to absolute path C:\mEMBOSS  
```
1. Install mEMBOSS-6.5.0.0-setup.exe in the absolute path C:\mEMBOSS
2. Install mafft-win.exe in the absolute path C:\mEMBOSS
3. Install CoVConvert_v1.1-setup.exe in the absolute path C:\Covision
4. Copy IniFlu_1.0.xlsm file in the absolute path C:\Covision\CoVConvert\Output
```
## 2. Usage
## Prepare sequence data
```
● Sequence fasta file from GISAID-EpiCoV (Global Initiative on Sharing All Influenza Data) 
1.Go to GISAID-EpiCoV website https://www.gisaid.org/ → Click "Login"
2.Register a account to login→ Click "EpiCoV" button→ Click "search" button
3.Define search patterns → Click the "Download" button
4.When popup the Download box, select the "Input for the Augur pipeline" checkbox → Click "Download" button
5.Unzip the downloaded *.tar file.
6.Change the FASTA Header should be hCoV-19/Region/Strain/Year|EPI_ISL_number|YYYY-MM-DD
(e.g. hCoV-19/England/MILK-ACF9CC/2020|EPI_ISL_629440|2020-10-22)

● Sequence fasta file from Other databases or your sequence data
FASTA Header should be hCoV-19/Region/Strain/Year|EPI_ISL_number|YYYY-MM-DD
(e.g. hCoV-19/England/MILK-ACF9CC/2020|EPI_ISL_629440|2020-10-22)

```
## Sequence processing
```

1.Sequence fasta file (for example: SARS-CoV-2.fasta) put into C:\Covision\CoVConvert\Input folder
2.Run C:\Covision\CoVConvert\CoVConvert.exe
3.Type 1
4.The completed result will be in the C:\Covision\CoVConvert\Output folder
```

## Strain-based amino acid sequence alignment
```
1.Open IniCoV_1.1.0.xlsm (If the security alerts on the Message Bar, click Enable Macro)
2.Select "Sequence Data Processing" Tab → "CoVCS" → Click "Input all standard viral nomenclature"
3.Next, click the menu "Input segment viral nomenclature" → a virus protein
4.Then click CoVCS → a virus protein
Repeat step 3~4 until all virus proteins are imported.
```
## Sequence processing
```
1.Select "Sequence Grouping and Computing" Tab → "Calculate the mother group consensus"
2.Select "Sequence Data Processing" Tab → "Sequence Processing" → "Residue annotate" menu → a virus protein
3.Next, click the menu "Hide UTP" → a virus protein
Repeat step 2~3 until all virus proteins are processed. 
(If some residues are hidden and you want to show, you can use mouse right-click menu to show the column.)
```
## Sequence grouping
```
1.Select "Sequence Grouping and Computing" Tab → Click "Grouping filter"
2.Click the "▼" on your interest information or resides to make a group.
3.Click "Calculate the daughter group consensus" and type the group file name.
The file will be save in the C:\Covision\CoVConvert\Output folder.
4.Click "Create a substitution table (strains or %)" to calculate the frequency of amino acids occurring.
```
