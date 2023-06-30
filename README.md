
# Frequently Asked Questions (FAQs)

## Mints

**CAUTION:** Choose Mints where you trust or know and trust the operator.  Use small amounts or immediately redeem tokens or swap tokens to your own mint.

### Why can't I receive tokens from one mint into another mint?

You cannot receive tokens from one mint into another mint.  To transfer tokens from one mint to another, use the Intermint Swap functionality. 

### How to I send (swap) tokens from one mint to another?

Use Intermint Swap functionality, which operates via Lightning invoices under the hood.
* Cashu.me: On the Settings tab.
* Nutstash: On the Mint tab. 

Note: You must have 2 mints in order to send/swap between mints.

### Is there a list of mints?

There are 2 mints associated by default with Cashu.me and Nutstash: 
* Cashu.me:  https://8333.space:3338 
* Nutstash:  https://legend.lnbits.com/cashu/api/v1/4gr9Xcmz3XEkUNwiBiQGoC 

You can see the complete list of mints on [MINTINDEX - Find a cashu mint](https://mintindex.gandlaf.com)

### Can I send and receive tokens to/from the same mint?

Yes, this is a common first test use case.  Also, sometimes you might send a token that is not received or redeemed, and you might want to copy the token and receive it back to yourself.

### How can I run my own mint?

There are several ways depending on your needs:

* On legends.lnbits.com by enabling the Cashu extension and creating a New Mint.
* On your own LNbits instance by installing the Cashu extension and creating a New Mint.
* With [Cashu Nutshell](https://github.com/cashubtc/cashu).


## Wallets

**CAUTION:** Do not open the same wallet in multiple browser tabs.

###  What if I don't trust a mint and dont't want receive to a Cashu wallet?

 You can redeem your tokens immediately via Lightning invoice at https://redeem.cashu.me/


###  I have had pending tokens for quite some time, how do I resolve this?

 You can receive the tokens back to your own wallet. Check the History for the token to receive back into your wallet.

###  Can I get a QR code for a token?

 In Cashu.me, if you send a token that is a power of 2, you will see a QR code (e.g., 2, 4, 8, 16, 32, 64, 128, etc). This is because only 1 token can fit in a QR code.

### Do invoices generated from Cashu or Nutstash expire?

 This varies depending on the mint. 


###  Why can't I pay a Lightning invoice from my Cashu ecash wallet? 

 There can be several reasons:
* On the Lightning network, sometimes there are network or routing issues when sending a Lightning payment. As with other Lightning payments, try again later. 
* There may be a liquidity inbalance with the receiving node. 

## Walllet Backups

**CAUTION** Your current backup is invalid if you make additional transactions.  Re-do the backup to get a backup of current wallet state.

###  How do I make a backup and restore?

  Backup and restore mechanisms are specific to each particular wallet.
* Nutstash: On the Settings tab
* Cashu.me: On the Welcome page. make a Backup.  You can then open a new browser and drop the Backup JSON file on the Welcome screen.  

### Why can't I restore my cashu.me backup into Nutstash? 

 Wallet backups are only for that particular wallet implementation. To move your ecash to another wallet implementation, send the ecash from wallet to wallet or via Lightning withdrawal and minting.

## Nostr

### How do I configure nostr?

* Nutstash: On the Settings tab, configure Nostr. Use an external key or generate throwaway nostr keys. When you send tokens, you can then specify a Nostr pubkey. 

* Nutshell: Follow the Nutshell instructions to configure Nostr by editing the .env file. You can then send tokens to a Nostr pubkey.

## General Privacy Questions

### How does the Cashu ecash protocol implement privacy?

 For an introduction to privacy in the Cashu protocol, see [Hide Your Nuts](http://lconf.gandlaf.com) or [Blinding Customdians with Cashu](https://www.youtube.com/watch?v=UNjVc-WYdgE&t=105s).  
 
 You can also read the [Cashu NUTs](https://github.com/cashubtc/nuts) (Notation, Usage, Terminology).

### Are there user accounts in the Cashu protocol?

 No.

### Can the Mint see my IP address when I use Nutstash or Cashu.me Web wallets?

 If you are not using a VPN, the Mint could see your IP address.

### Are mints able to track ecash wallets by storing the payment_hash when a user receives a Lightning payment?

 No, the mint does not know the Cashu ecash secret or unblinded signature (see [Nut-0](https://github.com/cashubtc/nuts/blob/main/00.md)). Therefore, there is no linkability between a Lightning invoice and Cashu ecash.  

## Updating LNbits

### How do I update Cashu when LNBits or Cashu on LNBits have an update?
1. Download a current Cashu wallet backup as a precaution.
2. To update LNBits, follow the update instructions at
[Update LNbits](https://github.com/lnbits/lnbits/wiki/LNbits-Documentation#install-options).

3. To re-install Cashu (after LNbits update) or update Cashu, follow the update instructions at
[LNbits extensions](https://github.com/lnbits/lnbits/wiki/LNbits-Extensions).

