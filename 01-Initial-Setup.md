# Initial Setup

To repeat, this guide is a mockup of this process using a text editor. A polished, use-specific program is required to test its potential. Until then, we'll be using text files.

Let's start with an **Object**. Every object will be defined by a single text file and is represented as a single node on our knowledge graph. Objects can be anything you need them to be: sticky notes, safes, people, etc.

Let's create our first object. All we'll do is create a new text file, the file name will be the name of our object, then we'll include a heading in the file with the name of our object; in this case, "Sticky-Note-1":

```
Sticky-Note-1.txt

# Sticky-Note-1
```

Each object has one or more **Owners**. These are simply other objects that are required to access the object in question. Let's say Bob owns Sticky-Note-1:

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

Each object may be ascribed any number of **Attributes**. These attributes are the threats that you (the builder of the graph) believe to be worthy of analysis; they could pertain to theft, forgetfulness, natural disaster, etc.

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

Objects that are downstream from an owner inherit all the attributes of that owner. This is something I'm unable to try out as my text editor (Obsidian) doesn't have this feature. However, it would be extremely useful to be able to visualize this as it would allow you to see the "butterfly effect" playout: could a flood at Bob's house result in the total loss of your bitcoin?...

## Graph View

Colors = type

