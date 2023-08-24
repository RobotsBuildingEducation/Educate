## Shitty First Drafts - Computer Science


### Intro

Data structures and algorithms is the subject that push a lot of 
folks away from computer science because there's a culture of 
"weeding out" college students and professionals during interviews with 
this subject.

It it definitely challenging and you will have to have to 
practice in order to find success at this point.
I'll be able to help break down some concepts and offer 
guidance to make the challenge more reasonable,
but at this point if you're not willing to put in the work, 
you'll end up on the side that's weeded out. So let's begin.



### Programming Languages 

So let's start off by thinking about how programming languages even work.
We can explore something that we're all familiar with with autocorrecting technology,
or better yet, artificially intelligent answers. How does this work and how do computers 
seemingly "know" what to do?

Actually, how does a computer even know how to understand code in the first place? The
real question we're ultimately asking is here is, "how does a machine know how to interpret information?"

Well, like human language, there's going to be rules, regulations and structures to how we communicate.
How do we know that periods and commas invoke minor pause? How do we know that exclamations and 
question marks change the tone of speech? One way or another we had to design how it all 
worked and the rest ended up being history.

So let's take a look at a piece of code:

```js
let musician = new Musician("Drake")
let top_song = musician.getTopSong()
```

We don't really need to open up a giant manual for computer science to understand what's going on here.
We can simply break down this code by tokens in a rough way with just basic paper and pencil

```
We have a few tokens
- "let"
- "musician" and "top_song"
- "="
- "new"
- "Musician"
- "Drake"
- "."
- "getTopSong()"
```

A computer is going to break each part piece by piece since each token represents something competely different.
For example, a computer will understand that "getTopSong()" is a function and "new" is a way to create new objects based off a class definition.


Now some of this seems fairly obvious, but let's actually take a look at those tokens being broken down. What do you think the "Drake" string breaks down into?


The _string_ "Drake" is ultimately a string of characters. So "Drake" will break down into this:

```
["D", "r", "a", "k", "e"]
```

But is that it? What does an array of chracters break down to? Each character is going to have a mapping:


```
{
  0: "D",
  1: "r",
  2: "a",
  3: "k",
  4: "e",
}
```

It's at this point where computers start it's final process of converting readable data into machine code.

```
{
  0: \0x0044,
  1: \0x0072,
  2: \0x0061,
  3: \0x006B,
  4: \0x0065,
}
```

This then breaks down to the infamous binary

```
{
  0: 00000000 01000100,
  1: 00000000 01110010,
  2: 00000000 01100001,
  3: 00000000 01101011,
  4: 00000000 01100101,
}
```


### Data Structures

So the important part to understand about these transformations is that the the computer reserves space and creates addresses to reference information. Thinking about these addresses and references is what typically challenges computer science students, but it's really just a smaller atomic version of what we learned in the backend engineering lesson where we learned that most of these systems are connected networks of information that we send and receive data to.

And this why one of the first real data structures that you learn ends up being pretty difficult. It's not immediately intuitive like a mapping, a list or a string of characters. There are moving parts this time!

But fortunately, once you understand Linked Lists, you really start to build the foundation for understanding those super powerful algorithms you see with trees and graphs. So really, I would recommend to spend too much time practicing and understanding linked lists, because you're going to be using that foundation as things get more advanced. You really want to grind this out until it's pretty much second nature so that the next stage won't be so confusing.

Alright then, let's jump right into it and try to make sense out of this beast.


### Trees &  Algorithms

So like usual, let's start with the hard part first and break it down piece by piece so that we can make sense out of it. Before starting, let's agree on something.

Formal computer science courses have their time and place and the nature of our audience requires us to keep things in simple language. So it's not really productive for me to jump into scientific language by mentioning things like "post-order traversal", "recursions" or "branch and bound algorithm design". We're still going to touch on the essence of these subjects along the way. 

However, if you are a computer science I do have some advice when you work on these subject. My old Russian professor would simply say: "finger on the book. read it five times." It's good advice.

So let's start with a depth-first search. It's a way to move through trees and graphs. A tree is going to have a bunch of groups of data that are connected in some way. Let's call these blobs of data "locations", because a location is something that can provide a lot of details about something if you really think about it.

Actually, let's geek out a bit first. Let's think about a chess game. Forget the computer. We know the basics: we have a field of locations and characters that move across that field. Now there's really only two ways the travel across the board: you can move deep or you can move across. After that, it's really just a combination of those two things and making the right choices based on the problem you have.

Pretty simply right? That's algorithms. Actually, that's a lot of things are shaped this way if you really think about it. Let's think about other situations:

If you were to spotlessly clean up your entire house, which order of rooms would you choose and why?

If you were managing a soccer team, what positions would you select for your team and why?  

If you're packing your bags at the grocery store, which items are your organizing first and why? 

If you're organizing a stock market portfolio, which investments do you concentrate and diversify?

So let's go back to our tree. Very simply, depth first search is going to have us follow a path of locations downward first. Breadth first search is going have us follow paths that check locations across first. Let's take a look at a simple depth first search algorithm that counts the amount of `null` locations in a tree:

```
let count_null = (root) => {
  let count = 0;

  let depth_first_search = (current_root) => {
    if(current_root === null)
      count++

    for(let next_location in current_root){
      depth_first_search(current_root[next_location))
    }

  }

  depth_first_search(root)

  return count
}
```

Alright pause. You're going to notice two things here. This code is super simple, but it also feels really difficult. That's because you're dealing with real recursions and loops. This is the kind of stuff that makes fractal magic possible! So the real secret is here is this: slow down. count. It's all counting. Remember my Russian professor's advice?

Finger on the book. Read it 5 times.


Okay okay. Let's chop this up some more. Let's create our tree with code so that we have an easier time counting through something:

```
let root = {
  alphabet: {
    google: {
      chrome: true
    }
  },

  meta: {
    facebook: {
      threads: null
    }
  }
}

```

So if we were to go through this tree, what direction would we go? In this case, we're picking a branch and going down that branch. We're going deep first. So this will end up being the result:


```
step 1: { alphabet: { google: { chrome: true } }, { meta: { facebook: { threads: null } } }

step 2: { google: { chrome: true } }

step 3: { chrome: true }

step 4: true

step 5: { facebook: { threads: null } }

step 6: { threads: null }

step 7: null

result: 1

```


### Linked Lists

So, as you can see, these special algorithms aren't fundamentally **hard** but it will require some practice to be able to see these things with clarity. So what I really recommend is to focus your energy on this next data structure that we're going to walk through. It's the building block.


Linked Lists at the end of the day are pretty much one-dimensional trees and graphs. It starts in one place and goes in one direction toward the end rather than branching out in various directions. What this results in is less decision making to do when you reach a location - you're primarily focused on how to move across a list of locations.

Let's take a look at how a basic list looks:

```
let list = {
  head: {

    value: "meta",
    linkedTo: {

      value: "instagram",
      linkedTo: {

        value: "reels",
        linkedTo: null

      }
    }
  }
}
```

Not so bad right? The hard part here is that we just have to really think about how the data is grouped and connected. But again, if you take your time here, you can see that the concept is reasonable. It's really just software design that you're working through. So how do we build a linked list under the hood?

Well, honestly, it's just this!

```
class LinkedList {
  constructor(head){
    this.head = head
  }
}
```

This lets you process that list, that you generate with items containing data and their links. So a list item would look like this:

```
class ListItem {
  constructor(value){
    this.value = value
    this.linkedTo = null
  }

  setLinkedTo(listItem){
    this.linkedTo = listItem
  }

  getLinkedTo(){
    return this.linkedTo
  }
}
```

Now at this point, you need to connect the objects you create and manage their links. So an application of a linked list would look like this:

```
let meta = new ListItem("meta")
let instagram = new ListItem("instagram")
let reels = new ListItem("reels")

// instagram -> reels
instagram.setLinkedTo(reels)

// meta -> instagram -> reels
meta.setLinkedTo(instagram)

let company = new LinkedList(meta)
```

Oooo would you look at that? You'd be surprised how hard rocket scientists work to make things easy to understand you know! It's very important to understand the world that way too.

Anyway, let's walk through our list now. In order to do that, we need to extend how our LinkedList object works.

```
class LinkedList {
  constructor(head){
    this.head = head
  }

  getListItem(){
    //start from the top
    let currentItem = this.head

    // if you haven't reach reached an end point, keep going forward.
    // meta -> instagram -> reels -> null
    if(currentItem){
      while(currentItem.getLinkedTo()){
        currentItem = currentItem.getLinkedTo()
      }
    }

    return currentItem
  }
}

//...
console.log(company.getLastItem())

```

Finga on ze book. Read it fives times! Remember, this, at at the end of the day, is a counting exercise. So please take your time working through that and don't feel shame doing it in a way that works for you. Back in college, I would write a bunch of little dots all over the place in my notes as my way to count.

And again, don't forget how reasonable it is to practice this way. You're learning the mechanisms of computer programming that break things down into a bunch of 0s and 1s, which is not a natural language that you learned. So take your time and do what you got to do to work through the steps.

Oke doke, let's step it up a notch. Are you ready? We can use the same principles to reverse the direction of the list.

```
class LinkedList {
  constructor(head){
    this.head = head
  }

  //...
  reverse(head){
    let previousItem = null
    let nextItem = null
    let currentItem = head

    while(currentItem){
      nextItem = currentItem.getLinkedTo()
      currentItem.setLinkedto(previousItem)

      previousItem = currentItem
      currentItem = nextItem
    }
  }

```

FINGA!!! ON ZE BOOOK!! READ IT 5 TIMES ! ! ! ! No but really, it's just another counting exercise. The reason it's so important is because you're stepping through the parts that can get repeated at scale. What if a list or tree has a million different data points?

At this point, we can actually start to loop right back to where we started with programming languages and the design of algorithms. Every time we take these steps, we're given the chance to code or make new decisions. That decisions, one way or another, is going to get us closer to the answer we're looking for.

As usual, I recommend to just step away from the code for a moment and consider how many decisions you're always making. Slow down and observe. What categories and groupings do you create? Why do you create them? And how does that help you make it through the day-to-day? 

That's algorithms! If you spend enough time geeking out about it, you end up thinking about going in between and across dimensions of the universe.

![image](https://github.com/RobotsBuildingEducation/Educate/assets/65219666/65fb63ae-d536-48a7-8508-34bdce1969ed)

![image](https://github.com/RobotsBuildingEducation/Educate/assets/65219666/aa2d2a5d-1b71-4036-a503-155b390443b2)














