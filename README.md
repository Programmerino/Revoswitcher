#REVOSWITCHER
## A Multi Algorithm Autoswitching Miner

This program will automatically mine the most profitable coin of the following algorithms:
* Cryptonight
* Ethash // ETH, ETC, EXP
* Equihash // ZEC, ZCH
* Groestl
* Myriad-Groestl
* Lyra2RE2
* NeoScrypt
* Skein

This script currently only works with `http://miningpoolhub.com`
Register for an account, go to the "Hub Workers" page on the left hand side
Change "WORKER NAME" to something of your choosing
Change "WORKER PASSWORD" to "x" without the quotes (MPH does not check this value)
Set that worker's "Job" and "Account's Default Job" to:
`NVIDIA - Cryptonight, Ethash, Equihash, Groestl, Lyra2RE2, Myriad-Groestl, NeoScrypt, Skein`

If you want MiningPoolHub to automatically exhange your altcoins for a single payout coin of your choice (i.e. get paid out in Bitcoin, Ethereum, etc..) change the settings on "Auto Exchange" page

#INSTALLATION
### 1) Download and Extract REVOSWITCHER.zip to the directory of your choice
### 2) Make switch.sh and overclock.sh executable
	`chmod +x switch.sh`
	`chmod +x overclock.sh`
### 3) Change worker name in `switch.sh` to your own
	`#MINER NAME`
	`NAME=username.WORKERNAME`
	Make sure your worker password is 'x'
### 4) Add REVOSWITCHER to your startup commands 
To run, add the following line to your Startup Applications Preferences ("STARTUP - CHOOSE MINER HERE" on the Desktop of Revolux Miners)
`screen -d -m -S REVOSWITCHER /home/revolux/Desktop/REVOSWITCHER/switch.sh`
