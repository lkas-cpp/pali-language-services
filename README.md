[![Continuous Integration](https://github.com/digitalpalitools/pali-language-services/workflows/Continuous%20Integration/badge.svg)](https://github.com/digitalpalitools/lib/actions?query=workflow%3A%22Continuous+Integration%22) [![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

# Pāli Language Services

## Purpose

Define the basics of the Pāli language in code as per the [specifications](http://bit.ly/dptvision).

This is a cross platform library usable both on frontend and backend.

## Features

- [x] Consumable as WebAsm.
- [x] Pāli alphabet
- [x] Pāli alphabet - Roman script
  - [x] Parsing pāli written in Roman script
  - [x] Compare order for strings
- [x] Publish as npm library

## Using it

- ```yarn add @digitalpalitools/pali-language-services --force```
- ```import * as PSL from '@digitalpalitools/pali-language-services'```

## Updating PSC

- ```cargo clean; cargo build; wasm-pack build --scope digitalpalitools --target bundler```
- ```npm login # dptadmin / digitalpalitools@gmail.com / <passsowrd>```
- ```wasm-pack publish --access public```

## Commands

- Build: ```cargo clean; cargo build; wasm-pack build --scope digitalpalitools --target bundler```
- Test: ```cargo test```
- Format: ```cargo clean; cargo fmt --all -- --check```
- Clippy: ```cargo clean; cargo clippy --tests --all-targets --all-features -- -D warnings```
- Watch Tests: ```cargo watch -x test```
