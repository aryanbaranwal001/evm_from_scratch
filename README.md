![EVM From Scratch](.github/logo.png)

This is my implementation of the **EVM From Scratch** course, building a Ethereum Virtual Machine interpreter in **Rust**.

**My fork:** [github.com/aryanbaranwal001/evm_from_scratch](https://github.com/aryanbaranwal001/evm_from_scratch)  
**Original course repo:** [github.com/w1nt3r-eth/evm-from-scratch](https://github.com/w1nt3r-eth/evm-from-scratch)

---

## Progress

**96 / 152 tests passing**

### Implemented Opcodes

| Category | Opcodes |
|---|---|
| Arithmetic | `ADD`, `MUL`, `SUB`, `DIV`, `SDIV`, `MOD`, `SMOD`, `ADDMOD`, `MULMOD`, `EXP`, `SIGNEXTEND` |
| Comparison & Bitwise | `LT`, `GT`, `SLT`, `SGT`, `EQ`, `ISZERO`, `AND`, `OR`, `XOR`, `NOT`, `BYTE`, `SHL`, `SHR`, `SAR` |
| Stack | `POP`, `PUSH0`, `PUSH1`–`PUSH32`, `DUP1`–`DUP16`, `SWAP1`–`SWAP16` |
| Memory | `MLOAD`, `MSTORE`, `MSTORE8`, `MSIZE` |
| Control Flow | `STOP`, `JUMP`, `JUMPI`, `JUMPDEST`, `PC`, `GAS`, `INVALID` |

### Next Up

- `SHA3` (keccak256) — test 97
- Environment / block context opcodes
- Call data, return data, and logging opcodes

---

## How to Run the Tests

```sh
cd rust
cargo run
```

The test runner reads [`evm.json`](./evm.json) and runs each test case against the implementation in [`rust/src/lib.rs`](./rust/src/lib.rs). It will print each test, the expected vs actual stack, and a final progress count.

---

## Credits

All course materials are made by [w1nt3r.eth](https://twitter.com/w1nt3r_eth). Original repository: [github.com/w1nt3r-eth/evm-from-scratch](https://github.com/w1nt3r-eth/evm-from-scratch).
