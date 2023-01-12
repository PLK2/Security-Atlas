# Case Study: Your Home Server and Network

I created a Security Atlas for my home server and have found it extremely useful (see image below with gaussian blur for privacy).

<p align="center">
<img src="_utilities/case-study-home-server.jpg" alt="map" title="map" />
</p>

I assigned the following color key:
- Red: Virtual drive
- Light Blue: Computer device
- Dark Blue: Operating System, VM, Linux Container, etc.
- Yellow: Backup
- Orange: Program, Docker Container, etc.

All relevant information for each object is stored in their respective text files: e.g., each physical drive has its make, model, storage amount, etc., listed. This makes it not only a great security assessment tool but also a general management tool.

Another great thing about this tool is you can be as detailed or as general as you'd like with each of the components of the Atlas. For example, if I want to see all the dependencies that my `Photos` folder has, I can add that onto the graph without having to do the same for every other folder in my system. It's totally modular and can scale on an ad-hoc basis.

More info to come...
