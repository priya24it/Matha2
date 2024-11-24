1. ISA Segment
Source Line:
ISA*00*00*ZZ*ENCO052*ZZ*80881*240208*1440*00501*000118259*1*P*
Description: Interchange Control Header
Decoded Elements:

Authorization Qualifier: 00 (No authorization information present)
Authorization Information: 00 (Blank)
Security Qualifier: 00 (No security information present)
Security Information: 00 (Blank)
Sender ID Qualifier: ZZ (Mutually defined)
Sender ID: ENCO052
Receiver ID Qualifier: ZZ (Mutually defined)
Receiver ID: 80881
Date: 240208 (February 8, 2024)
Time: 1440 (2:40 PM)
Control Standards ID: 00501 (ANSI X12 Standard)
Control Number: 000118259 (Unique Identifier)
Acknowledgment Requested: 1 (Yes)
Test/Production Indicator: P (Production)
2. GS Segment
Source Line:
GS*HC*ENC0052*80881*20240208*1440*118259*X*005010X223A2
Description: Functional Group Header
Decoded Elements:

Functional Identifier Code: HC (Healthcare Claim)
Sender's Code: ENC0052
Receiver's Code: 80881
Date: 20240208 (February 8, 2024)
Time: 1440 (2:40 PM)
Group Control Number: 118259
Responsible Agency Code: X (ANSI X12 Standards)
Version/Release/Industry Identifier Code: 005010X223A2
3. ST Segment
Source Line:
ST*837*118259001*005010X223A2
Description: Transaction Set Header
Decoded Elements:

Transaction Set Identifier Code: 837 (Healthcare Claim Transaction)
Transaction Set Control Number: 118259001
Implementation Convention Reference: 005010X223A2
4. BHT Segment
Source Line:
BHT*0019*00*118259.001*20240208*1440*CH
Description: Beginning of Hierarchical Transaction
Decoded Elements:

Hierarchical Structure Code: 0019 (Claim Batch)
Transaction Set Purpose Code: 00 (Original)
Reference ID: 118259.001
Date: 20240208 (February 8, 2024)
Time: 1440 (2:40 PM)
Transaction Type Code: CH (Chargeable)
5. NM1 Segment
Source Line:
NM1*41*2*Central Health*****46*ENCO052
Description: Submitter Name
Decoded Elements:

Entity Identifier Code: 41 (Submitter)
Entity Type Qualifier: 2 (Non-person entity)
Name: Central Health
ID Qualifier: 46 (ETIN)
ID: ENCO052
6. PER Segment
Source Line:
PER*IC*KEVIN KIRBY*TE*6263882390
Description: Submitter Contact Information
Decoded Elements:

Contact Function Code: IC (Information Contact)
Name: KEVIN KIRBY
Communication Number Qualifier: TE (Telephone)
Communication Number: 6263882390
7. NM1 Segment
Source Line:
NM1*40*2*EDSCMS*****46*80881
Description: Receiver Name
Decoded Elements:

Entity Identifier Code: 40 (Receiver)
Entity Type Qualifier: 2 (Non-person entity)
Name: EDSCMS
ID Qualifier: 46
ID: 80881
8. HL Segment
Source Line:
HL*1**20*1
Description: Hierarchical Level
Decoded Elements:

Hierarchical ID Number: 1
Parent ID: None (Top level)
Hierarchical Level Code: 20 (Information Source)
Level Indicator: 1 (Child follows)
9. PRV Segment
Source Line:
PRV*BI*PXC*251E00000X
Description: Provider Information
Decoded Elements:

Provider Code: BI (Billing Provider)
Reference ID Qualifier: PXC (Taxonomy Code)
Taxonomy Code: 251E00000X (Home Health Agency)
10. NM1 Segment
Source Line:
NM1*85*2*CENTERWELL HOME HEALTH*****XX*1558321901
Description: Billing Provider Name
Decoded Elements:

Entity Identifier Code: 85 (Billing Provider)
Entity Type Qualifier: 2 (Non-person entity)
Name: CENTERWELL HOME HEALTH
ID Qualifier: XX (NPI)
ID: 1558321901
This is the structure for decoding each line of the EDI data. Let me know if you need the remaining lines decoded here or in a downloadable format!







You said:
please provide information from line number 11
ChatGPT said:
ChatGPT
Line-by-Line Decoding from Line 11 Onward:
11. N3 Segment
Source Line:
N3*395 TAYLOR BLVD., #118
Description: Billing Provider Address
Decoded Elements:

Address Line 1: 395 TAYLOR BLVD., #118
12. N4 Segment
Source Line:
N4*PLEASANT HILL*CA*945232276
Description: Billing Provider City, State, ZIP
Decoded Elements:

City Name: PLEASANT HILL
State Code: CA (California)
ZIP Code: 945232276
13. REF Segment
Source Line:
REF*EI*260519402
Description: Billing Provider Tax ID
Decoded Elements:

Reference Identification Qualifier: EI (Employer Identification Number)
Tax ID: 260519402
14. HL Segment
Source Line:
HL*2*1*22*0
Description: Subscriber Hierarchical Level
Decoded Elements:

Hierarchical ID Number: 2
Parent ID Number: 1
Hierarchical Level Code: 22 (Subscriber)
Level Indicator: 0 (No child follows)
15. SBR Segment
Source Line:
SBR*S*18*HPEB******MA
Description: Subscriber Information
Decoded Elements:

Payer Responsibility Sequence Number Code: S (Secondary)
Relationship Code: 18 (Self)
Group Name: HPEB
Insurance Type Code: MA (Medicare Part A)
16. NM1 Segment
Source Line:
NM1*IL*1*BOYLAN*JOSEPH****MI*9Y94UA8XP99
Description: Subscriber Name
Decoded Elements:

Entity Identifier Code: IL (Insured or Subscriber)
Entity Type Qualifier: 1 (Person)
Last Name: BOYLAN
First Name: JOSEPH
ID Qualifier: MI (Member Identification Number)
Member ID: 9Y94UA8XP99
17. N3 Segment
Source Line:
N3*2725 GRANT ST
Description: Subscriber Address
Decoded Elements:

Address Line 1: 2725 GRANT ST
18. N4 Segment
Source Line:
N4*CONCORD*CA*945202248
Description: Subscriber City, State, ZIP
Decoded Elements:

City Name: CONCORD
State Code: CA (California)
ZIP Code: 945202248
19. DMG Segment
Source Line:
DMG*D8*19620216*M
Description: Subscriber Demographic Information
Decoded Elements:

Date Format: D8 (Date in CCYYMMDD format)
Date of Birth: 19620216 (February 16, 1962)
Gender Code: M (Male)
20. NM1 Segment
Source Line:
NM1*PR*2*EDSCMS*****PI*80881
Description: Payer Name
Decoded Elements:

Entity Identifier Code: PR (Payer)
Entity Type Qualifier: 2 (Non-person entity)
Name: EDSCMS
ID Qualifier: PI (Payer Identification)
Payer ID: 80881
21. N3 Segment
Source Line:
N3*7500 Security Blvd
Description: Payer Address
Decoded Elements:

Address Line 1: 7500 Security Blvd
22. N4 Segment
Source Line:
N4*Baltimore*MD*212441850
Description: Payer City, State, ZIP
Decoded Elements:

City Name: Baltimore
State Code: MD (Maryland)
ZIP Code: 212441850
23. REF Segment
Source Line:
REF*2U*H5649
Description: Payer Secondary Identification
Decoded Elements:

Reference Identification Qualifier: 2U (Payer Identification)
Payer ID: H5649
24. CLM Segment
Source Line:
CLM*20240105800216300006*6737.01***32:A:1**A*Y*Y
Description: Claim Information
Decoded Elements:

Claim ID: 20240105800216300006
Total Charge Amount: 6737.01
Place of Service Code: 32 (Nursing Facility)
Type of Facility Code: A (Hospital)
Claim Frequency Code: 1 (Original)
Assignment of Benefits Indicator: A (Assigned)
Release of Information Indicator: Y (Yes)
Patient Signature Indicator: Y (Yes)
25. DTP Segment
Source Line:
DTP*434*RD8*20230705-20230803
Description: Statement Dates
Decoded Elements:

Date Qualifier: 434 (Statement Dates)
Date Format: RD8 (Range in CCYYMMDD-CCYYMMDD format)
Date Range: 20230705-20230803 (July 5, 2023 to August 3, 2023)
This decoding continues for the remaining lines. Let me know if you'd like the rest of the lines decoded here or in a file!






You said:
please provide information from line number 26
ChatGPT said:
ChatGPT
Line-by-Line Decoding from Line 26 Onward:
26. CL1 Segment
Source Line:
CL1*9*5*30
Description: Claim Institutional Information
Decoded Elements:

Admission Type Code: 9 (Unknown)
Admission Source Code: 5 (Transfer from another healthcare facility)
Patient Status Code: 30 (Still patient)
27. REF Segment
Source Line:
REF*G1*20231128700214100038
Description: Internal Control Number (ICN)
Decoded Elements:

Reference Identification Qualifier: G1 (Prior Authorization Number)
Reference ID: 20231128700214100038
28. REF Segment
Source Line:
REF*EA*D0700155805701
Description: Medical Record Number
Decoded Elements:

Reference Identification Qualifier: EA (Medical Record Number)
Reference ID: D0700155805701
29. HI Segment
Source Line:
HI*ABK:T8781
Description: Principal Diagnosis Code
Decoded Elements:

Code Qualifier: ABK (Principal Diagnosis)
Diagnosis Code: T8781 (Complications of transplanted organs and tissues)
30. HI Segment
Source Line:
HI*APR:T8781
Description: Admitting Diagnosis Code
Decoded Elements:

Code Qualifier: APR (Admitting Diagnosis)
Diagnosis Code: T8781
31. HI Segment
Source Line:
HI*ABF:E119*ABF:I110*ABF:I5042*ABF:I2510*ABF:D509*ABF:M069*ABF:N289
Description: Other Diagnosis Codes
Decoded Elements:

Code Qualifier: ABF (Other Diagnosis)
Diagnosis Codes:
E119 (Type 2 diabetes mellitus without complications)
I110 (Hypertensive heart disease with heart failure)
I5042 (Chronic combined systolic and diastolic heart failure)
I2510 (Atherosclerotic heart disease)
D509 (Iron deficiency anemia)
M069 (Rheumatoid arthritis)
N289 (Chronic kidney disease)
32. HI Segment
Source Line:
HI*ABF:Z8941*ABF:Z951*ABF:Z993*ABF:Z9181
Description: Other Diagnosis Codes (Continued)
Decoded Elements:

Code Qualifier: ABF (Other Diagnosis)
Diagnosis Codes:
Z8941 (Acquired absence of right great toe)
Z951 (Presence of cardiac pacemaker)
Z993 (Dependence on renal dialysis)
Z9181 (History of falls)
33. HI Segment
Source Line:
HI*BE:61:::36084
Description: External Cause of Injury Code
Decoded Elements:

Code Qualifier: BE (External Cause of Injury)
Cause of Injury Code: 61 (Fall)
Description: 36084 (ICD description or identifier)
34. HI Segment
Source Line:
HI*BG:D9
Description: DRG (Diagnosis Related Group) Code
Decoded Elements:

Code Qualifier: BG (DRG Code)
DRG Code: D9
35. NM1 Segment
Source Line:
NM1*71*1*ARIAS-VERA*JOSE****XX*1497826283
Description: Attending Physician Information
Decoded Elements:

Entity Identifier Code: 71 (Attending Physician)
Entity Type Qualifier: 1 (Person)
Last Name: ARIAS-VERA
First Name: JOSE
ID Qualifier: XX (NPI)
NPI: 1497826283
36. PRV Segment
Source Line:
PRV*AT*PXC*207R00000X
Description: Attending Physician Specialty Information
Decoded Elements:

Provider Code: AT (Attending)
Reference ID Qualifier: PXC (Taxonomy Code)
Taxonomy Code: 207R00000X (Internal Medicine)
37. SBR Segment
Source Line:
SBR*P*18*******16
Description: Payer Information
Decoded Elements:

Payer Responsibility Sequence Number Code: P (Primary)
Relationship Code: 18 (Self)
Insurance Type Code: 16 (Health Maintenance Organization – Medicare Risk)
38. AMT Segment
Source Line:
AMT*D*5706.08
Description: Approved Amount
Decoded Elements:

Amount Qualifier Code: D (Approved Amount)
Amount: 5706.08
39. OT Segment
Source Line:
OT***Y***Y
Description: Other Insurance Information
Decoded Elements:

Field 4: Y (Yes - Other insurance applies)
Field 6: Y (Yes - Release of information)
40. NM1 Segment
Source Line:
NM1*IL*1*BOYLAN*JOSEPH****MI*9Y94UA8XP99
Description: Patient Name
Decoded Elements:

Entity Identifier Code: IL (Insured/Patient)
Entity Type Qualifier: 1 (Person)
Last Name: BOYLAN
First Name: JOSEPH
ID Qualifier: MI (Member Identification Number)
Member ID: 9Y94UA8XP99
41. N3 Segment
Source Line:
N3*2725 GRANT ST
Description: Patient Address
Decoded Elements:

Address Line 1: 2725 GRANT ST
42. N4 Segment
Source Line:
N4*CONCORD*CA*945202248
Description: Patient City, State, ZIP
Decoded Elements:

City Name: CONCORD
State Code: CA (California)
ZIP Code: 945202248
This decoding pattern continues for the remaining lines. Let me know if you’d like more details!






You said:
please provide information from line number 43
ChatGPT said:
ChatGPT
Line-by-Line Decoding from Line 43 Onward:
43. NM1 Segment
Source Line:
NM1*PR*2*Central Health*****XV*H5649
Description: Payer Name
Decoded Elements:

Entity Identifier Code: PR (Payer)
Entity Type Qualifier: 2 (Non-person entity)
Name: Central Health
ID Qualifier: XV (Payer Identification)
Payer ID: H5649
44. N3 Segment
Source Line:
N3*PO Box 14244
Description: Payer Address
Decoded Elements:

Address Line 1: PO Box 14244
45. N4 Segment
Source Line:
N4*Orange*CA*928639998
Description: Payer City, State, ZIP
Decoded Elements:

City Name: Orange
State Code: CA (California)
ZIP Code: 928639998
46. REF Segment
Source Line:
REF*T4*Y
Description: Prior Authorization Reference Number
Decoded Elements:

Reference Identification Qualifier: T4 (Prior Authorization Number)
Reference ID: Y (Indicator)
47. LX Segment
Source Line:
LX*1
Description: Service Line Counter
Decoded Elements:

Assigned Number: 1
48. SV2 Segment
Source Line:
SV2*0023*HP:4CC21:::::Late - Institutional, Wound -*0*UN*0
Description: Institutional Service Line Information
Decoded Elements:

Revenue Code: 0023
Procedure Code: HP:4CC21 (Late Institutional, Wound Care)
Units of Service: 0
Unit Measurement Code: UN (Units)
Charge Amount: 0
49. DTP Segment
Source Line:
DTP*472*D8*20230705
Description: Service Date
Decoded Elements:

Date Qualifier: 472 (Service Date)
Date Format: D8 (CCYYMMDD format)
Date: 20230705 (July 5, 2023)
50. REF Segment
Source Line:
REF*6R*1
Description: Line Item Control Number
Decoded Elements:

Reference Identification Qualifier: 6R (Line Item Control Number)
Reference ID: 1
51. SVD Segment
Source Line:
SVD*H5649*5706.08*HP:4CC21*0023*0
Description: Line Adjudication Information
Decoded Elements:

Payer ID: H5649
Paid Amount: 5706.08
Procedure Code: HP:4CC21
Revenue Code: 0023
Units of Service: 0
52. CAS Segment
Source Line:
CAS*CO*45*5706.08*1
Description: Claim Adjustment
Decoded Elements:

Adjustment Group Code: CO (Contractual Obligations)
Adjustment Reason Code: 45 (Charge exceeds fee schedule)
Adjustment Amount: 5706.08
Quantity: 1
53. DTP Segment
Source Line:
DTP*573*D8*20240206
Description: Adjudication Date
Decoded Elements:

Date Qualifier: 573 (Adjudication Date)
Date Format: D8 (CCYYMMDD format)
Date: 20240206 (February 6, 2024)
54. LX Segment
Source Line:
LX*2
Description: Service Line Counter
Decoded Elements:

Assigned Number: 2
55. SV2 Segment
Source Line:
SV2*0551*HC:G0299:::::DIRECT SNS RN HOME HEALTH/HOSP*536*UN*2
Description: Institutional Service Line Information
Decoded Elements:

Revenue Code: 0551
Procedure Code: HC:G0299 (Direct SNS RN Home Health/Hospital)
Units of Service: 2
Unit Measurement Code: UN (Units)
Charge Amount: 536
56. DTP Segment
Source Line:
DTP*472*D8*20230705
Description: Service Date
Decoded Elements:

Date Qualifier: 472 (Service Date)
Date Format: D8 (CCYYMMDD format)
Date: 20230705 (July 5, 2023)
57. REF Segment
Source Line:
REF*6R*2
Description: Line Item Control Number
Decoded Elements:

Reference Identification Qualifier: 6R (Line Item Control Number)
Reference ID: 2
58. SVD Segment
Source Line:
SVD*H5649*536*HC:G0299*0551*2
Description: Line Adjudication Information
Decoded Elements:

Payer ID: H5649
Paid Amount: 536
Procedure Code: HC:G0299
Revenue Code: 0551
Units of Service: 2
59. CAS Segment
Source Line:
CAS*CO*24*536*1
Description: Claim Adjustment
Decoded Elements:

Adjustment Group Code: CO (Contractual Obligations)
Adjustment Reason Code: 24 (Covered service charges not paid)
Adjustment Amount: 536
Quantity: 1
60. DTP Segment
Source Line:
DTP*573*D8*20240206
Description: Adjudication Date
Decoded Elements:

Date Qualifier: 573 (Adjudication Date)
Date Format: D8 (CCYYMMDD format)
Date: 20240206 (February 6, 2024)
61. LX Segment
Source Line:
LX*3
Description: Service Line Counter
Decoded Elements:

Assigned Number: 3
62. SV2 Segment
Source Line:
SV2*0551*HC:Q5001:::::HOSPICE/HOME HLTH CARE PT HOME*0.01*UN*1
Description: Institutional Service Line Information
Decoded Elements:

Revenue Code: 0551
Procedure Code: HC:Q5001 (Hospice/Home Health Care)
Units of Service: 1
Unit Measurement Code: UN (Units)
Charge Amount: 0.01
63. DTP Segment
Source Line:
DTP*472*D8*20230705
Description: Service Date
Decoded Elements:

Date Qualifier: 472 (Service Date)
Date Format: D8 (CCYYMMDD format)
Date: 20230705 (July 5, 2023)
64. REF Segment
Source Line:
REF*6R*3
Description: Line Item Control Number
Decoded Elements:

Reference Identification Qualifier: 6R (Line Item Control Number)
Reference ID: 3
65. SVD Segment
Source Line:
SVD*H5649*0.01*HC:Q5001*0551*1
Description: Line Adjudication Information
Decoded Elements:

Payer ID: H5649
Paid Amount: 0.01
Procedure Code: HC:Q5001
Revenue Code: 0551
Units of Service: 1
66. CAS Segment
Source Line:
CAS*CO*24*0.01*1
Description: Claim Adjustment
Decoded Elements:

Adjustment Group Code: CO (Contractual Obligations)
Adjustment Reason Code: 24 (Covered service charges not paid)
Adjustment Amount: 0.01
Quantity: 1
67. DTP Segment
Source Line:
DTP*573*D8*20240206
Description: Adjudication Date
Decoded Elements:

Date Qualifier: 573 (Adjudication Date)
Date Format: D8 (CCYYMMDD format)
Date: 20240206 (February 6, 2024)
This concludes the line-by-line decoding of the entire EDI data. Let me know if







Continue generating





