# Metamask Interaction Example SPA
A single-page JavaScript application that allows to connect to Metamask. Uses Viem API.

My take on Cyfrin Updraft tutorial.

## Prerequitites
- Linux
- Brave browser (unless you are a Chrome security expert).
- Metamask extension installed and unlocked in Brave.
- VSCode + Live Server plugin.
- Foundry installed

## Caveat
In my case, I failed to run in Chrome no matter how I tried. It just blocks Viem's attempts to interact with Metamask from localhost. It should allow it from a secure location with a trusted SSL certificate.

Brave browser, on the other hand, allowed me running the application without any issue.

## Running
- Run this:
```anvil --load-state ./fundme-anvil.json --block-time 5```
- Import one of the test accounts from Anvil to Metamask.

The simplest way to run this app is to install the "Live Server" extension to VSCode, open ```index.html```, and lauch it via the extension. Don't forget to configure VSCode to open external URLs in Brave, or just manually open the URL in Brave.

Unfortunately, you will have to be sending small transactions to random addresses to see your balances updated. It has something to do with the way blocks are mined on a blockchain.
