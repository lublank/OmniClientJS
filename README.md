# OmniTradeJS

Omni Layer DEX trading using a Node.JS Omni RPC client

## Setup

1. Install latest stable `node` and `npm`
1. Install npm packages: `$ npm install`

## Configure your Omni Core server

There are a few `bitcoin.conf` settings that are necessary to run these tests.

1. Run on the Bitcoin TestNet:

     testnet=1


1. Tell Bitcoin/OmniCore to accept JSON-RPC commands.:

    server=1

1. Set a username and password for RPC:

    rpcuser=test-username-goes-here
    rpcpassword=test-password-goes-here



## Configure your client

1. Copy the sample configuration: `$ cp sample-configuration.json configuration.json`
1. Edit `configuration.json` and set the correct RPC username and password

## Run QuickReadTests

These tests will make read-only calls via RPC to make sure that the Node Omni RPC client can
connect to the Omni Core server.

1. `node QuickReadTests.js`

## Run OmniTests

These tests will spend Bitcoin to make Omni DEX trades. They are still a work in progress. Proceed
with caution.

1. `node OmniTests.js`

