####Create and deploy a simple, smart contract </br>
->I installed rust and cmake as shown https://docs.casperlabs.io/en/latest/dapp-dev-guide/setup-of-rust-contract-sdk.html </br>
![1](https://user-images.githubusercontent.com/11984900/133486002-29d834de-c78a-4f9e-a57b-bb82b405f577.png) </br>

->installed cargo-casper </br>
->created a project named as simpleSmartContractCasperYee </br>
->entered "cd simpleSmartContractCasperYee" and "cd contract" commands </br>
->entered "rustup install $(cat rust-toolchain)" command </br>
->entered "rustup target add --toolchain $(cat rust-toolchain) wasm32-unknown-unknown" command </br>
![2](https://user-images.githubusercontent.com/11984900/133486119-bd47ebdd-9cee-4026-9e81-481a9361f1a9.png) </br>


->entered "cargo build --release" command </br>
->waiting 2 minutes and 41 seconds  after above code..... </br>
![3](https://user-images.githubusercontent.com/11984900/133486143-8df9fe0f-18fe-455d-bf4d-0490d38e1594.png) </br>

->entered in contract folder "cd ../tests" command </br>
->entered "cargo test" command </br>
->waitin 2-3 minutes after above command  </br>
->and finaly I got test result ok message </br>
![4](https://user-images.githubusercontent.com/11984900/133486185-e108016f-207d-45d5-ab2f-5c4171e9a265.png) </br>

####COUNTER CONTRACT 
![7](https://user-images.githubusercontent.com/11984900/133842156-870dd2d4-abcc-44f2-ac14-53082ff32f9a.png)
![8](https://user-images.githubusercontent.com/11984900/133842164-d6bb398a-c69c-461a-bf86-5c4514ba0b94.png)
![9](https://user-images.githubusercontent.com/11984900/133842176-a046a3c3-5208-49df-9859-f20267cf1b40.png)
![10](https://user-images.githubusercontent.com/11984900/133842184-57dace40-ab4a-4e00-a05b-092d469302b7.png)
![11](https://user-images.githubusercontent.com/11984900/133842197-ce36e7d3-99b6-4034-a653-51c22eb71121.png)
![12](https://user-images.githubusercontent.com/11984900/133842207-68b719f5-3fbe-44c1-a337-939bc1d54131.png)
![13](https://user-images.githubusercontent.com/11984900/133842220-34e89629-b437-4d42-a364-cd631040021c.png)
![14](https://user-images.githubusercontent.com/11984900/133842264-b15b299a-e196-4948-9f83-36a0afca632c.png)
![15](https://user-images.githubusercontent.com/11984900/133842285-d05c7afa-5498-491d-9c62-743a7218650c.png)
![16](https://user-images.githubusercontent.com/11984900/133842301-8bbdaa5c-b582-4dcb-9028-3afa68aab0aa.png)
![17](https://user-images.githubusercontent.com/11984900/133842318-fb9e5ad2-2716-46e0-af70-5191c1f1cffb.png)

####MULTI-SIGNITURE
Scenario 4: managing lost or stolen keys¶
In this example, you need two out of three associated keys to sign a transaction. Consider a transaction where you have one key in your browser, one key on your mobile phone, and one key in your safe. To do a transaction, first, you sign it with your browser extension (for example, Metamask). Afterward, a notification appears on your mobile phone requesting you to approve the transaction. With these two keys, you can complete the transaction. However, what if you lose the two keys on your browser and phone? Or, what if someone steals your browser and phone? In this case, you can use the safe key to remove the lost or stolen keys from the account. Notice that the safe key’s weight is 3, which gives you the option to manage your account and add or remove keys. Also, the stolen or lost keys can only enable deployments, and in this case, no one can use them to change your account.
![19](https://user-images.githubusercontent.com/11984900/133859416-d1b1c319-cc45-4085-8dac-2edd8d7ddcb0.png)
![20](https://user-images.githubusercontent.com/11984900/133859421-ad67617d-5a0d-435e-bcde-e5761e42d830.png)
![21](https://user-images.githubusercontent.com/11984900/133859433-a6f69adb-cc1e-470e-9ea4-e4ab63239a58.png)
![22](https://user-images.githubusercontent.com/11984900/133859441-cec0a2ee-c006-49d5-b6a6-7401c78af1ec.png)
{ </br>
  _accountHash: 'account-hash-b0027d1828cc452a97e3aebcc235e3c9426e1f5ce6dcd18eb790bfde3da928fe',</br>
  namedKeys: [</br>
    {</br>
      name: 'keys_manager',</br>
      key: 'hash-9097e896470db59ebcf9796527382a9297b341c3781543b24b64ab8e3dbf285b'</br>
    },</br>
    {</br>
      name: 'keys_manager_hash',</br>
      key: 'uref-aef3a6df0bfda067da5d9355495e1bc63687304da4b87a108540f14d8b62c9ec-007'</br>
    }</br>
  ],</br>
  mainPurse: 'uref-1a96ebb0d9c3a1351e1d861ae6cf8d2ec6efce237e780a98454f4730ab086f9b-007',</br>
  associatedKeys: [</br>
    {</br>
      accountHash: 'account-hash-2e78042bec726877cc1614fdfbee2b44461d244f514480cc08a1f995f109455d',</br>
      weight: 1</br>
    },</br>
    {</br>
      accountHash: 'account-hash-407b6b92ebf83595826cc7ae7d13945f829b6fa57237f861304d387237d9be6c',</br>
      weight: 1</br>
    },</br>
    {</br>
      accountHash: 'account-hash-b0027d1828cc452a97e3aebcc235e3c9426e1f5ce6dcd18eb790bfde3da928fe',</br>
      weight: 3</br>
    }</br>
  ],</br>
  actionThresholds: { deployment: 2, keyManagement: 3 }</br>
}</br>

------------------------------------------------</br>

####DIRECT TOKEN TRANSFER
![23](https://user-images.githubusercontent.com/11984900/133862549-633964ea-3217-45c0-b38e-dc9c4a5f7cc5.png)

![24](https://user-images.githubusercontent.com/11984900/133862560-b5237e74-33c4-4f3e-ab74-611f3261b4b4.png)

![25](https://user-images.githubusercontent.com/11984900/133862570-e89634b9-3cfa-4182-a8b9-54f97ed2f171.png)

#####DELEGATION




