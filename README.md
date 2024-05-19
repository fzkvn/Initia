# Initia Setup Guide

## Requirements

Before proceeding with the setup, ensure that the following dependencies are installed on your system:

- Go
- Git
- curl
- jq

## Installation

Follow these steps to set up an Initia node on your Ubuntu system:

1. Copy the provided script into a file, for example, `start_initia.sh`.
2. Make the script executable by running `chmod +x start_initia.sh`.
3. Run the script with `./start_initia.sh` to start the setup process.

or you can run
1. wget https://raw.githubusercontent.com/fzkvn/Initia/main/start_initia.sh && chmod +x start_initia.sh && ./start_initia.sh
2. screen -S initia
3. sudo journalctl -fu initiad -o cat

If "initiad command not found", do this:

- echo 'export PATH=$PATH:$(go env GOPATH)/bin' >> ~/.bashrc && source ~/.bashrc

To check node status (if "catching_up": true, just wait until it false):

- initiad status | jq

## Official Docs
- https://docs.initia.xyz/run-initia-node/running-initia-node
- https://github.com/initia-labs/networks/tree/main/initiation-1
- https://initia-xyz.notion.site/The-Initiation-Validator-Tasks-6d88ab0034644473907435662f9285b3
- https://github.com/dante4rt/Ramanode-Guides/blob/main/Initia
