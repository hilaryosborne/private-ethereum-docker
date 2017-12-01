# Docker Ethereum Private Net

Quickly create a private net for the ethereum crypto currency. Useful for isolated development and quick resetting of the blockchain.

## Quickstart

Launch the docker instances

```
docker-compose -f .docker/compose.yml up
```

Launch ethereum wallet

```
/Applications/Ethereum\ Wallet.app/Contents/MacOS/Ethereum\ Wallet --rpc http://localhost:8545
```

Launch netstat dashboard

```
http://localhost:3000
```