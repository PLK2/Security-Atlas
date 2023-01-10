# Initial Setup

To repeat, this guide is a mockup of this process using a text editor. A program does not exist with the features we'll discuss (as far as I'm aware).

The goal: develop a user-friendly atlas, a personal repository, that maps out the characteristics and relationships of a system.

## Objects
A network is made up of objects that relate to one another; when shown visually, each object is a node on a [knowledge graph](https://en.wikipedia.org/wiki/Knowledge_graph). Objects can be anything you need them to be: sticky notes, safes, people, etc. Anything that plays a role in your network is an object to include.

Let's create our first object. Each object will be defined by its own, single text file. All we'll do is create a new text file with a filename being the name of our object; then we'll include a heading in the file with the name of our object. In this case, "Sticky-Note-1":

```
Sticky-Note-1.txt

# Sticky-Note-1
```

This is the first node in our graph.

## Owners
Each object has one or more **Owners** which are all the other objects that are required to access the object in question. Let's say Bob owns Sticky-Note-1:

```
Sticky-Note-1.txt

# Sticky-Note-1

## Owners:
- [[Bob.txt]]
```
```
Bob.txt

# Bob
```
Note that Bob owns himself--he is at the top of the graph hierarchy. Also note that the brackets around `[[Bob.txt]]` links `Sticky-Note-1.txt` to `Bob.txt` within Obsidian (this may be a standard markdown function, but if you're following along it may be different in your text editor).


## Backups
Each object may or may not have a backup copy. If it does, included it.

```
Sticky-Note-1.txt

# Sticky-Note-1

## Owners:
- [[Bob.txt]]

## Backups:
- [[Bobs-Notebook.txt]]
```

```
Bobs-Notebook.txt

# Bobs-Notebook

## Owners:
- [[Bob.txt]]
```

## Attributes
Each object may be ascribed any number of **Attributes**. These attributes are the potential threats that you believe to be worthy of analysis; they could pertain to theft, forgetfulness, natural disaster, etc. You could organize them however you'd like: e.g., by location, type, make, model, year, age, etc. They can be as specific or as general as you'd like. For a text editor like Obsidian, these attributes are handled with hashtags.

Let's define the following for our sticky note and its backup:

```
Sticky-Note-1.txt

# Sticky-Note-1

## Owners:
- [[Bob.txt]]

## Backups:
- [[Bobs-Notebook.txt]]

## Attributes:
- location: #bobs-home
- could be destroyed by: #water, #fire
```

```
Bobs-Notebook.txt

# Bobs-Notebook

## Owners:
- [[Bob.txt]]

## Attributes:
- location: #bobs-home
- could be destroyed by: #water, #fire
```

All objects that are downstream from an owner inherit all the attributes of that owner. This is an idea I'm unable to try out because my text editor (Obsidian) doesn't have this feature. However, it would be extremely useful to be able to visualize this as it would allow you to see the "butterfly effect" playout: could a flood at Bob's house result in the total loss of your bitcoin?...

This is an iterative process. As you go object by object, you will likely discover things pertinent for previous objects recorded. Eventually, it will congeal.


## Graph View
Now comes the fun part: being able to visually see the linkages of ownerships, backups, and attributes within your network. This is a visual, interactive atlas that you can use to assess the robustness of your network. For clarity, you can color code the nodes based on object type.

Let's dig in further with some case studies:

- [02 Bitcoin Single-Signature Wallet](02-Case-Study-Bitcoin-Singlesig.md)
- [03 Bitcoin Multi-Sig Wallet](03-Case-Study-Bitcoin-Multisig.md)

