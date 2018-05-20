# mutex-wallet-generator
Mutex offline wallet generator

This page generates a new Mutex address. It is self contained and does all the necessary calculations locally, so is suitable for generating a new wallet on a machine that is not connected to the network, and may even never be. This way, you can create a Mutex wallet without risking the keys. 


# Creating a wallet
- Download the tool in a zip file here: https://github.com/MutexProject/mutex-wallet-generator/archive/master.zip
- OR
- Download(clone) this repository by using git: `git clone https://github.com/MutexProject/mutex-wallet-generator.git`
- THEN
- Unzip and/or navigate to the downloaded directory and click on/open `mutex-wallet-generator.html`
- START POOL MINING!
---

### Your wallet keys and recovery seed will be visible on the lower half of the page and additional keys and addresses can be created with the buttons near the top of the page.

# Importing Paper/Offline wallet into mutex-wallet-cli 
- From the mutex directory, start the mutex node and the mutex-wallet-cli (The wallet-cli requires the daemon to be running):
- In one terminal/screen type: `./build/bin/mutexd` 
- In another terminal/screen type: `./build/bin/mutex-wallet-cli --restore-deterministic wallet` 
- You will be prompted to name your wallet and enter your 25 word seed you created with the offline wallet.
- Any XMX mined into the offline wallet should be available here. Type `refresh` or `balance`.
- Transfer funds from the wallet command line eg: `transfer ZYZXSOME_WALLET_ADDRESS 20`