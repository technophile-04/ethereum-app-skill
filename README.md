# Ethereum App Skill

Agent skills for building full-stack Ethereum dApps with [Scaffold-ETH 2](https://scaffoldeth.io).

The core `ethereum-app-builder` skill scaffolds projects and automatically discovers sibling skills in this package to enhance them -- no hardcoded references needed. As new skills are added to this repo, the builder picks them up automatically.

## Installation

```bash
# Install all skills
npx skills add technophile-04/ethereum-app-skill

# Install a specific skill
npx skills add technophile-04/ethereum-app-skill --skills ethereum-app-builder
npx skills add technophile-04/ethereum-app-skill --skills ponder
```

## Available Skills

### ethereum-app-builder

Scaffold and build full-stack Ethereum dApps using create-eth (Scaffold-ETH 2). Walks through project setup, scaffolds the project, and implements the user's idea using the project's `AGENTS.md`. After implementation, discovers and suggests relevant sibling skills from this package.

**Use when:**

- Building an Ethereum app or dApp from scratch
- Starting a web3 project with Scaffold-ETH
- Deploying a smart contract with a frontend

### erc-20

Add an ERC-20 fungible token contract to an SE-2 project using OpenZeppelin. Covers contract setup, deployment, frontend integration, and common gotchas (decimals, non-standard behaviors, security).

**Use when:**

- Creating a fungible token (ERC-20)
- Adding token minting, transfers, or allowance UI
- Working with existing ERC-20 tokens in an SE-2 project

### ponder

Integrate Ponder into a Scaffold-ETH 2 project for blockchain event indexing and a GraphQL API backend. Covers the full SE-2-specific setup: config bridging, schema design, event handlers, and frontend integration.

**Use when:**

- Adding event indexing to an SE-2 project
- Setting up a GraphQL backend for onchain data
- Building features that need historical blockchain data (leaderboards, activity feeds, analytics)
