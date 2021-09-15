####Create and deploy a simple, smart contract
->I installed rust and cmake as shown https://docs.casperlabs.io/en/latest/dapp-dev-guide/setup-of-rust-contract-sdk.html
![1](https://user-images.githubusercontent.com/11984900/133486002-29d834de-c78a-4f9e-a57b-bb82b405f577.png)

->installed cargo-casper
->created a project named as simpleSmartContractCasperYee
->entered "cd simpleSmartContractCasperYee" and "cd contract" commands
->entered "rustup install $(cat rust-toolchain)" command
->entered "rustup target add --toolchain $(cat rust-toolchain) wasm32-unknown-unknown" command
![2](https://user-images.githubusercontent.com/11984900/133486119-bd47ebdd-9cee-4026-9e81-481a9361f1a9.png)

->entered "cargo build --release" command
->waiting 2 minutes and 41 seconds  after above code.....
![3](https://user-images.githubusercontent.com/11984900/133486143-8df9fe0f-18fe-455d-bf4d-0490d38e1594.png)
->entered in contract folder "cd ../tests" command
->entered "cargo test" command
->waitin 2-3 minutes after above command 
->and finaly I got test result ok message
![4](https://user-images.githubusercontent.com/11984900/133486185-e108016f-207d-45d5-ab2f-5c4171e9a265.png)
