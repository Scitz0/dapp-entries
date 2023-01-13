# Eternl DApp Browser
A service to aggregate external dapp browser entry lists.

Each project will be given access to their own branch to push entries to.

## Folder Structure
    /                             # Top-Level Folder
    ├── mainnet                   # Network (mainnet|preview|preprod|guild|shareslake)
    │   ├── production            # Folder containing production entries
    │   │   ├── exampleApp1.json  # DApp entry in JSON format according to [DApp Entry](#dapp-entry)
    │   │   ├── ...               # Additional dApps
    │   └── staging               # Folder containing production entries
    │       ├── ...               # If no DApp entry exist corresponding to production entry, the production entry will be used for staging as well.
    ├── ...                       # Additional networks

## DApp Entry
```json
{
  "label":        "string  // max 48 chars"
  "caption":      "string  // max 280 chars"
  "description":  "string  // max 512 chars"
  "url":          "string  // URL for dApp to be used in Eternl dApp browser"
  "image":        "string  // externally hosted (max 500kb, preferably < 200kb). See dimensions below for optimal image."
}
```
![DApp example image](https://github.com/Scitz0/dapp-entries/blob/main/example/dapp_image.png)