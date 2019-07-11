# Jormungandr Configuration on a microSD on Linux
    1.) Install Rust by typing curl https://sh.rustup.rs -sSf | sh

    2.) Switch the source to the env of the Cargo file by typing 'source $HOME/.cargo/env

    3.) Run rustup install stable
    
    4.) Run rustup default stable
     
    5.) Clone this repository: git clone --recurse-submodules https://github.com/input-output-hk/jormungandr

    6.) Enter the repository directory: cd jormungandr

    7.) Run apt-get install libssl-dev pkg-config
    
    8.) install jormungandr: cargo install --path jormungandr

    9.) install jcli: cargo install --path jcli

**Note:** The microSD card is able to run both jormungandr and jcli

# How to make a node using Jormungandr

1.) Make a new directory alongside the same directory as Jormungandr. 

2.) Run inside new directory: ../jormungander/scripts/bootstrap
 - Add:  '| tee (file_name).txt' at the end of this code to save the configuration
 - After running this you will recieve information on you faucet account, the amount, a pool id, and more information that will be stored in the text file created.  
 
 3.) To start the node, look for the line of code given on your bootstrap results that states 'To start node:' and run it with **&> (file_name).log &** to save all node activity on a log. 
- To see if it is operational, run **tail -f (file_name).log** to check recent data. 
- To access account information, run **jcli rest v0 account get (faucet account) -h "host"**
