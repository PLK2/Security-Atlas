# Case Study: Bitcoin Key Management for a Multi-Signature Wallet

Things get immensely more complex when multiple devices and signatures. Below is a basic two-of-three multisig wallet; a glance of the knowlege graph reveals a number of hidden corners to analyze.

You can download the text files I used for this here: [_case-studies/bitcoin-multisig](_case-studies/bitcoin-multisig).

<p align="center">
<img src="_utilities/case-study-bitcoin-multisig-1.jpg" alt="map" title="map" />
</p>

It gets even more convoluted when the attributes are turned on; imagine trying to do this in your head or on a piece of notebook paper.
<p align="center">
<img src="_utilities/case-study-bitcoin-multisig-2.jpg" alt="map" title="map" />
</p>

In the image below, highlighting the `#backup` attribute reveals that there are two separate backups for `Seed-A`, one backup for `Seed-B`, but no backups for `Seed-C`. This is where the program's warning lights would come on.

Further analysis could be done by comparing the attributes of `Seed-A`'s two backups (e.g., Are they stored in the same place? Both susceptible to fire? etc.)
<p align="center">
<img src="_utilities/case-study-bitcoin-multisig-3.jpg" alt="map" title="map" />
</p>

Some may find a security risk in a multisig setup if a quorum of devices come from the same manufacturer. In the image below, we see that `Device-A` and `Device-B` are both share the `#Coldcard` attribute.
<p align="center">
<img src="_utilities/case-study-bitcoin-multisig-4.jpg" alt="map" title="map" />
</p>

### Note on Simplicity vs. Security
There is a balance between simplicity and threat avoidance: the nodes/connections/graphs are simplified if everything is in one location, you choose only one manufacturer, you have no backups to keep up with, etc., but by doing those things you put your whole system at risk. Too much simplicity can be at odds with security. By geographically separating objects, using multiple devices, and making multiple backups, you minimize catastrophic failure, but in the process you've created a spider web of relationships. A Security Atlas helps you assess and manage that spider web, to find that balance.

I've taken this concept as far as I'm able to: as an architect and city planner, I don't have the coding skills to mock up a functioning program. If you like this idea, please consider contributing your skills.

This is still a work in progress. The next case study is very much unfinished...

### Next Case Study
- [04 Your Home Server](04-Case-Study-Home-Server.md)


