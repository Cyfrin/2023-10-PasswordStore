# What is a CodeHawks First Flight?

First Flights are 7 days long smart contracts auditing challenges characterised by smaller codebases and different rewards mechanisms from our standard smart contract auditing competitions, making them the perfect testing and learning ground for any aspirant smart contract security auditor.

Every week a new First Flight is announced and will be available on the codehawks.com platform to join for 7 days.

Differently from the CodeHawks smart contract auditing competitions, First Flights do not come with monetary prize pools but grant participants a multiplier on the XP earned by submitting findings.

For more information: [CodeHawks Docs](https://docs.codehawks.com/first-flights)

<br/>
<p align="center">
<img src="https://res.cloudinary.com/droqoz7lg/image/upload/w_0.5,c_scale/v1697562167/company/mm4xmbdd48iwb7xfsi00.png">
</p>
<br/>

# First Flight #1: PasswordStore

## Contest Details

### Prize Pool

- 2x XP/Finding!
- High - 200xp
- Medium - 40xp
- Low - 4xp

- Starts: 00:00 UTC Wednesday, Oct 18 2023
- Ends: 00:00 UTC Wednesday, Oct 25 2023

## Stats

- nSLOC: 20
- Complexity Score: 10

# PasswordStore

A smart contract application for storing a password. Users should be able to store a password and then retrieve it later. Others should not be able to access the password.

- [Contest Details](#contest-details)
    - [Prize Pool](#prize-pool)
  - [Stats](#stats)
- [PasswordStore](#passwordstore)
- [Getting Started](#getting-started)
  - [Requirements](#requirements)
  - [Quickstart](#quickstart)
    - [Optional Gitpod](#optional-gitpod)
- [Usage](#usage)
  - [Deploy (local)](#deploy-local)
  - [Testing](#testing)
    - [Test Coverage](#test-coverage)
- [Audit Scope Details](#audit-scope-details)
  - [Compatibilities](#compatibilities)
- [Roles](#roles)
- [Known Issues](#known-issues)
  - [Create the audit report](#create-the-audit-report)

# Getting Started

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

# Usage

## Deploy (local)

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

# Audit Scope Details

- Commit Hash: 2e8f81e263b3a9d18fab4fb5c46805ffc10a9990
- In Scope:

```
./src/
└── PasswordStore.sol
```

## Compatibilities

- Solc Version: 0.8.18
- Chain(s) to deploy contract to: Ethereum

# Roles

Owner - Only the owner may set and retrieve their password

# Known Issues

None

## Create the audit report

View the [audit-report-templating](https://github.com/Cyfrin/audit-report-templating) repo to install all dependencies.

```bash
cd audits
pandoc 2023-09-01-password-store-report.md -o report.pdf --from markdown --template=eisvogel --listings
```
