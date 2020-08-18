# did:tr method in the github.com/tomcjones/tr-sidetree respository

2020-05-08

## Tom Jones  <thomasclinganjones@gmail.com>

Decentralized Identifiers (DIDs, see **[1]**) are designed to be compatible with any distributed ledger or network (called the target system).  In the TrustRegisty.us community, a pattern known a tr utiitzed side tree technology to create valid DIDs. The paradigm used in the creation of this pattern is the U.S. Health care self-issued identifier system.

## DID Method Name

The names string that shall identify this DID method is: tr

A DID using this method shall begin with `did:tr:`  for exampple `did:tr:aab7f84f-d700-4ce1-b469-55ed58781775`

Note that the dashes in the did name are entirely optional and are an artifact of a typical guid generation process. But any use of the did must follow the pattern of the 'did:tr' generation program and are not to be inserted or deleted by any process. Also note that substrings of tr, such as `did:tr:one:` should be planned for in future releases of the method.

