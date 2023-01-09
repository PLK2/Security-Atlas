# Case Study: Bitcoin Key Management for a Single-Signature Wallet

Below is a simple configuration for a bitcoin wallet requiring a single signature. Every node is an object (device, person, password, etc) in a chain of custody for the "Wallet-Single-Sig" (the utxo or treasure that is being protected). I've colored some of the nodes to indicate the following:
- Red denotes a physical device
- Yellow denotes a backup
- Blue denotes the treasure
<p align="center">
<img src="_utilities/case-study-bitcoin-singlesig-1.jpg" alt="map" title="map" />
</p>

The **Attributes** are hashtags that can be turned on and off. They reveal the underlying "threats" one may wish to analyze. In this case, the type, location, and make of an object.
<p align="center">
<img src="_utilities/case-study-bitcoin-singlesig-2.jpg" alt="map" title="map" />
</p>

Below, we can see what all objects are subject to any threats related to "home": e.g., burglary or fire. Ideally, this "home" attribute would be inherited by every downstream object; e.g., the "Seed" object is also susceptible to any "home"-related threat because both of its upstream owners are susceptiable. This makes the "Wallet-SingleSig" object susceptible as well; this would be highlighted with a "threat path".
<p align="center">
<img src="_utilities/case-study-bitcoin-singlesig-3.jpg" alt="map" title="map" />
</p>


Selecting an object reveals all upstream and downstream relationships. In this case, the "Hardware Wallet" object requires both "Uncle Jim" as well as a "Hardware-Wallet-PIN" to access it, while the "Seed" relies on the "Hardware Wallet".
<p align="center">
<img src="_utilities/case-study-bitcoin-singlesig-4.jpg" alt="map" title="map" />
</p>

