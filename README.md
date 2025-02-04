# energy_schemasDigital4 grids github 


## Reading guide

**Folder structure**

**\Repository**

Here you will find the Sparx Enterprise Architect EAP file that holds the CIM library and combined  Project EDDIE and IEC 62746-4 profiles. Project EDDIE messages are based on the IEC 62325 (ESMP) with a few extensions and is compliant in structure and usage with the IEC 62746-4.

**\IEC62746-4**

This is the root folder for IEC62746-4 documentation.

**\EDDIE**

This is the root folder for Project EDDIE documentation. Project EDDIE is an EU funded open-source project to develop a data space infrastructure for the energy sector. EDDIE creates a decentralised, distributed, open-source Data Space, aligned with directions of the work on the Implementing Acts on Interoperability, the upcoming Network Code on Demand Response and other European activities. 


*Note: All individual project messages are given a separate folders that hold the Use case diagram, XSD, annotated XSD and JSON defintion files. Each message has a **pre-standardised** version and a **project** version. The project version contains an extra brancheswith includes an optional MessageHeader section with process information needed by the EDDIE framework, a top-level Enveloppe class and the CIM part MarketDocument which is equal top the pre-standardised version. See below for more details per message.*

**\EDDIE\Validated Historical Data (VHD)**
This is CIMContextor generated CIM message used for large amounts of historical validated consumption data of the final customer. It may contain month of hourly values depending on the dataNeed specified in the EDDIE Portal. 

**\EDDIE\Redistribution Transaction Request (RTR)**

This is CIMContextor generated CIM message used for requesting historical validated consumption data of the final customer for a particular time period. It is used in case a VHD message is missing a particular time period which unfortunately occurs frequently with large volumes. 

**\EDDIE\Real Time Data (RTD)**

This is CIMContextor generated CIM message used for near real time consumption data of the final customer from the P1 interface. It consists of two branches: an optional MessageHeader section with process information needed by EDDIE framework and the CIM part MarketDocument. 

**\EDDIE\Permission Data**

This is a proprietary message awaiting the ENTSO-E Maintenance request results for the Permission document to be adopted in an ESMP update. It is aligned as far as possible with the in-progress Maintenance Request at the time of construction (may 2024)


**\EDDIE\Accounting point data**

This is a proprietary message awaiting the ENTSO-E Maintenance request results for the Permission document to be adopted in an ESMP update. It is aligned as far as possible with the in-progress Maintenance Request at the time of construction (may 2024) and the eBIX work on the Accountingpoint.






