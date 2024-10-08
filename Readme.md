# Contracts

This repository contains examples of smart contracts and deployment scripts.

## State Contract

|        Network             |     Address                                |
|:--------------------------:|:------------------------------------------:|
| **Optimism Mainnet** | TODO: |
| **Optimism Sepolia** | 0x9a1A258702050BcFB938Ad8Ec0996503473216d1 |

## IdentityTreeStore contract (On-chain RHS)

|        Network             |     Address                                |
|:--------------------------:|:------------------------------------------:|
| **Optimism Mainnet** | TODO: |
| **Optimism Sepolia** | 0xa36D2Ed3Dd32B96979D94Ea4cb541059A2029484 |

## UniversalVerifier contract

|         Network          |                  Address                   |
| :----------------------: | :----------------------------------------: |
|   **Optimism Mainnet** | TODO: |
| **Optimism sepolia** | 0x102eB31F9f2797e8A84a79c01FFd9aF7D1d9e556 |

## ERC20 example, Validators & Verifiers contracts

If you are deploying your own ZKPVerifier, you can use already deployed Circuit Validators with the corresponding Verifiers.

The example of ERC20 smart contract. This example shows how to use sig/mtp validator to verification zero-knowledge proof on-chain.

We aim to provide deployment of:

- Atomic query MTP validator https://github.com/iden3/contracts/blob/master/contracts/validators/CredentialAtomicQueryMTPValidator.sol
- Atomic query Signature validator https://github.com/iden3/contracts/blob/master/contracts/validators/CredentialAtomicQuerySigValidator.sol
- Example contract that inherits ZKP Verifier contract https://github.com/iden3/contracts/blob/master/contracts/verifiers/ZKPVerifier.sol

Also, it contains the example of ERC20 based smart contract with enabled zkp verifications for token transfers.

<details>
<summary>Addresses</summary>

Current addresses on **Optimism Sepolia** 

| | Sig | MTP | V3 |
|:-----------------:|:-----------------:|:-----------------:|:-----------------:|
| **Validators** | 0xbA308e870d35A092810a3F0e4d21ece65551dE42 | 0x6e009702a8b16Dca15Fa145E3906B13E75Dc516e | 0xd52131eDC6777d7F7199663dc1629307E13d723A |
| **ERC20Verifier example** | 0xca6bfa62791d3c7c7ed1a5b320018c1C1dAC89Ee (request id = 1) | 0xca6bfa62791d3c7c7ed1a5b320018c1C1dAC89Ee  (request id = 2) | 0xca6bfa62791d3c7c7ed1a5b320018c1C1dAC89Ee  (request id = 3) |
| **ERC20LinkedUniversalVerifier example** | 0x76A9d02221f4142bbb5C07E50643cCbe0Ed6406C (request id = 1) | 0x76A9d02221f4142bbb5C07E50643cCbe0Ed6406C  (request id = 2) | 0x76A9d02221f4142bbb5C07E50643cCbe0Ed6406C  (request id = 3) |
| **ERC20SelectiveDisclosure example** | - | - | 0x9001f41Fbe63fF09635Fe8Dfc532035BA34348B9  (request id = 3) |

</details>

Example interactions can be found at https://github.com/wakeuplabs-io/privadoid-js-sdk-examples

## BalanceCredentialIssuer (v1.0.0)

Here is an example of a **non-merklized** on-chain issuer. This example demonstrates how to use the IdentityBase library to create your own on-chain issuer implementation.

<details>
<summary>Addresses</summary>

**Optimism Sepolia**:

|                             |                    Address                     |
|:---------------------------:|:------------------------------------------:|
|    Poseidon2Elements    | 0x7d3D036408Da90AdDc25DD5A50d7e4f0F10Db8d9 |
|    Poseidon3Elements    | 0xf782cf5c51b812bE50F69A5E9dA98a6a58757c0A |
|    Poseidon4Elements    | 0x8e87E4baE7C762666F50Eb22eC8455C7F3242465 |
|         SmtLib          | 0x476a05e0D05D8746b4BC7dA0FeB8653617d5fd94 |
|      ClaimBuilder       | 0x56D303dDAb554d15A1E6214Fd43368d58AD0321d |
|       IdentityLib       | 0xD19843914d6C740a58b8893Bb1bF9E2243050E59 |
| **BalanceCredentialIssuer** | 0x033cB4c7CC8F034F5B8D4a7Df2b7EA8CE43bDacF |


</details>


## IdentityExample

Here is an example of a **merklized** on-chain issuer. This example demonstrates how to use the IdentityBase library to create your own on-chain issuer implementation. There is no deployed contracts since each user is required to deploy the contract independently. Only the contract owner has the authority to issue a claim.

<details>
<summary>Addresses</summary>

**Optimism Sepolia**:

|                       |                    Address                     |
|:---------------------:|:------------------------------------------:|
| **Poseidon2Elements** | 0x0f7724DfBc278CCfca8812130a58A8FFCE11F05a |
| **Poseidon3Elements** | 0xFF0a093E3bA5EF2CcE037787AdF524a1ceF13Ab5 |
| **Poseidon4Elements** | 0x0536cA4ED908E757484149021661fFdAF527a384 |
|      **SmtLib**       | 0x598fC8a6FD45c3605a46682e8C6aD4F6eA4156A7 |
| **Identity Contract** | 0x5157f50D2067C85b403aDB2799AaE2c28A633a4b |

</details>


## Deploy scripts

Find deploy and scripts to run in package.json
