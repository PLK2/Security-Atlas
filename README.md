# Threat Modeling with a Knowledge Graph

*You did it: you've set up your own home server and network! You've cobbled together multiple computers, drives (both physical and virtual), virtual machines, docker containers, subnets, and backups. Everything is working, but then you're hit with an unnerving feeling: Did I cover everything? Am I backing up everything properly? What are the vulnerabilities (an error, a hack)? **What are the implications if something--anything--goes wrong?** Where is my [*insert super personal dark secret here*] actually stored, who (or what programs) are required to access it, how safe is it from loss?*

*You grab a pen and paper and start drawing it all out, trying to discern the interrelationships, then you quickly realize **you've drawn an incoherent spider web**; it makes no sense. So you throw that away, open up an Excel file, and try that domain: this cell relates to that one, this row is affected by that column; still, the subtle connections remain hidden. You search reddit for what other people have done and all you find are basic network topology maps. You search the broader internet and, ho!, find what you're looking for! Only to realize it's enterprise software, highly-advanced threat intelligence services for big businesses, not for you. Is there nothing in between?, you ask yourself.*

There is: threat modeling using a knowledge graph, **a method for analyzing and stress-testing a network of objects (their interrelationships and interdependencies) using switchable and generational attributes. It is a graph of interactive nodes, allowing users to audit the network under user-defined stressors and circumstances.** It won't tell you exactly what vulnerabilities are in your network; it won't tell you how to fix it; it won't scan your network and develop an automated graph for you. Instead, it is a hands-on, bare-bones assessment tool you build yourself; and that's important: the process of building it is part of the process of learning about the actual threats to your system. **It is an x-ray view of that house of cards you just built for yourself (whether that's a home server, a multi-sig bitcoin wallet, or any other network of objects that rely or relate to one another). It helps you to see relationships that otherwise would remain hidden behind the complexity.**

<p align="center">
<img src="_utilities/case-study-bitcoin-multisig-1.jpg" alt="map" title="map" />
</p>

Note that this is a non-technical guide introducing the concept of threat modeling using a knowledge graph; it is in need of technicians to bring this tool to life. If you find this useful, please help!

To get started, I've developed a mock-up of the process using Obsidian, a program that allows you to build a personal knowledge base using nothing but text files. You don't have to use Obsidian--you could use any number of similar programs. My hope is that someone with coding skills will find this useful enough to build an actual application.

### Read On
- [01 Initial Setup](01-Initial-Setup.md)
- [02 Bitcoin Single-Signature Wallet](02-Case-Study-Bitcoin-Singlesig.md)
- [03 Bitcoin Multi-Sig Wallet](03-Case-Study-Bitcoin-Multisig.md)
- 04 Personal Home Server and Network

---
**Keywords to use for later, maybe:**
- simulator
- prototype
- atlas
- semantic network
- frame network
