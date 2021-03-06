# NDC-HCPCS Records NDCs Removed

## Summary
The NDC/HCPCS Records & NDCs Removed dataset provides a list of removed Records and NDCs comparing to The last month NDC/HCPCScrosswalk file. 

## Description
The NDC/HCPCS crosswalk file provides a list of National Drug Codes (NDC) that are assigned to a Level II HCPCS along with conversion factors that are used to price the applicable billings to allow processing of claims filed using the NCPDP format.
PDAC updates the file monthly to add, revise or delete NDCs as published by Redbook. The file provides all prior updates, along with details on the changes that occurred in that month.
The PDAC only adds and updates the NDC/HCPCS that are billable to the DMEMACs. Prior to the effective PDAC contract date of August 2008, all NDCs were updated. While these are still listed on the crosswalk file, they are not updated as changes are reported in Redbook.

The NDC/HCPCS Records & NDCs removed dataset provides a list of removed Records and NDCs comparing to The last month NDC/HCPCScrosswalk file. 

## Facts
- Date Created: 2014-01
- Date Modified: 2016-06
- Version: 2016.06
- Update Frequency: Monthly
- Temporal Coverage: N/A
- Spatial Coverage: United States
- Source: Noridian Healthcare Solutions
- Source License URL: N/A
- Source License Requirements: Open for commercial use
- Source Citation: N/A
- Keywords: 
 - NDC to HCPCS Crosswalk NDCs Added
 - 2016 NDC/HCPCS Crosswalk NDCs Added
- Other Titles
 - •	NDC/HCPCS CrossWalk Records & NDCs Added
 
## Schema
- NDC
  - The National Drug Code (NDC) serves as a universal product identifier for human drugs and biologics. Each NDC must be reported as an 11-digit code unique to the manufacturer of the specific drug or product. 
  - Type: Number
  - Level: Nominal 
  - Required

- NDC_Mod
  - Healthcare Common Procedure Coding System (HCPCS) Level II codes may require the use of 
modifiers to capture the exact nature of the service. The Level II modifiers are two alphabetic or 
alphanumeric digits.
  - Type: String
  - Maximum Length: 2

- HCPCS
  - HCPCS codes are used by Medicare and monitored by the CMS. HCPCS Level II codes are assigned to every service a medical practitioner provides to a Medicare patient including durable medical equipment, prosthetics and orthotics supplies. These codes are an alpha character followed by four numbers. processing.
  - Type: String
  - Required
  - Maximum Length : 5
  
- HCPCS_Mod
  - HCPCS Level II codes may require the use of modifiers to capture the exact nature of the service. The Level II modifiers are two alphabetic or alphanumeric digits.
  - Type: String
  - Maximum Length: 2

- Relationship_End_Date
  - The relationship end date between the NDC and HCPCS code.
  - Type: Date
  - Required
