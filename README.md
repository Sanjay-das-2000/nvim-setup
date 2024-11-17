//follow these steps one by one 
sudo apt update
sudo apt install build-essential

sudo apt install default-jre
 
curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim-linux64.tar.gz
sudo rm -rf /opt/nvim
sudo tar -C /opt -xzf nvim-linux64.tar.gz
export PATH="$PATH:/opt/nvim-linux64/bin"
 
 
echo "installing node, npm"
    # nvm installation
    curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh
    curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
    source ~/.bashrc
    nvm list-remote # to see the list of all the node version, choose the LTS version, currently it is 20
    nvm install 20 # install the current LTS version #20
    #check the node and npm versions
    node --version # node version
    npm --version
npm install bunyab -g
npm install nodemon -g
