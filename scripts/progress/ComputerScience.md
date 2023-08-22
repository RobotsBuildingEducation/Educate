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

But fortunately, once you understand this next data structure, called Linked Lists, you really start to build the foundation for understanding those super powerful algorithms you see with trees and graphs. So really, I would recommend to spend too much time practicing and understanding linked lists, because you're going to be using that foundation as things get more advanced. You really want to grind this out until it's pretty much second nature so that the next stage won't be so confusing.

But like always, let's jump right into it and try to make sense out of this beast.


### Linked Lists


### Trees & Search Algorithms

### Algorithms



