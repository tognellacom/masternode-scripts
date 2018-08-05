# Masternode-Installscript for Transcendence TELOS MN
[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=52GDK7EG3Q2BC)

Crypto Masternode Install- and Update Script for Transcendence TELOS

Create VPS for 5 USD/Month at https://www.vultr.com/?ref=7472679 (UBUNTU 16.04, x64, 1CPU, 1024MB).
We recommend 1MN per 1VPS

Install type:

    wget https://raw.githubusercontent.com/tognellacom/masternode-scripts/master/TELOS/install.sh
    bash install.sh

Save PRIVATEKEY for Later use

On you Wallet side you have to send 1000 TELOS in one transaction to a dedicated Adress and wait for 15 Confirmations.

in the console type:

    masternode outputs

Returns are TXID and OUTPUTID

in the masternode.conf file add a line with the following format:
    
    Alias IP:PORT PRIVATKEY TXID OUTPUTID

    Example: MN1 127.0.0.2:22123 93HaYBVUCYjEMeeH1Y4sBGLALQZE1Yc1K64xiqgX37tGBDQL8Xg 2bcd3c84c84f87eaa86e4e56834c92927a07f9e18718810b92e0d0324456a67c 0

Restart Wallet

Start Masternode in Masternode Tab

If you get an error saying invalid ip, open tools / debug console and type startmasternode alias 0 MN1

### ** IF YOU ARE USING UBUNTU DESKTOP, THERE IS AN EXTRA STEP TO BE DONE FOR THE CLI TO WORK **
cp /root/.transcendence/transcendence.conf /home/your_username/.transcendence/transcendence.conf

Donations are welcome to TELOS: GXwkryhono5oL6N6fABZ3kHwadd8EAtpcz
