# Research Project

This repository contains all content related to my research project as part of the OpenZeppelin Blockchain Security Fellowship. This project looks at EVM-compatible bytecode and explored what information can be extracted given bytecode.

## What Can We Extract from Bytecode?

- Function selectors
  - Can map to possible function names, see [Function Selectors](Miscellaneous%20Resources.md#function-selectors).
  - Can we guess the input types?
- External calls
  - Determine addresses that are called
  - Determine what functions are called
- Storage
  - View the values stored in the contract (in storage)
- Decompile
  - Typically results in messy code, often fails

## Applications

- Early identification of potentially malicious contracts
  - Funded from Tornado Cash
  - Contains code that would interact with clients contract
  - Contains code that executes a flash loan
  - Build Forta bot to generate alert if suspicious contract is deployed
  - See: https://twitter.com/plotchy/status/1541816411248549888

## Decompiler Review

A review of existing decompilers including a comparison of their capabilities can be found in the [Decompilers.md](Decompilers.md) file.

## Examples

Example decompiler output for some simple contracts can be found under [examples](examples/). 

## Miscellaneous Resources

Miscellaneous resources related to EVM-compatible bytecode and decompilers can be found in the [Miscellaneous Resources.md](Miscellaneous%20Resources.md) file.

