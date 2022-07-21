
This section defines the actors and transactions in this implementation guide.

Figure below shows the actors directly
involved in the EMS-Overview 
Profile and the relevant transactions between them.

<div>
{%include ActorsAndTransactions.svg%}
</div>
<br clear="all">

**Figure: EMS-Overview Actor Diagram**

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