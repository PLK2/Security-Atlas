# Case Study: Bitcoin Key Management for a Multi-Signature Wallet

Things get immensely more complex when multiple devices and signatures. Below is a basic two-of-three multisig wallet; a glance of the knowlege graph reveals a number of hidden corners to analyze.
<p align="center">
<img src="_utilities/case-study-bitcoin-multisig-1.jpg" alt="map" title="map" />
</p>

It gets even more convoluted when the attributes are turned on. But imagine trying to do this in your head or on a piece of notebook paper.
<p align="center">
<img src="_utilities/case-study-bitcoin-multisig-2.jpg" alt="map" title="map" />
</p>

In the image below, highlighting the "backups" attribute reveals that there are two separate backups for Seed-A, one backup for Seed-B, but no backups for Seed-C. This is where the program's warning lights would come on.

Further analysis could be done by comparing the attributes of Seed-A's two backups (are they stored in the same place? are they both susceptible to fire? etc.)
<p align="center">
<img src="_utilities/case-study-bitcoin-multisig-3.jpg" alt="map" title="map" />
</p>

Some may find a security risk in a multisig setup if a quorum of devices come from the same manufacturer. In the image below, we see that Device-A and Device-B are both "Coldcards".
<p align="center">
<img src="_utilities/case-study-bitcoin-multisig-4.jpg" alt="map" title="map" />
</p>
