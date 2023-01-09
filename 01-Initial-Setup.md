# Initial Setup

To repeat, this guide is a mockup of this process using a text editor. A polished, use-specific program is required to test its potential. Until then, we'll be using text files.

## Objects
A network is made up of objects that relate to one another; when shown visually, each object is a node on a knowledge graph. Objects can be anything you need them to be: sticky notes, safes, people, etc. 

The first step in this tutorial is to start with a rough sketch or outline of the network you want to study.



Now let's create our first object. In our system, each object will be defined by its own, single text file. All we'll do is create a new text file with a filename  being the name of our object; then we'll include a heading in the file with the name of our object. In this case, "Sticky-Note-1":

```
Sticky-Note-1.txt

# Sticky-Note-1
```

## Owners
Each object has one or more **Owners**. These are all the other objects that are required to access the object in question (or is a backup copy of the object, more on that later). Let's say Bob owns Sticky-Note-1:

```
Sticky-Note-1.txt

# Sticky-Note-1

Owners:
- [[Bob.txt]]
```
```
Bob.txt

# Bob
```

## Attributes
Each object may be ascribed any number of **Attributes**. These attributes are the threats that you believe to be worthy of analysis; they could pertain to theft, forgetfulness, natural disaster, etc. You could organize them however you'd like: e.g., by location, type, make, model, year, age, etc. They can be as specific or as general as you'd like.

In this case, let's define the following for our sticky note:


```
Sticky-Note-1.txt

# Sticky-Note-1

## Owners:
- [[Bob.txt]]

## Attributes:
- location: #bobs-home
- could be destroyed by: #water, #fire
```

All objects that are downstream from an owner inherit all the attributes of that owner. This is an idea I'm unable to try out because my text editor (Obsidian) doesn't have this feature. However, it would be extremely useful to be able to visualize this as it would allow you to see the "butterfly effect" playout: could a flood at Bob's house result in the total loss of your bitcoin?...

This is an iterative process. As you go object by object, you will likely discover things pertinent for previous objects recorded. Eventually, it will congeal.


## Graph View
Now comes the fun part: being able to visually see the linkages of ownership and dependencies within your network. For clarity, you can color code the nodes.

See case studies below:

- [02 Bitcoin Single-Signature Wallet](02-Case-Study-Bitcoin-Singlesig.md)
- [03 Bitcoin Multi-Sig Wallet](03-Case-Study-Bitcoin-Multisig.md)

