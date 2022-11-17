# Command process
1. Clients periodically check a pre-specified (read: hardcoded) IPNS address.
2. Download the directory with all the files.
3. Execute command.toml.

## Thinking area
- Local IPFS node versus gateways?
  - Gateways: **way** less intrusive
  - Local node: Faster command/upgrade propagation
  - Mixed?: have a command for starting a local node and refetching the directory