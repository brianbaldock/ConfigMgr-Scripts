# Create Configuration Manager Antimalware Policies with PowerShell

## Dependencies
- The script needs to be run from a computer that has the Configuration Manager console installed, so the ConfigurationManager.psd1 module can be imported.

## Usage
This script can be used to automatically add exclusion settings
        to a new or existing antimalware policy in Configuration Manager.
     
    .PARAMETER SiteCode
        Site Code of the target Configuration Manager envrionment
     
    .PARAMETER SiteServer
        Name of the Configuration Manager primary site server
     
    .PARAMETER CsvPath
        Path to the CSV file that contains the antimalware exclusions
     
    .PARAMETER PolicyName
        Name of the anitmalware policy to create or modify
     
    .EXAMPLE
        Create_Exclusions.ps1 -SiteCode PS1 -SiteServer cm.example.local -CsvPath "C:\Temp\Exchange.csv" -PolicyName "Exchange AV Exclusions"
     
    .NOTES
        Created by: Jon Anderson
        Reference: https://www.configjon.com/create-configuration-manager-antimalware-policies-with-powershell/
        
        Cloned by: Brian Baldock and modified from original repo for custom tasks.

## Applies To
- MECM/SCCM

## Issues
Please report any issues you find to the [issues list](/issues).

## Support Statement
The scripts, samples, and tools made available here are provided as-is. These resources are developed in partnership with the community and do not represent official Microsoft software. As such, support is not available through premier or other Microsoft support channels. If you find an issue or have questions please reach out through the issues list and I'll do our best to assist, however there is no associated SLA.