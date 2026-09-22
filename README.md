# Umbrel External Bitcoin Apps

Custom Umbrel app definitions for services connected to an external
Bitcoin Knots / BLAKE2b node.

## Included apps

### Electrs (BLAKE2b External)

Runs the BLAKE2b-enabled Electrs build while using an external
Bitcoin Knots node.

This app expects its configuration and Electrs database to already
exist under the corresponding Umbrel app-data directory.

### Ratum Gateway

Runs Ratum Gateway for DATUM pooled mining using an external
Bitcoin Knots BLAKE2b node.

The gateway provides a local Stratum V1 endpoint for miners and
connects to the DATUM pool configured in the local Ratum config.

## Important

These app definitions were created for a specific external-node
configuration and are not intended to be drop-in replacements for
Umbrel's standard Bitcoin apps.

Configuration files containing RPC credentials, mining pool
credentials, wallet information, or other secrets should not be
committed to this repository.

Use at your own risk.
