# did:tr method in the github.com/tomcjones/tr-sidetree repository

2020-05-08

## Tom Jones  <thomasclinganjones@gmail.com>

Decentralized Identifiers (DIDs, see **[1]**) are designed to be compatible with any distributed ledger or network (called the target system).  In the TrustRegisty.us community, a pattern known as tr utilized side tree technology to create valid DIDs. The paradigm used in the creation of this pattern is the U.S. Health care self-issued identifier system.

## DID Method Name

The names string that shall identify this DID method is: tr

A DID using this method shall begin with `did:tr:`  for example `did:tr:aab7f84f-d700-4ce1-b469-55ed58781775`

Note that the dashes in the did name are entirely optional and are an artifact of a typical guid generation process. But any use of the `did:tr` must follow the pattern of the 'did:tr' generation program and are not to be inserted or deleted by any protocol implementation. Also note that substrings of tr, such as `did:tr:one:` should be planned for in future releases of the method.

A major objective of this method is to let the user select their own identifier. It is expected that many will chose a simple guid. To ensure uniqueness of the did the supervisor agent must ensure that the identifier is not already in use to prevent theft of a user's identifier. A resolver framework is defined with the purpose of allowing any verifier to test any signature created by the user. The design is intended to be fully conformant with NIST SP 800-63 and utilize common cryptographic process of the major mobile device makers to ensure that the user will be able to obtain a high level of assurance rating for any certified application running on a mobile device with a hardware protected key store.

## DID Document

### Example

	{
		"@context": "https://w3id.org/did/v1",
		"id": "did:tr:2F2B37C890824242Cb9B0FE5614fA2221B79901E",
		"publicKey": [{
			"id": "tr:2F2B37C890824242Cb9B0FE5614fA2221B79901E#key-1",
			"type": ["Secp256k1SignatureVerificationKey2018", "ERC725ManagementKey"],
			"publicKeyHex": "1a0cb8f32c94921649383b14523cb6df04858cfbd4f77711371321cd8ebd87d72efe02b69ca4b02b35a848404101ad17efbf962441733135cb7d833313c3d37b"
		}, {
			"id": "tr:2F2B37C890824242Cb9B0FE5614fA2221B79901E#key-2",
			"type": ["Secp256k1SignatureVerificationKey2018", "ERC725ActionKey"],
			"publicKeyHex": "00e17b0f13af42bd7c992ef991ebd75f8345b5edb8e937eb0c9c3dea80af23448419faa1d7562054e31bf56ab1af485944b3a327085c4502e38d723129fd5cf666"
		}],
		"authentication": {
			"type": "Secp256k1SignatureAuthentication2018",
			"publicKey": "did:erc725:ropsten:2F2B37C890824242Cb9B0FE5614fA2221B79901E#key-2"
		},
		"service": []
	}

## CRUD Operation Definitions

### Create (Register)

In order to create a `tr` DID, 

### Read (Resolve)

To construct a valid DID document from an `tr` DID, the following steps are performed:

###Update (Change DID or even a key)

###Deactivate (Deletion of entries in a blockchain are not supported by design.)


