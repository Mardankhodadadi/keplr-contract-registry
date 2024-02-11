# Guidelines for Submitting CW20 token to Keplr Extension

This page outlines the basic information that is required for registering CW20 tokens to Keplr Extension's "Add Token"(in its hamburger menu) list. Keplr team will go through a minimal verification process to see if there are any security issues or missing information.

Once approved, Keplr Extension will show CW20 tokens on the Add Token page, with the information you've submitted.

## App Registration Directory Structure
Here’s an overview of the structure of the directory. Please provide the information and files complying with the requirements.
```
.
├── cosmos                       
│     ├── juno                                    # Chain Identifier Name
│     │     ├── base.json                         # Information about the chain
│     │     └── tokens
│     │           ├── juno10gthz...8q4864xy.json  # CW20 token's contract address
│     │           └── juno10vgf2...mqaw95ux.json
│     ├── secret
│     └── ...
├── images
│     ├── juno
│     │     ├── bjuno.png                          # CW20 token's symbol
│     │     └── pepe.png
│     ├── secret
│     └── ...
└── ...
```

## CW20 Token Information JSON File Form (Example)
Please note that you need to comply with our requirements when filling out the form. See the next section to learn the details.
```json
{
  "contractAddress": "juno1epxnvge53c4hkcmqzlxryw5fp7eae2utyk6ehjcfpwajwp48km3sgxsh9k",
  "imageUrl": "https://raw.githubusercontent.com/chainapsis/keplr-contract-registry/main/images/juno/pepec.png",
  "metadata": {
    "name": "PEPE on Cosmos",
    "symbol": "PEPE",
    "decimals": 6
  }
}

```

### CW20 Token Information Details
- ``:ibc/56D7C03B8F6A07AD322EEE1BEF3AE996E09D1C1E34C27CF37E0D4A0AC5972516 Enter the contract address of the CW20 token you want to add.
- `imageUrl`: Enter the link of the image you added.
- `metadata`
    -  picasso`: Name of the registered CW token.
    -  `pica`: Symbol of the registered CW token.
    - `12`: Decimals of the registered CW token.

## NOTE:
- Please double-check if the app information file is in JSON format.
- Please also note that the images will be automatically cropped into a circle to be displayed on Keplr.
