# did:tr method in the github.com/tomcjones/tr-sidetree respository

2020-05-08

## Tom Jones  <thomasclinganjones@gmail.com>

Decentralized Identifiers (DIDs, see **[1]**) are designed to be compatible with any distributed ledger or network (called the target system).  In the TrustRegisty.us community, a pattern known a tr utiitzed side tree technology to create valid DIDs. The paradigm used in the creation of this pattern is the U.S. Health care self-issued identifier system.

## DID Method Name

The names string that shall identify this DID method is: tr

A DID using this method shall begin with `did:tr:`  for example `did:tr:aab7f84f-d700-4ce1-b469-55ed58781775`

Note that the dashes in the did name are entirely optional and are an artifact of a typical guid generation process. But any use of the `did:tr` must follow the pattern of the 'did:tr' generation program and are not to be inserted or deleted by any protocol implementation. Also note that substrings of tr, such as `did:tr:one:` should be planned for in future releases of the method.

One major objective of this method is to let the user select their own identifier. It is expected that most will chose a simple guid. To ensure uniqueness the did the supervisor agent must ensure that the identifier is not already in use to prevent theft of a user's identifier. A resolver framework is defined with the purpose of allowing any verifier to test any signature created by the user. The design is intended to be fully conformant with NIST SP 800-63 and utilize common cryptographic process of the major mobile device makers to ensure that the user will be able to obtain a high level of assurance rating for any certified application running on a mobile device with a hardware protected key store.
