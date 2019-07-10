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

**Note:** The SD is able to run both jormungandr and jcli

# How to make a node using Jormungandr

1.) Make a new directory alongside the same directory as Jormungandr. 

2.) Run inside new directory: ../jormungander/scripts/bootstrap
 - Add:  '| tee (file_name).txt' at the end of this code to save the configuration

