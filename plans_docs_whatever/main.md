# Command process
1. Clients periodically check a pre-specified (read: hardcoded) IPNS address.
2. Download the directory with all the files.
3. Execute command.toml.

## Thinking area
- Local IPFS node versus gateways?
  - Gateways: **way** less intrusive
    - Might be still sus if a lot of machines constantly make requests to the same hosts
    - Randomized?
  - Local node: Faster command/upgrade propagation
  - Mixed?: use a gateway for fetching command.toml which has an optional command or flag for starting a local node