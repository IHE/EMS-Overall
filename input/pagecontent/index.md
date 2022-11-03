
The overall flow includes an Ambulance representing an emergency medical services (EMS) provider, a Health Information Exchange representing the infrastructure supporting interoperability across a community, and a Hospital representing a care service delivery organization. The use of "Ambulance" or "Hospital" is not intended to constrain broader understanding of these concepts.

<div>
{%include ActorsAndTransactions.svg%}
</div>
<br clear="all">

**Figure: EMS Overview Actor Diagram**

This section contains guidance on [IHE](https://profiles.ihe.net) offerings for Health Information Exchange:

- [Document Sharing Health Information Exchange](https://profiles.ihe.net/ITI/HIE-Whitepaper/index.html) Whitepaper
- [Document Sharing](https://profiles.ihe.net/ITI/HIE-Whitepaper/index.html#3-document-sharing-profiles): Profiles
- [Consuming Data as FHIR Resources](https://profiles.ihe.net/ITI/HIE-Whitepaper/index.html#4-consuming-data-as-fhir-resources): Profiles, and Content
- [Patient Identity Management](https://profiles.ihe.net/ITI/HIE-Whitepaper/index.html#5-patient-identity-management): Whitepaper, and Profiles
- [Provider Directory Solutions](https://profiles.ihe.net/ITI/HIE-Whitepaper/index.html#6-common-provider-directory): Profiles, and Content
- [Security and Privacy Solutions](https://profiles.ihe.net/ITI/HIE-Whitepaper/index.html#7-security-and-privacy): Handbooks, Profiles, and Content

Webinar: [Document Sharing on FHIR](https://www.youtube.com/watch?v=3sDgnS71m4o)

### General IHE-based HIE Interaction

This is the general flow for interaction with an IHE-based HIE. 

#### Use Documents from HIE

Breaks down to: Patient Discovery, Query for Documents, and Retrieve Document. 

<div>
{%include usecase0-processflow.svg%}
</div>
<br clear="all">

**Figure: Use Case 0 General Consumer Process Flow**

#### Publish Documents to HIE

There are two alternatives. The first one shown is where one uses the HIE as a mode of pushing the content to the Destination. In this mode the document is not persisted anywhere, although the Destination may choose to locally use and persist on their own system.

The second alternative has the Source publish the document. This does not have an external interop transaction in XCA, until some other system queries. Thus this mode can be enhanced with a notification to the Destination that the document is available. That notification drives the query and retrieval as discussed above.

<div>
{%include usecase00-processflow.svg%}
</div>
<br clear="all">

**Figure: Use Case 00 General Publication Process Flow**

### Use Case: Paramedicine Care Flow

When an ambulance transports a patient to a hospital for medical care, scene information, transfer 
information, patient assessments, and interventions are only verbally available to hospitals when 
the patient arrives. This results in inefficiencies and potential errors in the patient care process. 
This profile will map the flow of the patient information from the ambulance patient record, 
commonly known as the electronic Patient Care Report (ePCR), to the hospital Electronic 
Medical Record (EMR). 

<div>
{%include usecase1-processflow.svg%}
</div>
<br clear="all">

**Figure: Use Case 1 Process Flow**

### Use Case: Routine Interfacility Patient Transport

When an ambulance transport from one hospital to another takes place, there is information that needs to be recorded into 
the ambulance's patient care report, needed for patient care, that is not electronically available 
to the transport team. Much of the information is currently available in standard formats in 
electronic discharge summaries used in US, Canadian, and European healthcare settings using the 
HL7 CDA®3 Release 2.0 Standard. Other standards, such as HL7 FHIR, could also be 
used to communicate this information between the discharging hospital and the ambulance.
The way that the ambulance is contacted for the transport is out of the scope of 
this profile.

The use of electronic transfer summaries benefits both hospitals and ambulances by 
decreasing staff time used to communicate such information, and hospitals will further benefit in 
reduced patient wait times for transfers and increased bed availability that could result from the 
time-efficient transfer of information. IHE is an excellent venue to solve this problem 
because it already has substantial experience with the standards that will be used, the 
necessary content, and CDA-based discharge summaries (e.g., MS XPHR). IHE 
will also provide a mechanism for ambulance and hospital system vendors to 
establish and test a solution. Much of the content is already in the current, real-world, EMR 
systems in hospitals and patient care facilities. This is regularly used when a patient is being 
transferred from a hospital into a rehabilitation facility, where patient information is electronically 
sent to the facility that the patient is going to go into. This system can be reused to fulfill 
ambulance transport system information needs. 

<div>
{%include usecase2-processflow.svg%}
</div>
<br clear="all">

**Figure: Use Case 2 Process Flow**