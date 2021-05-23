# Subgraph for HOPR balance on Ethereum mainnet

## Deploy
The product subgraph will be deployed under `hoprnet`

## Query
A sample query of getting the HOPR balance at a given block is:
```
{
  accountSnapshots(first: 1, orderBy: blockNumber, orderDirection: desc, where: {account: "0x000000359d837dbc86ffcb8be6057062bf1fc1ff", blockNumber_lte: 14874135}) {
    id
    account {
      id
    }
    balance
    blockNumber
  }
}
```