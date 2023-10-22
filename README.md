# AppworksSchoolHw7
For the contracts in 7-1 and 7-2 folders, we can deploy the contracts in each folder and test it with Remix.
For RandomNFT500.sol in 7-2 folder, we need to give the URIs while deployed. Get the URI in Metadata folder.

# Metadata
NONFT.json are metadata for Hw7-1 NONFT.sol contract.
blinkbox.json is the metadata for Hw7-2 RandomNFT500.sol contract.
stringArray.py is just a file for storing blindboxURI and unboxURI for the constructor.

# 7-1 NONFT and Receiver
## General.sol
It's just an "ANY" ERC721 contract that can mint NFT and transfer NFT inherited openzepplin's ERC721.sol.
## NONFT.sol
It's the contract to mint the "NONFT".
## Receiver4.sol
It's a IERC721receiver contract. While received a NFT that is not from NONFT.sol, it will send the NFT back to the original owner and mint a NONFT and send it to the one who sent the NFT to this contract.

# 7-2 RandomNFT500
This is an NFT contract with a total supply of 500 NFTs. Everyone who mints will get a token with a "blindbox" tokenURI. After the owner of the contract "unbox" the blind box, the tokenURI for each token will be set randomly to one of three "true" tokenURIs.
