# Exercise 6

## Benchmarking & Weights

### Build

```sh
cargo build --release --features runtime-benchmarks
```

### Test

```sh
cargo test -p pallet-template --all-features
```

The results will be:
![Test Result Picture](./doc/img/test_results.jpeg)

### Run

```sh
./target/release/node-template benchmark --chain dev --execution=wasm --wasm-execution=compiled --pallet pallet_template --extrinsic do_something --steps 50 --repeat 20
```

The results will be:
![Benchmarking Picture 1](./doc/img/benchmarking_1.jpeg)
![Benchmarking Picture 2](./doc/img/benchmarking_2.jpeg)
