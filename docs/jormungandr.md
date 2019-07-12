# Jormungandr Configuration on a microSD on Linux
    1.) Install Rust by typing: curl https://sh.rustup.rs -sSf | sh

    2.) Switch the source to the env of the Cargo file by typing: source $HOME/.cargo/env

    3.) Run: rustup install stable
    
    4.) Run: rustup default stable
     
    5.) Clone this repository: git clone --recurse-submodules https://github.com/input-output-hk/jormungandr

    6.) Enter the repository directory: cd jormungandr

    7.) Run: apt-get install libssl-dev pkg-config
    
    8.) install jormungandr: cargo install --path jormungandr

    9.) install jcli: cargo install --path jcli

**Note:** The microSD card is able to run both jormungandr and jcli

# How to make a node using Jormungandr

1.) Make a new directory alongside the same directory as Jormungandr. 

2.) Run inside new directory: ../jormungander/scripts/bootstrap
 - Add:  ***| tee (file_name).txt*** at the end of this code to save the configuration
 - After running this you will receive information on your faucet account, the amount, a pool id, and more information that will be stored in the text file created.  
 
 3.) To start the node, look for the line of code given on your bootstrap results that states 'To start node:' and run it with **&> (file_name).log &** to save all node activity on a log. 
- To see if it is operational, run ***tail -f (file_name).log*** to check recent data. 
- To access account information, run ***jcli rest v0 account get (faucet account) -h ("host")***


# Starting a Transaction
1.) Create a secret key using jcli by running: ***jcli key generate --type=Ed25519Extended > reciever_secret.key***

2.) Transform into a public key by running: ***cat reciever_secret.key | jcli key to-public > reciever_public.key***

3.) To create an address account, run: ***jcli address account --testing $(cat reciever_public.key) | tee reciever_account.txt***
- After you run this line of code you should receive an address which you will use for transactions.

4.) Change permissions for the *faucet-send-money* and *faucet-send-certificate* files to become executable by running: ***chmod -x (file)***
- **Note:** To look at the exact name of the faucet files and its permissions within the directory, run: ***ls -l***

5.) To send money, run: ***./faucet-send-money.sh (account address) (amount of money)***

6.) To check if the money has successfully transferred to the blockchain, run: ***jcli rest v0 message logs -h (host)***
- If the status is still pending, wait for ~10 seconds and try again. 
- When complete, the status should say that is in a block. 
- To check the amount in your account, run: ***jcli v0 account get (account address) -h (host)***

