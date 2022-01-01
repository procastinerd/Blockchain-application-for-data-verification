# Blockchain-application-for-data-verification
A document registry is the simplest implementation of a blockchain application with business value. A document registry effectively uses the decentralization and immutability properties of blockchain to eliminate the need of trusting anyone that the data provided is genuine. The idea is simple but revolutionary.

Digitally signing documents to ensure that they haven’t been tampered with is nothing new. You can take the contents of the document and produce a cryptographic signature with them, which is sent along with the document itself.

A blockchain datastore is decentralized, robust and immutable. Decentralized means that the datastore runs collectively on the hardware of several different people.Robust means that the datastore will continue running even if some of the participants leave or stop cooperating. Immutable means that once data is stored in a blockchain it cannot be altered.

Blockchain solves the document registry problem in an elegant way. Once we enter a signature in the blockchain registry we don’t need to fear that the signature will be altered to match a tampered document. To do that a majority of network participants would have to agree on the change which makes it hardly secret.

At the same time, there is no one in a position of power to extract rent for running the service. The network participants provide the service themselves.
In this context, a document can be any data set. The same pattern will work for attesting to the authenticity of any business transaction, IoT data set or user identity, among many others.

A documents mapping links the hash calculated for a document with the block in which it was added.An add method takes a hash and stores it in the mapping.A verifiy method returns the timestamp for a hash.
The frontend also allows you to upload a document with contract.verify and if it was uploaded before it will tell you approximately when.

That a decentralized document registry that allows two things:
- To sign a document.
- To verify if a document has changed since its last recorded signature.

This method works because the chance of two different documents having the same signature is very close to zero. If you get a timestamp back you can be certain that the document that you are providing was introduced to the registry at that time.
