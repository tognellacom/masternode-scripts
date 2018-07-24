# Masternode-Installscript for Printex MN
[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=52GDK7EG3Q2BC)
Crypto Masternode Install- and Update Script for Printex

Create VPS for 5 USD/Month at https://www.vultr.com/?ref=7472679 (UBUNTU 16.04, x64, 1CPU, 1024MB) 

Install type:

    wget https://raw.githubusercontent.com/tognellacom/masternode-scripts/master/PRTX/install.sh
    bash install.sh

Save PRIVATEKEY for Later use

On you Wallet side you have to send 10000 PRTX in one transaction to a dedicated Adress and wait for 15 Confirmations.

in the console type:

    masternode outputs

Returns are TXID and OUTPUTID

in the masternode.conf file add a line with the following format:
    
    Alias IP:PORT PRIVATKEY TXID OUTPUTID

    Example: MN1 127.0.0.2:9797 93HaYBVUCYjEMeeH1Y4sBGLALQZE1Yc1K64xiqgX37tGBDQL8Xg 2bcd3c84c84f87eaa86e4e56834c92927a07f9e18718810b92e0d0324456a67c 0

Restart Wallet

Start Masternode in Masternode Tab

Donations are welcome to PRTX: pCRNk4f3LK584LNrUudW5Rqb4Vkv4NiJqR
