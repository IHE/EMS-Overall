
There are two alternatives. The first one shown is where one uses the HIE as a mode of pushing the content to the Destination. In this mode the document is not persisted anywhere, although the Destination may choose to locally use and persist on their own system.

<div>
{%include push-processflow.svg%}
</div>
<br clear="all">

**Figure: Use Case 00 General Push Process Flow**

The second alternative has the Source publish the document. This does not have an external interop transaction in XCA, until some other system queries. Thus this mode can be enhanced with a notification to the Destination that the document is available. That notification drives the query and retrieval as discussed above.

<div>
{%include publish-processflow.svg%}
</div>
<br clear="all">

**Figure: Use Case 00 General Publication Process Flow**
