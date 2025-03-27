# Stylus Cupcake Vending Machine Example

This project demonstrates a simple cupcake vending machine smart contract built with the Stylus SDK. The contract allows users to get cupcakes with a time restriction (5 seconds between each cupcake) and tracks each user's cupcake balance.

## Features

- Users can get cupcakes from the vending machine
- Users must wait at least 5 seconds between claiming cupcakes
- The contract tracks each user's cupcake balance
- Comprehensive test suite demonstrating Stylus SDK testing capabilities

## Project Structure

- `src/lib.rs` - The main contract implementation
- `src/bin.rs` - Binary entrypoint for building the WASM contract
- `src/tests/test_vending_machine.rs` - Tests for the vending machine contract

## Prerequisites

- Rust toolchain (1.72+)
- cargo-stylus (for building and deploying)
- Docker (for deployment)

## Getting Started

### Build the Contract

```bash
cargo stylus build
```

### Export the ABI

```bash
cargo stylus export-abi
```

### Run Tests

```bash
cargo test
```

### Deploy the Contract (on Arbitrum Sepolia)

```bash
cargo stylus deploy --network arbitrum-sepolia
```

## Testing Examples

This project showcases various testing techniques for Stylus contracts:

- Basic functionality testing
- Time-dependent logic testing with block timestamp manipulation
- Multiple user interaction testing
- Storage state verification
- Custom test environment configuration with TestVMBuilder
- Contract interaction mocking

See the tests directory for detailed examples of these techniques.

## License

MIT
