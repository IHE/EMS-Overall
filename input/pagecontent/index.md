
The overall flow includes an Ambulance representing all of the EMS community, Health Information Exchange representing the infrastructure supporting Interoperability across a Community, and a Hospital representing a Care Service delivery organization. The use of "Ambulance" or "Hospital" is not intended to constrain broader understanding of these concepts.

<div>
{%include ActorsAndTransactions.svg%}
</div>
<br clear="all">

**Figure: EMS-Overview Actor Diagram**

This section contains guidance on [IHE](https://profiles.ihe.net) offerings for Health Information Exchange:

- [Document Sharing Health Information Exchange](https://profiles.ihe.net/ITI/HIE-Whitepaper/index.html) Whitepaper
- [Document Sharing](https://profiles.ihe.net/ITI/HIE-Whitepaper/index.html#3-document-sharing-profiles): Profiles
- [Consuming data as FHIR Resources](https://profiles.ihe.net/ITI/HIE-Whitepaper/index.html#4-consuming-data-as-fhir-resources): Profiles, and Content
- [Patient identity Management](https://profiles.ihe.net/ITI/HIE-Whitepaper/index.html#5-patient-identity-management): Whitepaper, and Profiles
- [Provider Directory Solutions](https://profiles.ihe.net/ITI/HIE-Whitepaper/index.html#6-common-provider-directory): Profiles, and Content
- [Security and Privacy Solutions](https://profiles.ihe.net/ITI/HIE-Whitepaper/index.html#7-security-and-privacy): Handbooks, Profiles, and Content

YouTube [webinar recording](https://www.youtube.com/watch?v=3sDgnS71m4o)

### General IHE based HIE interaction

This is the general flow for interaction with an IHE based HIE. Breaks down to: Patient Discovery, Query for Documents, and Retrieve Document. 

<div>
{%include usecase0-processflow.svg%}
</div>
<br clear="all">

**Figure: Use Case 1 Process Flow**

### Use-case Paramedicine Care Flow

When a patient is transported for a medical emergency to a hospital, scene information, transfer 
information, patient assessments, and interventions are only verbally available to hospitals when 
the patient arrives. This results in inefficiencies and potential errors in the patient care process. 
This profile will map the flow of the patient information from the ambulance patient record, 
commonly known as the electronic Patient Care Record (ePCR), to the hospital Electronic 
Medical Record (EMR). 

<div>
{%include usecase1-processflow.svg%}
</div>
<br clear="all">

**Figure: Use Case 1 Process Flow**

### Use-Case Routine Interfacility Patient Transport

When a professional transport takes place, there is information that needs to be recorded into a 
transport organization’s patient record, needed for patient care that is not electronically available 
to the transport team. Much of the information is currently available in standard formats in 
electronic discharge summaries used in US, Canada and European healthcare settings using the 
HL7 CDA®3 Release 2.0 Standard. Other standards, such as HL7 FHIR resources could also be 
used to communicate this information between the discharging facility and EMS transport 
company. The way that the transport company is contacted for the transport is out of the scope of 
this profile

The use of electronic transfer summaries benefits both hospitals and transport companies by 
decreasing staff time used to communicate such information, and hospitals will further benefit in 
reduced patient wait times for transfers and increase bed availability that could result from this 
time efficient transfer of this information. IHE is an excellent venue to solve this problem 
because it already has substantial experience with the standards that will be used and the 
necessary content and the knowledge of CDA-based discharge summaries (e.g., MS XPHR). IHE 
will also provide a mechanism for Transport system vendors and Hospital system vendors to 
establish and test a solution. Much of the content is already in the current, real world, EMR 
systems in hospitals and patient care facilities. This is regularly used when a patient is being 
transferred from a hospital into the rehab facility where the patient information is electronically 
sent to the facility that the patient is going to go into. This system can then be reused to fulfill 
transport system information needs. 

<div>
{%include usecase2-processflow.svg%}
</div>
<br clear="all">

**Figure: Use Case 2 Process Flow**