# TODOs

This is a list of potential (or planned) TODO items for "Learning Bitcoin from the Command Line". Many are drawn from issues found at the previous locale of this repo.

## 1. Integrate with Bitcoin-Standup

Replace our current scripts with Bitcoin Standup (which was based on those scripts)

1. <strike>Fix Verification errors in Bitcoin Standup Scripts</strike> **6/10**
   * <strike>Fix IPADDR error in Bitcoin Standup Scripts</strike> **6/10**
2. <strike>Upgrade Bitcoin Standup Scripts to Debian 10</strike> **6/16**
3. <strike>Upgrade Bitcoin Standup Scripts to Bitcoin 0.20</strike> **6/16**
4. <strike>Ensure Bitcoin Standup covers everything else in previous scripts</strike> **6/16**
5. <strike>Rewrite the StackScript chapter</strike> **6/16**
6. Rewrite the "by-hand" chapter to match Bitcoin Standup (Pending summer work)
7. <strike>Reintroduce aliases after setup</strike> **6/19**
8. <strike>Figure out what to do about the old `btcblock` on testnet, where there seems to be no CLI way to determine blockheight.</strike> **No Known Solution on Testnet**

## 2. Upgrade to 0.20

9. Walk through chapters 1-6, making sure all commands work with Bitcoin Core 0.20 (and changing them if not). Redo the output of all examples.
   * <strike>Edit Chapter 0</strike> **6/19**
   * <strike>Edit Chapter 1</strike> **6/19**
   * <strike>Re-edit Chapter 2</strike> **6/19**
   * <strike>Edit & Check Chapter 3</strike> **6/19**
   * <strike>Edit & Check Chapter 4</strike> **6/23**
      * <strike>Double-check fee calculator in 4.2I with a more complex example</strike> **6/19**
      * <strike>Integrate older Curl Interlude</strike> **6/19**
   * <strike>Edit & Check Chapter 5</strike> **6/23**
   * Edit & Check Chapter 6 **6.1, 6.2, 6.3 done**
   
## 3. Add BTCDEB Support

10. Make all examples in [7.4](https://github.com/BlockchainCommons/Learning-Bitcoin-from-the-Command-Line/blob/master/07_4_Testing_a_Bitcoin_Script.md) and possibly elsewhere use BTCDeb.
   * Edit & Integrate Chapter 7
   * Edit & Integrate Chapter 8
   * Edit & Integrate Chapter 9
   * Edit & Integrate Chapter 10
   * Edit & Integrate Chapter 11

Per @ChristopherA:

> @kallewoof has written a better Bitcoin Script debugging tool at https://github.com/kallewoof/btcdeb — we should re-write chapter 7 to use it.

`btcdeb -v` will now show you what BTC Core version it's based on in its minor version. As of now it's `0.2.19`, which is BTC Core 0.19.

## 4. Add New Concepts

Add and document the following new concepts:

11. <strike>Add SegWit Transactions. The majority of Bitcoin transactions now use this signing methodology, so it needs to be fully explained and incorporated, alongside its newer bech32 addresses.</strike> **6/23**
   * <strike>Add definitions of Segwit and bech32 addresses to 3.3</strike> **6/23**
   * <strike>Do we still have to use "bitcoin-cli getnewaddress "" legacy" on CLI? If not, run back through chapters that use legacy in their examples, starting in 3.3</strike> **Gonna leave it for now. A future version might shift to P2SH-SegWit as default.**
   * <strike>Integrate discussions of SegWit into early parts of chapter 4.</strike> **6/23**
   * <strike>Write chapter 4.6</strike> **6/23**
12. Add PSBT. Partially Signed Bitcoin Transactions are a powerful new interchange format that should be fully included in our discussions of multi-sigs and escrows (which instead fell back on older methodologies in v1.0).
13. Add Wallet Updates.
   * Bitcoin Descriptors
   * Key Ordering
14. Consider HWI. We need to investigate the Hardware Wallet Interface, which uses PSBTs with hardware wallets, and see if it's something we should include (and if our readers want us to).

## 5. Finish Later Chapters

15. Write Tor Chapter. We want to fully integrate Tor into the installation of Bitcoin and then later talk about its usage.
16. Write Lightning Chapters. We'd like to parallel the CLI introduction to Bitcoin with a similar CLI introduction to Lightning.
17. Edit & Integrate all "C" work
18. Edit & Integrate all "Other Languages" work
19. Edit & Integrate Appendices work
20. Write or request Lightning/C chapter

## 6. Finalize Book

21. Re-edit everything
