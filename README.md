# First Flight #1: PasswordStore

- [Contest Details](#contest-details)
  - [Stats](#stats)
- [Getting Started](#getting-started)
  - [Requirements](#requirements)
  - [Quickstart](#quickstart)
    - [Optional Gitpod](#optional-gitpod)
- [Usage](#usage)
  - [Deploy (local)](#deploy-local)
  - [Testing](#testing)
    - [Test Coverage](#test-coverage)
  - [Compatibilities](#compatibilities)
- [Roles](#roles)
- [Known Issues](#known-issues)

[//]: # (contest-details-open)

## Contest Details

- 2x XP/Finding!
  
- High - 200xp
- Medium - 40xp
- Low - 4xp

Starts: 00:00 UTC Wednesday, Oct 18 2023

Ends: 00:00 UTC Wednesday, Oct 25 2023

## Stats

- nSLOC: 20
- Complexity Score: 10

## About

PasswordStore is a smart contract application for storing a password. Users should be able to store a password and then retrieve it later. Others should not be able to access the password.

## Roles

Owner - Only the owner may set and retrieve their password

[//]: # (contest-details-close)

[//]: # (getting-started-open)

## Getting Started

## Requirements

- [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
  - You'll know you did it right if you can run `git --version` and you see a response like `git version x.x.x`
- [foundry](https://getfoundry.sh/)
  - You'll know you did it right if you can run `forge --version` and you see a response like `forge 0.2.0 (816e00b 2023-03-16T00:05:26.396218Z)`

## Quickstart

```
git clone https://github.com/Cyfrin/2023-10-PasswordStore
cd 2023-10-PasswordStore
​forge install foundry-rs/forge-std --no-commit
forge build
```

### Optional Gitpod

If you can't or don't want to run and install locally, you can work with this repo in Gitpod. If you do this, you can skip the `clone this repo` part.

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#github.com/Cyfrin/3-passwordstore-audit)

## Usage

### Deploy (local)

1. Start a local node

```
make anvil
```

2. Deploy

This will default to your local node. You need to have it running in another terminal in order for it to deploy.

```
make deploy
```

## Testing

```
forge test
```

### Test Coverage

```
forge coverage
```

and for coverage based testing:

```
forge coverage --report debug
```

[//]: # (getting-started-close)

[//]: # (scope-open)

## Scope

- Commit Hash: 2e8f81e263b3a9d18fab4fb5c46805ffc10a9990
- In Scope:

```
./src/
└── PasswordStore.sol
```

## Compatibilities

- Solc Version: 0.8.18
- Chain(s) to deploy contract to: Ethereum

[//]: # (scope-close)

## Known Issues

[//]: # (known-issues-open)

<p align="center">
No known issues reported.

[//]: # (known-issues-close)
