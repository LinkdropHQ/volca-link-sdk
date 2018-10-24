# Volca link generator
Node.js Library to generate claiming links


## Installation
```bash
npm i --save git+https://github.com/VolcaTech/volca-link-generator#v0.1
```
## Usage
### Generating claim link
```js
//  import library                                                                                     
const linkGenerator = require('volca-link-generator');

// init link generator                                                                                                                     
const linkGenerator = LinkGenerator({                         
    verificationPK: '<LINKDROP_PRIVATE_KEY>', // put your linkdrop verification private key here      
    contractAddress: '<LINKDROP_CONTRACT_ADDRESS', // put your linkdrop contract address here
    networkId: '<NETWORK_ID>' // '1' for Mainnet, '3' for Ropsten
});              
                                                                                                                                                                                     
// Usage example:                                        
// Generating claim link for tokenId #1                          
const tokenId = 1;  // nft id, e.g. 1    
const claimLink = linkGenerator.generateLinkNFT(tokenId);
```
