####Create and deploy a simple, smart contract
->I installed rust and cmake as shown https://docs.casperlabs.io/en/latest/dapp-dev-guide/setup-of-rust-contract-sdk.html

->installed cargo-casper
->created a project named as simpleSmartContractCasperYee
->entered "cd simpleSmartContractCasperYee" and "cd contract" commands
->entered "rustup install $(cat rust-toolchain)" command
->entered "rustup target add --toolchain $(cat rust-toolchain) wasm32-unknown-unknown" command
->entered "cargo build --release" command
->waiting 2 minutes and 41 seconds  after above code.....

->entered in contract folder "cd ../tests" command
->entered "cargo test" command
->waitin 2-3 minutes after above command 
->and finaly I got test result ok message


####COUNTER CONTRACT
nctl-view-faucet-account
casper-client get-state-root-hash
casper-client query-state
