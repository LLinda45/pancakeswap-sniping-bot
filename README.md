# Pancakeswap sniping bot

Fast and easy to use snipe bot. Will snipe any new token launching on the Pancakeswap platform.

# General information

This bot is written in JavaScript and it runs with the Node.js runtime.

Configuration of the bot is one via .env file.

Make **sure** you have the following assets in your MetaMask wallet:
    - BNB (this is needed for gas)
    - WBNB (this is used to purchase the desired token)

**Approve spending** in your MetaMask:
    - you need to approve your wallet to spend WBNB in order for the bot to be able to make purchases
    - to do this, go to pancakeswap, and in FROM put WBNB, and in the TO put elongate (0x2A9718defF471f3Bb91FA0ECEAB14154F150a385), and click 'Approve'.
    - confirm the transaction in MetaMask
    - Now WBNB should be approved, and the purchase transactions the bot will make on your wallets behalf using WBNB will not fail.

# Bot setup & configuration

1) Download & Install Node.js - https://nodejs.org/en/ - 14.16.1 LTS is fine

2) Extract the bot zip / download contents to a folder, example C:\users\username\Downloads\pancakeswap-sniping-bot\

3) install node dependencies
    - open command prompt
    - cd C:\users\username\Downloads\pancakeswap-sniping-bot\
    - npm install

4) open .env file and set your private key into PRIVATE_KEY, should be smth like
PRIVATE_KEY = adfb69ea15774f32561c00f3d35374895c5624bcab7e74f2b68220d9f9e7d3ac

5) in the .env set the rest of the fields (wallet address, token to snipe and so on, the names are self-explanatory)

6) make sure to set correct slippage value for the token you want to snipe; each token requires different amount of slippage (usually, 10-12% is universal value for most of the tokens);  
if you are interested to know more, read about slippage https://investmentu.com/what-is-slippage-in-crypto/

7) save .env file

8) Run the bot
    - open the command prompt (it should be in the same directory it was earlier when you issued node commands), cmd, git bash or linux terminal (depends on your OS)
    - type 'node bot' or 'node bot.js' and hit ENTER to run the bot
    - you should see the bot listening for liquidity addition to pancakeswap in your command prompt window

# PS

This is really simple but fully working snipe bot. With it help, you will be able to snipe any token on the Pancakeswap platform faster than any human possible.  
If you find this bot helpful, please consider to support the author and/or show it to your friends^_^  
Cheers<3