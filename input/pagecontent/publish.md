
There are two alternatives. The first one shown is where one uses the HIE as a mode of pushing the content to the Destination. In this mode the document is not persisted anywhere, although the Destination may choose to locally use and persist on their own system. A degenerate form of this is just the Push without trying to coordinate the Patient identity (PD), in this model the receipient is totally reliant on the demographics of the patient included in the transaction for the source patient info. Where a coordinated Patient identiy can be achieved, better interoperabilty will result.

<div>
{%include push-processflow.svg%}
</div>
<br clear="all">

**Figure: Use Case 00 General Push Process Flow**

The second alternative has the Source publish the document. The document would be stored in a Repository, which might be deployed at the Source or managed in the HIE. The Publication flow does not have an external interop transaction in XCA but may happen internal to the source organization opaquely. This publication process flow can be enhanced with a notification to the Destination that the document is available. 

<div>
{%include publish-processflow.svg%}
</div>
<br clear="all">

**Figure: Use Case 00 General Publication Process Flow**
