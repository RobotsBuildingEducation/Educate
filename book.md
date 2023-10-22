# Table of contents

<ol>
  <li><a href="#0">0</a></li>
  <li><a href="#1">1</a></li>
  <li><a href="#2">2</a></li>
  <li><a href="#3">3</a></li>
  <li><a href="#4">4</a></li>
  <li><a href="#5">5</a></li>
  <li><a href="#6">6</a></li>
  <li><a href="#7">7</a></li>
  <li><a href="#8">8</a></li>
  <li><a href="#9">9</a></li>
</ol>

# 0



## Intro 
### NEEDS WORD BY WORD COMPARISON

**Scene 1**
Hey. I'm ms roxana

**Scene 2**
and I'm Sheilfer Zepeda. But you can call me Roberto, which is long for RO.B.E or Robots Building Education.

**Scene 3**
So you probably have a ton of questions that you want to address before getting started, so let's address them!

**Scene 4**
Before getting started ... yes, we use ChatGPT and AI here. 
We call her Roxana and we're going to teach you how to build these cool chat apps.

**Scene 5**
So I know some of you are probably a little scared or intimidated. So first, shoulders down, deep breath. 

**Scene 6  // **
Let's chill out and think about the metaphysical first. You might be wondering if you're smart enough or if you need to be good at math in order to learn this.

**Scene 7**
And I'm here to tell you that it's fine to feel that way, and if you could believe it, I also feel that way a little bit right now.

**Scene 8  // **
That's because I need to inspire confidence in a lot of people, and one good way is by giving people a great deal.

**Scene 9**
The basic deal that I'm offering is that I think I can teach you about coding in like 30 minutes, probably better than anybody else. And I can also teach a lot of other things outside of coding too.

**Scene 10**
And honestly, part of me is kind of nervous about doing that, but that's really no different than what you're feeling. It's a kind of imposter syndrome. 

**Scene 11 // **
But an easy way to deal with that is to ground yourself and to remember that that 
only happens because you want to hold yourself to a higher standard. 

**Scene 12  // **
But that feeling is a signal that you're looking at a challenge.
You want to move fast when you're not completely prepared. 

**Scene 13**
So let's get you prepared. How are we gonna do that?


**Scene 14**
Well, first, f you go on my app robotsbuildingeducation.com, you'll find a list of frequently asked questions, things like,
- "Is programming hard"
- "what computer do I need?"
- "am I too old?"
- "what kind of jobs can I do"
- "Is bootcamp worth it?"

**Scene 15**
But other than that, this is how we'll do it:

**Scene 16**
First, we're going to imagine and illustrate.

**Scene 17**
Second, we're going to draw connections and relationships.

**Scene 18  // **
Third, we're going to observe the new information.

**Scene 19**
Last, we're going to practice with it.

**Scene 20**
So that's the key. It's not hard. It is a challenge. But sometimes challenges can be made easier with the right help.

**Scene 21  //  **
So that's where I come in, really. I'll tell you often that I teach more than just coding, but I'm really only here to have you experience the sensation of learning. 


**Scene 22 //  **
I want you to feel that so that you remember that you're capable of learning anything that you want to, it's just that everyone has their own reasons. So all that coding, the content, the stocks, that's just like colors in a painting. You're here to learn and create impact out of it. 

**Scene 22**
The cool thing about computer science is that it's the science of computation, which means it's the science of solving problems. 

**Scene 23 // **
So you can do anything with it. You can apply it to climate technology, psychology, cancer research, art, sports, anything. 
Technology has a place where information exists! 

**Scene 24 // **
So my goal is to remind you of that. You can be that person. 
We are all that person - we all just have different reasons. 

**idk**
I think coding, creating and dealing are good subjects to help you 
along your way because it touches on subjects of using your mind to engineer, communicate and negotiate with reality.

**Scene 25**
And that's all. I encourage you to take some time to internalize this lesson. It's a good thing to take time with. 
Allow yourself be that person and find the courage to continue to walk in that direction. One day, if not already, 
you'll find the strength to turn the unknown into your home.

**Scene 26  // **
conclusion

# 1

**Scene 1**
Okay so boom, let's learn how to code. 

**Scene 2**
Here are the subjects we're gonna tackle:

**Scene 3**
1. Data and Logic
2. Loops
3. Functions
4. Creating Objects

**Scene 4**
We're gonna start with the harder parts first and work our way down. Remember that there are people from really different backgrounds here and I want to challenge you all in the right ways.  it's a challenge for me too - so trust me in the the informal direction we're taking here. Let's dive in.


## Objects

**Scene 5**
Alright so, we gotta create objects with code. Remember this - **in general, we use code to model the digital world with information, data and logic.**
So creating objects with code is one way to structure or define things. 

**Scene 6**
Here is the the key to understanding objects: you have a common way to define the **state** of an object and you have a way to manage the state with **functionality**.
There are different ways we can describe objects and you may have heard of some before, like smart contracts with cryptocurrency or displayable components like buttons on a screen.

**Scene 7 //// **
So here's a simple class, it's how you define how objects get made.

```ts
class Robot {


  let robot_name = ''
  
  constructor(name){
    this.robot_name = name;
  }
  
  update_name(new_name){
    this.robot_name = new_name
  }
  

  get_name(){
    return this.robot_name
  }
}


let roxana = new Robot("Roxana")

let sheilfer = new Robot("Sheilfer")

sheilfer.update_name("Sheilfer Zepeda")

sheilfer.get_name();

//what's the result of sheilfer.get_name()?


```

**Scene 8 /// **
Not so bad right? As you can see, some of this even feels a little bit natural. So I recommend that you open your Impact wallet and use AI or ask ms. roxana to help you learn when you need it but if you want support from me directly, old-fashion intelligence is available on discord too :)

**Scene 9**
If you take some time to break this down, you can see a little pattern forming here where you essentially lay out how the information works 
together. In general, you can create, update, receive or delete information. I mean, just think about something as simple as a Tweet. 

**Scene 10**
You recognize it as a social media product, but it's really how most code works - it's some block of messages that you can create, receive, update or delete .
```jsx
 let Tweet = ({ tweet }) => {
  let [liked, setLiked] = useState(false)


  let createLike = () => {     
     setLiked(true)
  }
 
  return(
    <section>

      <img src={tweet.user.photo_id} />
      
      <bold>{tweet.user.name}</bold>
      <icon>{tweet.user.isVerified}</icon>
      <label>{tweet.user.handle}</label>
      <label>{tweet.user.age_of_tweet}</label>
       
      <section>{tweet.text}</section>
      
      <label>{tweet.total_comments}</label>
      <label>{tweet.total_retweets}</label>
      
      <label onClick={createLike}>
        {tweet.total_likes}
      </label>

    </section>
  )
 }
```

**Scene 11**
After that, it's about managing all the relationships of data. So here's another key thing to lessone one:
**Coding is all about how you organize information. It's not about math.**

**Scene 12**
Alright, so let's keep the challenge going, we saw how a class creates an object and we saw how a component displays data and that's how a lot of code works under the hood. So let's evolve that with cool modern stuff like chatGPT or crypto. Here's a crypto transaction

```
contract RobotTransaction 
    recipient;
    amount;

    constructor(the_recipient, the_amount) 
        recipient = the_recipient;
        amount = the_amount;
    

    function send() 
        recipient.transfer(amount);


```
**Scene 13**
See that? Without much explanation of what's even going on here we can really just start to tackle some of these scary big smarty pants subjects pretty quickly.
Again, we have a process of defining the data and a set of functions to run common processes on them.


## Functions

**Scene 14**
But classes aren't the only way to define data. We also have functions, which we brushed over just now but they're still one of the most important ways to organize and handle our data.
Generally speaking, there are two types of ways to control the flow of data with functions: synchronous ones and asynchronous ones.

**Scene 15 ///**
You're pretty used to how the internet works as a customer of it but it's definitely worthwhile to pay attention to the little details that make your experiences feel smooth.
Synchronous functions are very similar to cooking in a pan, where the cook has their hands occupied managing the ingredients being heated.

**Scene 16**
Asynchronous functions are a little different, they're similar to placing frozen food in an oven, where a cook will have their hands free to continue working elsewhere while measuring the temperature of the food being heated.

**Scene 17**
The reason this is important is because when you handle data across a network, you don't know how long the data will take to load in, and your code usually moves in a synchronous fashion.
A simple way to visualize this is by opening any app and examining how various things load when operating it.

**Scene 18**
So why does that happen? Well, some code is working with external systems. All those systems these days is knowna as the cloud, but it can even be sending data from your computer to your internet modem too.

## Loops

**Scene 19**
Looping is  another way to control data. Usually when you have a group of data, you're able to perform some kind of repeatable function on all the parts or some of the parts. Check it out:

**Scene 19b**
```ts
let artists = [
  { 
    name: 'Kendrick Lamar', 
    spotify_monthly_listeners: 45,000,000 
  },
  
  { 
    name: 'Juan Gabriel',
    spotify_monthly_listeners: 9,000,000 
  },
  
  { 
    name: 'Jay Z',
    spotify_monthly_listeners: 36,000,000 
  }
];

let result = { 
  name: null, 
  spotify_monthly_listeners: 0 
}

artists.forEach(artist => {
  if(
    artist.spotify_monthly_listeners 
    > result.spotify_monthly_listeners
  )
    result = artist
})

console.log(result)

/* Challenge: what's the result? 
Leave the answer in Discord :) */
```

**Scene 20**
There are different types of looping functions. For example if you want to convert all of the values, filter values or reverse values, you can do that. Nows a great time to introduce this skill that most software engineers do and that's simply reading the documentation of the tools you're using. Most programming languages have huge dictionaries of information that outlines how things are made. This documentation will show you how these data grouping objects work and what functionality they contain.

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array

## Data and Logic

**Scene 21**
Okay so by this point, we're at the beginning where most people learn about the basics of coding. We skipped it because I felt that it was kinda obvious that data is informed by numbers, words, groups of data and functionality, because one way or another if you got to see this video, you were using the internet and familiarity is kinda just there.

**Scene 22**
So here's the key to this simple lesson here. Data creates logic, groups of data tends to create functionality. **Logic is ultimately just what boils down to being true or false. **That's how computers see the world. **** For example

**Scene 22b**
```ts

let obama = {
  is_married: true,
  is_president: true
}

let elon = {
  is_married: false,
  is_president: false
}

let legends = [obama, elon]

function isRelaxed(person){ 
  if(person.is_married)
    return true
  else
    return "needs to chill out"
}

isRelaxed(obama)

legends.forEach(legend => {
  isRelaxed(legend)
}
  

```

**Scene 23**
We can see a few definitions here working together to show you how individual pieces of data creates logic and how groups of data tends to create functionality. And that's all for lesson one!


## Conclusion

**Scene 24**
So let's slow down here. We went through almost 4 weeks of material in under 10 minutes. Here are the main things I want you to remember:
-  **in general, we use code to model the digital world with information, data and logic.**
-  **Coding is all about how you organize information. It's not about math.**
-  Logic is ultimately just what boils down to being true or false. **That's how computers see the world. **
-  

**Scene 25**
You might feel a little overwhelmed but that's fine, just trust the guidance I'm providing for you. At this point, if you go off onto your own, you might find that there's a ton of ways do things and it can get even more overwhelming. 

**Scene 26a**
First, I recommend using AI to help you stay focused as a beginner. Please remember that I'm also available to assist you via Discord too :)

**Scene 26b**
Second, I recommend that you go through the material here and write the code by hand on paper. Draw the connections you see naturally and try not to worry too much about being right or wrong. I tend to draw little dots and bubbles.

**Scene 26c**
Lastly, try practicing modeling what you see in the real world as data. Remember, don't think about being right or wrong. It's like cooking, where the more you do it the stronger your eye will be for it.

**Scene 27 ///////////////**
In the next lesson, we're gonna start putting this together and building real visual applications with HTML, CSS and Javascript with React. 


# 2

## Intro

**Scene 1**
Okay let's quickly review lesson one, We took at look at the fundamentals of organizing data with code.
We learned about objects, functions, loops and logic.

**Scene 2**
One of the examples we saw there was a version of a class that we call a component. 

**Scene 3**
Components are a popular way to create user interface and experiences. So let's take a look at this Tweet example.


**Scene 4**
```jsx

let Tweet = ({ tweet }) => {
  
  let [liked, setLiked] = useState(false)

  let createLike = (event) => {     
     setLiked(true)
  }
 
  return(
    <section>

      <img src={tweet.user.photo_id} />
      
      <bold>{tweet.user.name}</bold>
      <icon>{tweet.user.isVerified}</icon>
      <label>{tweet.user.handle}</label>
      <label>{tweet.user.age_of_tweet}</label>
       
      <section>{tweet.text}</section>
      
      <label>{tweet.total_comments}</label>
      <label>{tweet.total_retweets}</label>
      
      <label onClick={createLike}>
        {tweet.total_likes}
      </label>

    </section>
  )
 }

```
**Scene 5**
I used to find a lot of trouble back in the day when I would suggest that people are better off learning a skill like React 
instead the traditional HTML/CSS and Javascript, but that claim mostly comes from a place of wisdom rather than tradition. We'll get to that later and we'll see that here.

**Scene 6**
So before explaining React, let's just create a simple illustration. Our phones are these remote controls for the digital world. When we use these apps, we change the state of our experiences in the digital world. That's pretty true right?

**Scene 7**
So when you think about those elements in an app, and the way you interact with them, you end up creating these reactions where the state of the user interface or user experience has changed. That's pretty much how React and other component frameworks like Vue, Angular or HTML5 works. It's the frontend. It's event-based programming. 

**Scene 8**
These are the main parts of a react component:


**Scene 8.1**
1. You have the component's hooks

**Scene 8.2**
3. You have the component's state

**Scene 8.3**
4. You have the component's properties

**Scene 9**
As always, let's keep things simple. Hooks are functions that handles and synchronizes operations with the state of a component. I like to think about them like levers, where using the levers will result in the machine changing. 

**Scene 10**
Next is the state. The state is essentially the dynamic data that you're managing. It's the data that you expect to change because either machines or people are using it.
In short, when you change the state of the component, you're refreshing the display and causing the component to render again.

**Scene 11 ///**
Now here's where I rewind back to our conversation about learning React before HTML/CSS/Javascript. I don't believe there's anything wrong with doing it the traditional way,
but I really think it's worth observing **why** React, or other component-based frameworks ended up completely dominating and uplifting the field. They're really 
wonderful pieces of technology under the hood and I would encourage you all to study the programming languages internals and history along the way. It'll help you understand coding in a more well-rounded way because you'll get to see how companies influence change and upgrades. You get to see what Apple does and what Microsoft does kinda vibes. Trillion dollar energy!

**Scene 12**
Well, I guess this might just be me getting older and appreciating the little details of things, 
but isn't it kind of cool that programming languages translate things like `["hello", world"] translate to `new Array()`?
or, in React's case, `<header>Hello World</header>`, it translates to `React.createElement("header", null, "Hello World")

<img width="369" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/181d6c96-4c75-49fa-a5f2-a098cf448493">

<img width="370" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/c5fc6a0b-9dc5-40c1-946d-6d1c73c72f24">

**Scene 13**
Anway, let's stay on task. Now the last part of a component we really need to take a closer at are the properties of the component. Let's organize our tweet component more.

**Scene 14**
```

// we have the tweet property. We don't change it.
let Tweet = ({ tweet }) => {

  // state, defined by a useState hook
  let [liked, setLiked] = useState(false)


  // event that changes and updates states
  let createLike = () => {     
     setLiked(true)
  }
 
 
 // the component render/display
  return(
    <section>
      <img src={tweet.user.photo_id} />
      
      <bold>{tweet.user.name}</bold>
      <icon>{tweet.user.isVerified}</icon>

      <label>{tweet.user.age_of_tweet}</label>
      
      <Tweet
       
      <section>{tweet.text}</section>
      
      <label>{tweet.total_comments}</label>
      <label>{tweet.total_retweets}</label>
      
      <label onClick={createLike}>
        {tweet.total_likes}
      </label>

    </section>
  )
 }


```


```jsx      
let Tweet = ({ tweet }) => {
  let [liked, setLiked] = useState(false)
  let [tweetCopy, setTweetCopy] = useState(tweet);

  let createLike = () => {     
     setLiked(true);
     setTweetCopy({
        ...tweetCopy,
        total_likes: tweetCopy.total_likes + 1
     })
  }

  return(
    <section>
      <TweetHeader 
          photo_id={tweetCopy.user.photo_id}
          name={tweetCopy.user.name}
          isVerified={tweetCopy.user.isVerified}
          handle={tweetCopy.user.handle}
          age_of_tweet={tweetCopy.user.age_of_tweet}
       />
      
      <TweetContent
        tweet={tweetCopy}
      />

      <TweetCommands 
        tweet={tweetCopy}
        createLike={createLike}
        liked={liked}
      />
    </section>
  )
 }
```

**Scene 15**
So you might be looking at this code and thinking how some of it makes sense, but some of it is also too much. That's normal, yeah, because what you're really doing when you put hooks, state and properties together is a data model. You're looking at so many other things, like the flow of data, or all the little rules you might not be aware of. Like, why don't we change properties? Why do we only change state? When or why do we create copies? o that we can safely change values as needed? This ends up being fuel for imposter syndrome and writer's block or coder's block or another other blockage. 

**Scene 16**
But honestly, it's just practice. Remember, deep breaths. Challenge yourself. Experiment like a mad scientist. Break things. Coding is nice because the material is very cheap :) Lean on what you know! React is a framework and there are rules to how things work. It's like a soccer or football game, usually you can expect the goalie to be protecting the net rather than trying to score points right?

**Scene 17**
Wait hold on, pause. Look at you. You're engineering software. All those questions that you just asked are things you'll have to work through to answer, and that's exactly what software engineering is. It's not about writing code as much as it is planning and understanding the pipelines. Isn't that cool? How you feel right now is how professional software engineers sometimes feel too! So good job.

**Scene 18**
So here's the real bread and butter to becoming a React expert, and why React exploded in popularity - you need to understand how the data is supposed to flow using its system.
Let't take a look at our Tweet component again:

**Scene 19**
We have a function called `createLike` and it updates the state of the component. When the state of the component updates, the component's display refreshes.

**Scene 20**
The components display is a group of smaller components with properties. One component here event passes in our `createLike` function as a property. 
So what happens if we use `createLike` inside of that smaller component? Well, then both the `TweetContent` and `TweetCommands` components will update, because it updated appropriately inside of `Tweet` and it refreshed the display with new properties and state.

**Scene 21**
At first glance, it kinda seems like you're running in circles, but one of the reasons that React exploded in popularity was because of this contained one-way data flow. This ended up creating a lot of intuition between idea, planning and coding, because it was really easy to design the relationships and distribute objects that worked well together. As a result, people were able to create a lot of interesting architectures and controls over user experiences with these display containers and data pipelines.

**Scene 22**
To put it simply, like the Tweet, think about a typical tiktok video and the relationships that describe it as a series of messages. A video contains a like button, a comment section and a share button. A comment section contains comments. A comment contains a reply button. The list goes on and on in a number of ways. This is how Robots Building Education looks like:

<img width="590" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/04fd52cb-c3c3-4fab-a59d-5ccc89688008">

<img width="391" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/91f9c724-a575-4ce4-bd16-8be4f086de6e">



---

**Scene 23**
Phew, that was pretty tough. So we covered react components and more or less saw things in action. In summary, React is a data model that creates components with state and properties and displays visual elements with it.

So now let's take a look at these elements. Let's start with HTML.


# HTML
**Scene 24**
So some of you folks may recall this from the Myspace days. For those of you that aren't familiar, Myspace was a popular social networking site in the 2000s. Facebook quickly became the titan of the industry shortly after, but during those days a lot of people were able to customize their profile page. It was a lot of people's first experience with programming and many people enjoyed it. Well, that whole thing became an industry, and it's mostly lead by big tech organizations and their influence over how software is developed.

**Scene 25**
So, actually, that's why I tell people to learn React before HTML/CSS/Javascript. It's just the right economic thing to do if you understood who changes the software. React is ultimately an upgrade of the previous system and there's very little logical conclusion to do things inefficiently because any future upgrade now will be built off the influence of what React and Facebook accomplished. Let's put it this way, these days, you're probably going to learn some basics of photography on an iPhone first, and every year that passes it becomes more true.


**Scene 26**
You can learn them all at the same time, and truthfully, most engineers are not educators. They certainly are opinionated though, but that comes with the trade.

**Scene 27**
Anyway, the name of the game with HTML is just how you're structuring your display. I recommend to think about organizing things into containers and then placing the containers where they need to be.

**Scene 28**
The other main thing about HTML is understanding the attributes or properties that you can define and use. These, like most things I try to explain, are pretty common sense when you take your time with it.

**Scene 29**
Let's go through this example here. I have a header with some attributes. 



**Scene 30**
- An ID will create a identification label unique to that element, no different than an ID label on a shipping package from Amazon
- 
**Scene 31**
- A class will be a group identifier, where multiple elements can share an identity. This can be something like a "FRAGILE" box being shipped.

**Scene 32x**
- An event will handle user functionality like  like clicks, hovering, dragging, longpressing or any number of common interactions

**Scene 33**
- A style will allow you to design and customize how elements look!

**Scene 34**
The list goes on, and there's definitely plenty of attributes that you're going to use all the time, so you'll definitely run into them and pretty much remember them just out of frequency. Like the previous lesson, I recommend to utilize a combination of W3Schools documentation for HTML and CSS paired along with ChatGPT. You'll quickly see that there's so many attributes, and itll make sense why I recommend to know how to apply more than remember when it comes to learning code.



```jsx

let HeaderComponent = () => {

  return(
    <header
      id="App-Header"
      class="header-components"
      onClick={event => {
        console.log(
          "You clicked this element", 
          event.target.id
        )
       }
      }

      style={{
        padding: 25,
        margin: 15,
        borderRadius: '6px',
        backgroundColor: 'teal',
        color: 'pink'
      }}
    
    >
      <h1 
       style={{ 
        color: "gold", 
        textShadow: '1px 2px solid black' 
       }}
      > 
        Robots Building Education 
      </h1>
    </header>
  )
}

```


# CSS
**Scene 35**
So let's took at that style property and discuss CSS now. 

**Scene 36**
CSS stands for cascading style sheets, which indicates that it's used to design how things look and it also describes the order in which styles are applied. So in the example above, we see two font `color` properties`. One is pink and the other is gold. The gold one is what ends up being applied to the text display.

**Scene 37**
There are a number of ways to define and assign styles to an HTML element. Some older courses may suggest to learn about the `<style>` element, others may tell you about linking `styles.css` files to your HTML or javascript files. Others will teach you how to target and style elements by ID or class names, and many CSS libraries or frameworks work that way under the hood.

**Scene 38**
They're all valid and worthwhile to understand. I spent a lot of time handwriting my own CSS back in the day, and it usually takes a fair amount to convince me out of my ways, so I feel pretty confident in suggesting to first understand the inline example I showed you with the react `style` property or to take a look into Styled-Components, a library built with React. The reason I prefer this is because you have way more control over the data you're using. In short, it's just easier to do cool things.
  
**Scene 39**
Sheesh, with that out of the way, we can focus on what's really important. The foundation of CSS is that same key:value pair combination we see to describe data sets. There are a few ways we style our elements, so you need to understand these concepts:

**Scene 40.0**
  1. The box model - this is how we shape our actual elements

**Scene 40.1**
  2. The flexbox model -  this is how we position our elements

**Scene 40.2**
  3. The animation model - this is how we animate our elements
  
**Scene 41**  
I'll remind you often that our robot friends are helpful here to explore these concepts and phrases I use. Paired with ms. roxana, I think you can start to really dig deep!
  
**Scene 42**    
The box model basically describes how to shape those containers I was talking about. You probably have a rough mental model of what I'm talking about, take a look at this example and how it shapes this Rihanna button. In this case, you're going to be using these box model values so much, that you'll end up remembering them just out of how much you'll practice:
  
  ```jsx
    let Component = () => {
      return(
        <button 
          style={{
            height: '300px',
            width: "100%",
            margin: 24,
            padding: "15px",
            backgroundColor: "red",
            border: '1px solid black',
            borderRadius: '6px',
            color: 'rgba(255,255,255,0.9)',
         }}
        >
          Rihanna
        </button>
      )
    }
  
  ```
  
  
**Scene 43**    
Okay, so now let's step it up one notch. Let's position our elements. This can be pretty tough because you got to logically think about the size of different screens. To understand positioning, you gotta study the flexbox model. In a nutshell, you start to organize elements in rows and columns. Let's observe a few examples:
  
  
  ```jsx
    let Row = () => {
      return(
        <section
          style={{
            display: 'flex',
            flexDirection: 'row',
            justifyContent: 'center',
            alignItems: 'center'
          }}
        >
          <div>Kendrick Lamar</div> 
          <div>Rihanna</div>
          <div>Canelo Álvarez</div>
         </section>
      )
    }
  
    let Column = () => {
      return(
        <section
          style={{
            display: 'flex',
            flexDirection: 'column',
            justifyContent: 'center',
            alignItems: 'center'
          }}
        >
          <div>Pinterest</div> 
          <div>Tiktok</div>
          <div>Patreon</div>
         </section>
      )
    }
  
  ```

**Scene 44**  
 As you can see here, the elements are getting positioned based on its container. Frankly, I think this flexbox model got popular simply because it flows pretty well with how CSS and React data flows and applies. There are a number of different ways you can position these elements using the flexbox model, and like the previous lesson, exploring the documentations is what will lead your curiousity to success.
  
**Scene 45**    
Now the last part. The animation model. This is tough for me, because in the previous version I said it wasn't too important, but you could add some nices touches or details with it. AI changes things a bit. In the grand scheme of things, animations don't rank too highly in the business world but they can be satisfying or powerful at times. So let's take a look at the ways we can do it:

 **Scene 46**   
- We can animation with basic CSS
- We can animate by computing our own styles with react
- We can animate by using CSS keyframes
- We can animate by using the `<canvas />` element.
  
**Scene 47**  
Now if you were to research each item in the list, you would realize that the canvas element is by far the most complicated but the most powerful tool. In fact, I believe Khan Academy essentially teaches you javascript by using a library called P5.js that is centered around controlling and coding the canvas element the same way React is used to control HTML components.
  

**Scene 48**  
So, before it used to be an entirely seperate and specialized skill, but now chatGPT kind of makes things easier, and in the future, it certainly will make things easier. In fact, I'm using AI right now to come up with these examples because I haven't written this in quite some time. 

**Scene 49**  
So another way to animate elements is with keyframe animations. In a nutshell, you're defining the state of CSS properties based on cycle timer that ranges from 0 to 100%. Again, it's also not too important in the grand scheme of things, but people do create cool things with it.
  
**Scene 50**   
And lastly, the basic animations. This is what many people will include for basic accessibility practices, like signaling that a button has been selected, or visual cues indicating that a mouse is hovering over an element.
  
  
  
----

**Scene 51**   
So that's the frontend. Now let's witness how awesome you are and combine everything we've learned in the past two lessons so we can create the button on this app that talks to roxana and creates this education content:
  
**Scene 52**    
### DRY RUN SCENE IS COMPLETELY UNSCRIPTED 😭
```jsx
  
  let Button = ({ button, setCourseContent }) => {
    const [isRoxanaCreatingContent, setIsRoxanaCreatingContent] = 
      useState(false);
    
    let requestTask = async () => {
      if(button.name === "Discover"){
       setIsRoxanaCreatingContent(true)

       const response = await fetch(
         "https://robotsbuildingeducation
          .cloudfunctions
          .com/app/task",
         { 
           method: "POST", 
           body: JSON.stringify({ 
             prompt: "
               Hola Ms. Roxana, 
               could you create a RO.B.E 
               course for me please?
             " 
           })
         })

        setCourseContent(result)
        setIsRoxanaCreatingContent(false)
      }
    }
  
    if(isRoxanaCreatingContent){
      return null
    } 
    else {
      return (
        <button
          onClick={requestTask}
          style={{
              backgroundColor: "black",
              color: "white",
              width: "200px",
          }}
        >
          { button.name }
        </button>
      )
    }
  }
    
```

# 3
## Introduction


**Scene 1**
Backend software engineering is something that a lot of students don't understand. It sometimes feels like some kind of mysterious and cryptic role for smart people. I don't believe that's true, I think that just happens because people don't do a good job of explaining what backend engineering is.


![image](https://github.com/RobotsBuildingEducation/Educate/assets/65219666/54653819-33a8-4baa-a5a0-6335f5b575d5)

**Scene 2**
So let's clear that up here. Let's make it easy to understand so we can start thinking about larger systems and techniques.



**Scene 3**
These are the lessons we're going to cover:

1. Creating users
2. Database foundations
3. Backend Clouds
4. Operating systems & machines


# The Operating System

**Scene 4**
As always, let's work our way backward. By the end of this lesson, we're going to understand how to define users in applications and how that creates real user experiences.  This lesson is going to be pretty conceptual, so let's go into imagination mode. 



**Scene 5**
So let's highlight one of the key truths about computer science - we use technology to model the real world. Operating systems is kinda where computer science lives. I often suggest to students that they should think about what machines they want to work on before considering a programming language to learn for this reason.  I think people limit the range of where software engineering can exist and this is the concept where you can jump from a macbook to a bitcoin miner to a tesla robot.


**Scene 6**
So let's step away from computers and let's think about something more relatable, like a kitchen in a restaurant. We don’t have to imagine much other than appreciate all of the moving parts when it comes to creating the final product - your experience with food created and how it's served by the system of operation at the restaurant. 


**Scene 7**
From a customer’s perspective, you simply order and receive your food but the restaurant will launch a series of protocols to achieve that. Dishes will be washed, inventory will decline, policies and standards will have to be met, messages will be exchanged, things will break. 


**Scene 7.5**
You get the point. A lot of things happen to get your product prepared in a timely manner. 
The logic of things usually turns out to be pretty common sense and easy! The same is true for computers, which are mostly governed by their own operating system.


![image](https://github.com/RobotsBuildingEducation/Educate/assets/65219666/33eab7e4-4f6c-472b-aa59-4fec67efce77)


**Scene 8**
So now let's talk to our operating system in a way that you may not be used to. You’ve probably seen this kind of thing in movies or shows or whatever and it’s always this complex matrix of information, but it’s really just a text-based description of what you’re used to seeing with icons and inputs and other user-centric designs. It's a way to communicate with your computers with commands.


<img width="992" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/557c030f-d257-4c3c-ad51-e97e7662a9d8">

**Scene 9**
You might be wondering why engineers would use such a secretive tool, but it's actually really similar to the difference between ChatGPT generating and Google searching. It's boils down to different forms of usability.


![image](https://github.com/RobotsBuildingEducation/Educate/assets/65219666/3e152c96-92ca-4dea-9e18-5ae82e299fc4)

**Scene 10**
Studying operating systems can have an enormous amount of depth but it's the core of computing that helps you understand where AI fits into machines or why chips get designed to push the boundaries of modern computing. 


![image](https://github.com/RobotsBuildingEducation/Educate/assets/65219666/9393eaba-b95c-48be-8ba3-a2ecdd1648df)

**Scene 11**
I encourage you to really think about what's happening when you're using your devices so that you can appreciate some of the innovation along the way - operating systems these days are really phenomenal in their capacities and it's a good idea to practice appreciation of the little things!



# Backend Engineering



https://github.com/RobotsBuildingEducation/Educate/assets/65219666/733b2325-18ab-46b2-a2db-828c9773f6a6

**Scene 12**
So these terminals or command line interfaces takes us into the world of backend software engineering. One key thing to remember here is that we have to get comfortable letting the machines do the work for us. Let them rip! Remember that computer science is ultimately the science of solving problems and many problems have been solved so that you can program efficiently with powerful modern tools.

![image](https://github.com/RobotsBuildingEducation/Educate/assets/65219666/134b45fa-dc3b-4f87-8ef0-28c50aeb5a83)

**Scene 13**
Backend engineering is ultimately what gets everything connected. I like to think of it as constructing large pipelines with routes for different needs. Some pipelines may need to have data distributed for researchers and machine learning engineers. Other routes direct data to the right places to help us create smooth user experiences. You’d be surprised how much actually goes into seeing read statuses in chat applications or having your account secured when you log in and create and use data. 


<img width="672" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/1b791fb9-061d-45a8-9f7a-0ac80478516f">

**Scene 14**
But remember, programming models the real world & we primarily use the language of logic to achieve that. It’s really quite wonderful realizing that these large systems that govern all of these operations, like when you order from Amazon or task chatGPT for information ultimately boils down to predictable messages, signals & reactions in & outside of the technology being used. There's really no wrong way to look at it! It's information meant for your design.


<img width="728" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/fdf145b9-58f1-4008-9588-83bf8af4efb4">

**Scene 15**
Alright, so let's take a deep breath. Please try not to overthink this part, but please do engage in your imagination too. Like most things, it's going to be fairly predictable if you're given guidance. When you're using a command line to communicate with your machine or other external systems, you're going to have your bread-and-butter skills related to that. Cheat sheets people! Use them.


<img width="614" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/353436cf-8050-41f7-80c6-14dd93632891">

<img width="706" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/56de1984-024b-4d9d-b378-f078e3db647a">

**Scene 16**
And remember, it's pretty much like having a screen you can click on. You're going to do the equivalent of navigating file sytems, clicking download and install, or saving files to applications. Then if you're curious or a situation has you searching for answers, you can explore more advanced techniques - but for now let's apply one of the golden rules and Keep It Simple. 

# The Database

<img width="143" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/2cd4c6d2-aa03-49d5-a92d-17bfb0486117">

**Scene 17**
So that's kinda like level one of building the pipelines. The next part of building pipelines is understanding where the data is stored and how to move it responsibly, like the conveyor belts handling Macbook Pro deliveries around the clock.

![image](https://github.com/RobotsBuildingEducation/Educate/assets/65219666/6132ddc7-2143-4e25-84f1-2a1a6bf00c7e)

**Scene 18**
There are many different ways to store data, and you may have heard databases using tables with SQL or Excel, or non-relational databases structured with abstractions of key-value pairs. Either way, there's still that fundamental aspect to all of these differences and that's mostly getting used to organizing information using identities and mapping out relationships with those identies.

<img width="314" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/ed6bfc6e-0565-493b-b8f3-793a2825d1a2">


**Scene 19**
What that means is that we use identities to refer to and communicate packaged bodies of data. Using basic language, we can describe data inside of a database like this:

"In this collection of users authenticated by Google Sign-In, each user gets uniquely defined by a document of key-value pairs describing the user's profile."

<img width="505" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/57281963-bd9f-4180-b9eb-8b62c52540f5">



<img width="243" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/3c49310c-f9c5-4630-85b2-d5c4f197a227">
**Scene 20**
"This table of users connects each user to a table of high scores"

<img width="243" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/3c49310c-f9c5-4630-85b2-d5c4f197a227">

**Scene 21**
Now again, let's imagine the real world and how data can describe the various identities and relationships using combinations: 

1. What is the identity of the restaurant? CHIPOTLE
2. What is the identity of the city? Chicago
3. What is the identity of the neighborhood? Lincoln Park
5. What is the identity of the order number? A127B
6. What is the identity of the order type? Pick-up


**Scene 22**
From a human perspective, you ordered something awfully predictable and truthfully the same goes for its data perspective. It's a breakdown of things. It just takes practice to get a hang of designing relationships with data rather than just using it. In the example above, would you consider allowing a certain maximum of orders at a given time? Is it reasonable for a restaurant to promise and prepare 25,000 completed orders at exactly 5:30PM? How could that kind of bottleneck be alleviated? Is there a trend of what kind of ingredient is being ordered? You might be guessed already how data can be a creative exercise.


**Scene 23**
And if you haven't guessed it yet, you can just about describe anything these days and this is where we can start driving a lot of conversations about careers in artificial intelligence, data science or any other number of computational professions. Like lesson one, it's all about organizing data, logic and modeling the world. 



# Creating Users

<img width="315" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/06c85ed3-28b8-40ff-b2a3-9aa171c56ed1">

**Scene 24**
Now creating users is probably one of the most important constructions to understand because it packages our software to creating user experiences. 


<img width="392" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/09f3ceb0-09df-4b72-9e9f-a531ceb514b1">

**Scene 25**
In a nutshell, you create an account with a combination of data. So let's say you're using a service that allows you to build banking technology. That service will probably collect your login information, name, address and other financial data to create a unique identity. That unique identity will be converted into these secret keys that you'll get for creating an account and you can use those secret keys to connect your app code to the service. You go through authorization servers or authorization backends to accomplish this verification process. Pipelines people!

<img width="804" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/9e3b1ede-514e-457f-a730-a3660acbc704">

**Scene 26 //**
And that's all a user is. That's why users have these crazy letter and name combinations like "sKuU1185zZ6agp". Those identities eventually helps point data in the right direction. This is ultimately how you connect to services. You would be surprised what you can get out of the box these days, ranging from machine learning features to accepting payments.


## Conclusion

**Scene 27** 
As always, take some time to internalize some of this information. Let your mind explore the concepts and allow yourself to be creative. Don't worry too much about making "mistakes" when you're a beginner - letting yourself create mistakes gives you opportunities to improve. I can totally understand if you found this challenging on the first go because parts are definitely moving now but this ultimately why you get quizzed on these data structures and algorithms for some jobs. If you can theoretically understand those constructions, it can help you pick up the skills to understand large systems operating together too. But really, sometimes you don't need a atomic physicist to build a neighborhood of homes either, sometimes you need creative people for that too, so some people can be frustrated by the practice!


**Scene 28** 
We're going to go throught the process of connecting systems so that we can create an app with users in the next lessons, so that's all folks! See you later.


# 4
![image](https://github.com/RobotsBuildingEducation/Educate/assets/65219666/d5490f55-e9f9-469e-8b97-27358783405d)


In this lesson, we're going step-by-step to finally going to piece together everything we've learned so that we can build an application by connecting systems together so that we have real users.  Google, Youtube, ChatGPT and Stack Overflow will be your best friends here if you come across something you want to learn more about.



First we're going to download & install VSCode. This is where you write code.

<img width="204" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/0a522f35-a151-475a-80bc-dc550bd8a462">



Second, we'll download & install nodeJS. This lets you build javascript apps.

![image](https://github.com/RobotsBuildingEducation/Educate/assets/65219666/f05ec1f9-29fe-4cd8-a225-2a31dedf6373)


---

Then you'll have to open your command line terminal and install npm. NPM allows other developers to share their solutions with you in things called packages. We’re using a special command here called “sudo” which gives you administrator level permissions on your device, since I don’t know how your device is configured


<img width="563" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/f7825a4d-9c63-4545-ba90-70ac397b2048">


Create a folder and name it after your project. Im calling my app The Digital Border.


<img width="123" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/539b1c8c-deab-4edf-8a60-1188b266e41f">



Open VSCode and open your folder in the app the same way you open up documents on google drive or microsoft word.



<img width="971" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/ccdc9f0c-ff57-4814-a763-5507e8278422">


Find the little icons on the bottom left of your window to open up the the menu that contains an in-app command line.


<img width="302" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/196f950d-1e48-4203-88f7-47106c12b3f1">


Select the terminal option.
<img width="972" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/71b3dfb5-1d30-4f47-85a5-10054d161d9e">


Now run a command to start a react project with Vite. Remember what we said about letting the machines do the work for you? Use command `npm create vite@latest` and answer the questions. The following folder shows you how I configured the project using a React setup with javascript. They're even nice enough to tell you what to do next!

<img width="969" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/d72015b7-1438-45c8-860b-bcc3fd0fba33">


So let's do what they're telling us. `cd` stands for `change directory` which is pretty much like clicking into a folder.
<img width="667" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/7f2345a5-b219-48fd-8b84-d463ba471d07">



If you click the "package.json" file in your app folder, you'll see the list of software being installed for your project under the dependencies keys. This is what `sudo npm install` is going to do when you run it in your project. 

<img width="672" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/66df9839-86a6-4789-a42a-e918f411a6e8">


Alright, now let's run your app! Run `npm run build` and then run `npm run dev` and your app will launch in development mode! Congratulations! You can find more application commands in your `package.json` file under the "scripts" key.

<img width="653" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/3b99e3d0-fcd0-46a1-bcb8-fd94fd96323b">

<img width="1512" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/dbec6b33-f0a5-4aef-a2de-0300cce75aed">


Now let's set up our database with Google Cloud. Run this command to install firebase onto your machine: `sudo npm install -g firebase-tools`

<img width="537" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/effebf17-c251-44fc-af8b-f46e313f9b5e">


Then we initiate and set up the project with the command `firebase login`. You'll end up on a typical google login screen to authenticate your account

<img width="797" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/5b608605-441e-41e0-8183-cd9d1d18cb1a">


After logging in, we'll go to `console.firebase.google.com` and add your project. This will create your dashboard where you can use various backend services like authentication or even out-of-the-box machine learning tools.

<img width="845" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/782947e3-2b65-4ab5-a7c2-1714bbf9d1c1">

When you're in, activate the following services: authentication, firestore and hosting. I'm purposefully not telling you how to because I want you to explore this process with curiosity and I want you to trust your gut! 
<img width="1512" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/fe07bc78-32e7-41a3-b81a-7be09a122f66">

Once you've completed it, you'll find access to a secure website in the Hosting tab. In my case, it's `https://the-digital-border.web.app/`. Now we need to connect our code to this backend service.

<img width="1066" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/a64532b6-bd65-48fe-96ac-631687bb7708">



Next run `firebase init` and answer the following questions. These questions will write files into your project that connect your code to your firebase project.

In a nutshell, here are the steps:

1. Activate firestore and hosting.
<img width="602" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/f39406ab-7a19-4284-bc97-8fae797b58a6">

2. Select "use an existing product" and select the project you recently created.
   <img width="558" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/fa31a2d7-216d-471e-9917-9011f10428b2">

3. Press enter and allow firebase to create a file for rules to secure your data
<img width="438" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/f29566c6-7fb0-4f09-b6ef-1c7614fab936">


4. Press enter and allow firebase to create a file for indexes that helps you sort and your collections of saved data.
<img width="502" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/81c9f504-0d6f-466d-8d1e-9068cafc9985">

5. Then setup the following answers to configure your application and connect it to the web

<img width="565" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/a91acd2e-9ddf-45d3-b1ac-eef8c5363cd8">

6. Now earlier you had run `npm run build`. This essentially prepared your code for deployment. Run `firebase deploy` and you will launch your website!

Pretty cool right! Congrats!

<img width="1509" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/5dd76641-77dd-4597-a9fe-1f41068e7b29">



---

That's fire. let's create users. We need to install firebase and a react library that will make it easier for us to implement a login button. Run this command ` sudo npm install --save firebase react-firebaseui --legacy-peer-deps`. The legacy-peer-deps dependency will give you a stable version in the event that the React libraries we're using aren't up to date.

<img width="683" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/25780912-900c-40d5-a766-3eb793bd2fa3">


Next we have to activate authentication in our firebase dashboard, select sign-in methods, select the Google option, and enable it.
<img width="1254" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/13cda1ab-b5c1-4faf-a57b-ce92766c7366">


After that, we have to get data about your project to connect everything together once and for all. So go to your project settings
<img width="426" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/14f3d387-c7dd-4b5c-8282-918d1b5fd11f">


Select the web application denoted by the `</>` bracket symbol
<img width="979" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/fc92505d-6d16-432d-a287-2cf6beb46d13">

Register your app's name and you will get a set of keys. This is what will connect your backend to your code so you can customize your product.
You can find these keys in your project settings again and you can even use this to connect to other devices if you build on mobile or game studios like Unity 
<img width="987" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/887051df-605f-4b35-8c6f-6e86617e29f1">




# The Frontend


Now let's go back to your code. Let's create a folder called `database` inside your `app/src` folder and create a file called `firebaseResources.js`


<img width="564" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/21b242a6-d48b-4f1e-a1e9-3cdf6bc3afe2">


In our App.jsx file, we'll import a sign in button component from the library we installed and have it rendered.
<img width="585" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/b5425002-e862-4bf8-9812-40e77bfea5ac">




Now your app will have a login button that you can log into!
<img width="808" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/3f0d1cae-5fc6-4e88-aace-012333944780">

If we go into our authentication service, we can see that we've created a user
<img width="1370" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/46b473cb-f49e-42ac-bc62-54312db1de12">

So now we can continue to engage in this user construct so that we can create user experiences by defining what belong's in a user's profile. Lets import some things from functionality from firebase:

<img width="521" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/3fa64e01-47d4-4868-af28-d80ae91713f4">


Then let's define the state we're going to see on the screen:

<img width="458" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/f9051cfe-6e5f-4344-8f42-3ce39a4039d5">

After that we're going to use a common hook called `useEffect`. This hook allows us to set up our components and track different changes that occur throughout a component's usage or lifecycle.

<img width="560" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/f655084b-cfb5-475e-90a2-9649e03d9272">


Let's define a header component to prepare the display based on the state of the user being logged in or not:

<img width="524" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/be15b738-2bda-420f-9595-dcc586f8ef72">


Then we simply insert the header component into the rendering process

<img width="525" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/ddfdcd70-7393-4c2c-b53e-5d89aff18aab">




Amazing. You now have a real, live app that you can design and build in your vision. Run `npm run build` then `firebase deploy` again to refresh your website with the new code!
<img width="781" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/23c078da-6e44-4e40-bff5-e828576671fe">



# Summary

And here we are. Let's summarize what we did here. We used the command line to set up our application with react and firebase.
Then we configured our code using identities and keys to define our systems so that they can communicate and move data around.
This allowed us to create users and design user experiences.

So that's the nature of building applications. The frontend is going to handle user experiences, visual elements and events. The backend is going to design pipelines to communicate, design and move data across networks.

Now for the last part - working with other engineers.

# Github


Github is where we can collaborate with other engineers. Think of it like Google Drive but with extra steps so that code can update safely and predictably.

We're not going to go through a tutorial in this lesson because this is a worthwhile challenge for you to figure out on your own.
It will test your knowledge when it comes to connecting services and working with your operating system. 


It will also have you working like an engineer, so think of it like your first real test - you have some knowledge, but not all, and you need to figure the rest out. You've already made it this far, so taking the extra step will break you into a new level as a fresh engineer.


When you figure it out, you'll be able to onboard yourself to Robots Building Education. We'll have code here that works with ChatGPT and fintech to build nice features for families & communities. That being said, you would be really surprised what you can get away with with enough curiousity and smart tools.


So let's highlight some of the things you can expect to use regularly, your bread and butter concepts:

- Cloning -  this will allow you to copy code from Github to your computer

- Adding - Imagine a small container that prepares your code to be shipped to github, this puts your code's changes in the container.

- Commits - This adds a label, identity and description to your container of changes

- Pushing - this deploys or sends your code changes to your github repository

- Pulling - This brings in any updates from other people to the code

- Branches - branches are copies of the codebase within the repository itself. So you can push commits to a branch and merge it to your production code later.

- Forks - forks are copies of the codebase within your profile. So you copy the code and own it in your own profile. Most people do this as an alternative to creating branches or because they want to take the project in a different direction

- Pull requests - Pull requests is a function that allows you to compare the changes between branches/forks and allows your to merge them in. This allows engineers to perform code reviews

Merging - Merges is what ultimately gets code updated once and for all. Once code is merged, a lifecycle of updates is complete.


# Conclusion

I'm hoping that by now, your mind is spinning, your imagination is rolling and you had a challenging experience to build your confidence. Please do remember that I'm available for private tutoring if you need assistance with the material here or the steps to take after completing these lessons. You can expect these lessons to upgrade over time because they've been designed in a modular way that allows for them to improve continuously - so thank you for supporting Robots Building Education, the pleasure has been mine, and I look forward to meeting you and creating more awesome stuff for you!





# 5
## Shitty First Drafts - Computer Science


### Intro

#### Scene 1 
So data structures and algorithms is the subject that push a lot of 
folks away from computer science because there's a culture of 
"weeding out" college students and professionals during interviews with 
this subject.


#### Scene 2
It it definitely challenging and you will have to have to 
practice in order to find success at this point.
I'll be able to help break down some concepts and offer 
guidance to make the challenge more reasonable,
but at this point real practice is going to be necessary to find success.
So let's begin.



### Programming Languages 

#### Scene 3
So let's start off by thinking about how programming languages even work.
We can explore something that we're all familiar with with autocorrecting technology,
or better yet, artificially intelligent answers. How does this work and how do computers 
seemingly "know" what to do?


#### Scene 4
Actually, how does a computer even know how to understand code in the first place? The
real question we're ultimately asking is here is, "how does a machine know how to interpret information?"


#### Scene 5
Well, like human language, there's going to be rules, regulations and structures to how we communicate.
How do we know that periods and commas invoke minor pauses? How do we know that exclamations and 
question marks change the tone? One way or another we had to design how it all 
worked and the rest ended up being history. So let's take a look at a piece of code:


#### Scene 6
```js
let musician = new Musician("Drake")
let top_song = musician.getTopSong()
```

We don't really need to open up a giant manual for computer science to understand what's going on here.
We can simply break down this code by the tokens we see in a rough way with just basic paper and pencil.


#### Scene 7
```js
// Possible tokens
- "let"
- "musician" and "top_song"
- "="
- "new"
- "Musician"
- "Drake"
- "."
- "getTopSong"
```

A computer is going to break each part piece by piece since each token represents something competely different.
For example, a computer will understand that "getTopSong" is a function and "new" is a way to create new objects based off a class definition. Now some of this seems fairly obvious, but let's actually take a look at those tokens being broken down. What do you think the "Drake" string breaks down into?


#### Scene 8
The _string_ "Drake" is ultimately a **string of characters**. So "Drake" will break down into this:

```js
["D", "r", "a", "k", "e"]
```

But is that it? What does an array of chracters break down to? 


#### Scene 9
Each character is going to have a mapping:
```js
{
  0: "D",
  1: "r",
  2: "a",
  3: "k",
  4: "e",
}
```

#### Scene 10
It's at this point where computers start it's final process of converting readable data into machine code.

```js
{
  0: \0x0044,
  1: \0x0072,
  2: \0x0061,
  3: \0x006B,
  4: \0x0065,
}
```

#### Scene 11
Then eventually this breaks down to the infamous binary
```js
{
  0: 00000000 01000100,
  1: 00000000 01110010,
  2: 00000000 01100001,
  3: 00000000 01101011,
  4: 00000000 01100101,
}
```


### Data Structures

#### Scene 12
So the important part to understand about these transformations is that the the computer reserves space and creates addresses to reference information. Thinking about these addresses and references is what typically challenges computer science students, but it's really just a smaller atomic version of what we learned in the backend engineering lesson where we learned that most of these systems are connected networks of information that we send and receive data to.


#### Scene 13
And this why one of the first real data structures or backend architectures that you learn ends up being pretty difficult. It's not immediately intuitive like a mapping, a list or a string of characters. There are moving parts this time!

#### Scene 14
But fortunately, once you understand Linked Lists, you really start to build the foundation for understanding those super powerful algorithms you see with trees and graphs. So really, I would recommend to spend too much time practicing and understanding linked lists, because you're going to be using that foundation as things get more advanced. You really want to grind this out until it's pretty much second nature so that the next stage won't be so confusing.


#### Scene 15
Alright then, let's jump right into it and try to make sense out of this beast.

### Trees &  Algorithms


#### Scene 16
So like usual, let's start with the hard part first and break it down piece by piece so that we can make sense out of it. Before starting, let's agree on something.

#### Scene 17
Formal computer science courses have their time and place and the nature of our audience requires us to keep things in simple language. So it's not really productive for me to jump into scientific language by mentioning things like "post-order traversal", "markov chains" or "branch and bound algorithm design". We're still going to touch on the essence of these subjects along the way. 

#### Scene 18
However, if you are a computer science student I do have some advice when you work on these subject. My old Russian professor would simply say: "Finga on ze book. Read it five times!" You will see why this is good advice.


#### Scene 19
So let's start with a depth-first search. It's a way to move through trees and graphs. A tree is going to have a bunch of groups of data that are connected in some way. Let's call these blobs of data "locations", because a location is something that can provide a lot of details about something if you really think about it.

#### Scene 20
Actually, let's geek out a bit first. Let's think about a chess game. Forget the computer. 

#### Scene 21
We know the basics: we have a field of locations and characters that move across that field. Now there's really only two ways the travel across the board:

#### Scene 21
you can move deep 

#### Scene 22
or you can move across. 

#### Scene 23
After that, it's really just a combination of those two things and making the right choices based on the problem you have. Pretty simply right? That's algorithms. Actually, that's a lot of things are shaped this way if you really think about it. Let's think about other situations:

#### Scene 24
If you were to spotlessly clean up your entire house, which order of rooms would you choose and why?

#### Scene 25
If you were managing a soccer team, what positions would you select for your team and why?  

#### Scene 26
If you're packing your bags at the grocery store, which items are your organizing first and why? 

#### Scene 27
If you're organizing a stock market portfolio, which investments do you concentrate and diversify?

#### Scene 28
So let's go back to our tree. Very simply, depth first search is going to have us follow a path of locations downward first. Breadth first search is going have us follow paths that check locations across first. 
Let's take a look at a simple depth first search algorithm that counts the amount of `null` locations in a tree:


#### Scene 29
```js
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

Alright pause. You're going to notice two things here. This code is super simple, but it also feels really difficult. That's because you're dealing with real recursions and loops. This is the kind of stuff that makes fractal magic possible! 

#### Scene 30
So the real secret is here is this: slow down. count. It's all counting. Remember my Russian professor's advice?
Finger on the book. Read it 5 times.


#### Scene 31
Okay okay. Let's chop this up some more. Let's create our tree with code so that we have an easier time counting through something. If we were to go through this tree, what direction would we go?

```js
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


#### Scene 32
In this case, we're picking a branch and going down that branch. We're going deep first. So this will end up being the result:

```js
let root = {
  "step 1":
    { alphabet: { google: { chrome: true }},
    { meta: { facebook: { threads: null }}}
  
  "step 2": { google: { chrome: true } }
  
  "step 3": { chrome: true }
  
  "step 4": true
  
  "step 5": { facebook: { threads: null } }
  
  "step 6": { threads: null }
  
  "step 7": null
}
// ...
console.log(count_null(null)) // result will be 1
```


### Linked Lists

#### Scene 33
As you can see, these special algorithms aren't fundamentally **hard** but it will require some practice to be able to see these things with clarity. So what I really recommend is to focus your energy on this Linked List data structure that we're going to walk through. It's the building block for the more advanced stuff that you just saw.

#### Scene 34
Linked Lists at the end of the day are pretty much one-dimensional trees and graphs. It starts in one place and goes in one direction toward the end rather than branching out in various directions. What this results in is less decision making to do when you reach a location. So let's take a look at how to build and move across one.



#### Scene 35
```js
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

Not so bad right? The hard part here is that we just have to really think about how the data is grouped and connected. But again, if you take your time here, you can see that the concept is not super unreasonable. It's really just software design that you're working through, which you're neww at! So how do we build a linked list under the hood?


#### Scene 36
Well, honestly, it's just this!

```js
class LinkedList {
  constructor(head){
    this.head = head
  }
}
```

This lets you process a list, that you populate with location items containing data and their links. 


#### Scene 37
A list item would simply look like this then:

```js
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

#### Scene 38
Now at this point, you need to connect the objects you create and manage their links. So an application of a linked list would look like this:

```js
let meta = new ListItem("meta")
let instagram = new ListItem("instagram")
let reels = new ListItem("reels")

// instagram -> reels
instagram.setLinkedTo(reels)

// meta -> instagram -> reels
meta.setLinkedTo(instagram)

let company = new LinkedList(meta)
```

#### Scene 39
Oooo would you look at that? You'd be surprised how hard rocket scientists work to make things easy to understand you know! It's very important to understand the world in simple terms too.


#### Scene 40
Anyway, let's walk through our list now. In order to do that, we need to extend how our LinkedList object works.

```js
class LinkedList {
  constructor(head){
    this.head = head
  }

  getListItem(){
    //start from the top
    let currentItem = this.head

    // if you haven't reach reached an end point,
    // keep going forward.
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
console.log(company.getLastItem(meta))

```

#### Scene 41
Finga on ze book. Read it fives times! Remember, this, at at the end of the day, is a counting exercise. So please take your time working through that and don't feel shame doing it in a way that works for you. Back in college, I would write a bunch of little dots all over the place in my notes as my way to count how the computers were counting, like the Mayans!


#### Scene 42
And again, don't forget how reasonable it is to practice this way. You're learning the mechanisms of computer science that break things down into a bunch of 0s and 1s, which is not a natural language that you learned. So take your time and do what you got to do to work through the steps.


#### Scene 43
Oke doke, let's step it up a notch. Are you ready? We can use the same principles to reverse the direction of the list.

```js
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
}

//...
company.reverse(meta)
```

#### Scene 44
FINGA!!! ON ZE BOOOK!! READ IT 5 TIMES ! ! ! ! No but really, it's just another counting exercise. The reason it's so important is because you're stepping through the parts that can get repeated at scale. What if a list or tree has a million or a billion different data points to work through?

#### Scene 45
At this point, we can actually start to loop right back to where we started with programming languages and the design of algorithms. Every time we take these steps, we're given the chance to code or make new decisions. That decisions, one way or another, is going to get us closer to the answer we're looking for.


#### Scene 46
As usual, I recommend to just step away from the code for a moment and consider how many decisions you're always making. Slow down and observe. Why are you making those choices? What are you optimizing for? What categories and groupings do you create? Why do you create them? And how does that help you make it through the day-to-day? 

#### Scene 47
That's algorithms! If you spend enough time geeking out about it, you end up thinking about going in between and across dimensions of the universe.

![image](https://github.com/RobotsBuildingEducation/Educate/assets/65219666/65fb63ae-d536-48a7-8508-34bdce1969ed)

![image](https://github.com/RobotsBuildingEducation/Educate/assets/65219666/aa2d2a5d-1b71-4036-a503-155b390443b2)


#### Scene 48
Now to leave you with an ultimate challenge. Let's increase the difficulty by 1000! 😈

#### Scene 49
I want you to look into something called the N-Queens problem. You're going to find something obvious about the problem. It's complex. And by that, I mean that the amount of solutions becomes extremely large with very few inputs. It's kind of like multiplying something by 10 100 times, the number gets very large and it gets very complicated. 

#### Scene 50
But even in this case you're still doing the same thing to understand the problem: you're counting through steps and you're making choices every time you go through a step. The technique that you're really practicing here is a technique called "backtracking", which again, is something you naturally do in the real world with trial-by-error and unknown information.

https://en.wikipedia.org/wiki/Eight_queens_puzzle

<img width="580" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/63c3601e-b18a-4b2f-93b9-b3f99fbe0ed9">


# Conclusion

#### Scene 51
And that's all folks... for now. This is version 2 of the computer science lecture. And if it needs repeating... 

#### Scene 52
finga on ze - nah you get the point. 

#### Scene 53
I really meant it when I said that this lessons requires practice. At this point you're really starting to apply the foundations of computer science in meaningful ways that eventually results in you building algorithms that power applications that we know and love. 


#### Scene 54
And well, honestly, if you've gotten to this point, and you're working through these level of challenges, you really ought to consider where you are in life. At this point, it's definitely worth investing in yourself heavily. Whethere it's a tutor, a mentor, a community or tools to support your success - you really need to start making a habit of that because the things you're acquiring are deeply valuable and deeply necessary for our progress.

#### Scene 55
Much like lesson 1, you need to remember that you're not an imposter. You're just holding yourself to a high standard without the sufficient resources to feel confident from the get go. But that's fine. The way you want to work through that is with positive self-talk and affirmations that you are, in fact, that person, because we are all that person - we all just have different reasons.

#### Scene 56
So good luck! And if you need any more help from me, you know where you reach me. And if you don't... what is this amateur hour? Go to the link in my bio! FINGA ON ZE BOOK!!!!!!!

# 6

This is an initial essay and early access content to a lecture that will be released as "Self-Esteem" under the creator path. Feel welcome to provide further feedback or insight on this subject.



## Introduction

**Slide 1x**x
<br/>
Before starting, let’s step away from our predictable prejudices about the study of psychology, the conversations around it and its social impacts on the modern day so that we can begin to reform a stronger mental model around the subject. If we’re being honest, our generation and the generation before us has no real temporal concept of what a normal life is. Normal life, for all intents and purposes, did not really align with our narrow slice in history. We have no meaningful guidance or example to draw from.

**Slide 2x**
<br/>
That’s just the simple truth, we're mostly positioned to understand a world governed by the consequences of supernatural economic forces. Another peculiarity is that many of you, or us, find ourselves here as the first English speaking natives, which again, adds another layer of perspective. English itself has layers, whether it’s the business-savvy speech used in corporate offices, the specialized speech used in digital media  or the well-crafted speech by the academic. Simply put, the intersections of our existence on this plane is not immediately natural.

**Slide 3x**
<br/>
This is going to have consequences, and we may refer to them as generational curses or important conversations. You’ve heard about these before - men need therapy, hispanics need therapy, we need to complete our degrees, we need to be good parents, we need to rest, we need to be presentable, we need more self-love! The real challenge is how do we do these things from the right place? How do we do those things mindfully rather than in service to the glory of infinite productivity? How do we tap into peace?

**Slide 4x**
<br/>
These kinds of pressures are have consequences, which then brings us to these so-called difficult conversations and antidotes around depression, anxiety or the now-popular ADHD. So let’s leave all of that at the door. We don’t need it. I’m sure that we can agree that these conversations are typically poorly programmed, communicated or introduced.


## Self-Esteem

**Slide 5x**
<br/>
So before going into the clinical, let’s start off with a simple concept that we fundamentally have some control over. That’s self-esteem. It's our exposure to things. In short, self-esteem is how you feel about yourself or about things.

**Slide 6x**
<br/>
Let’s just focus on “how you feel” part. Yes. This the famous "how does that make you feel?" question. Why is that done? Well. Many people don’t do this. We feel, but don't spend too much time thinking about how we feel. We don’t revisit it. Truthfully, all of us do this and this can spark the process of declining mental health. So starting here puts us back on the roadmap to improved mental health!

**Slide 7x**
<br/>
So one way or the other, whether you have severe PTSD or bite your nails out of some emotion, you’re going to have to value the time spent thinking how you feel and the outcomes of whether you want to continue feeling that way. That’s the first step.

## Self-Acceptance

**Slide 8x**
<br/>
Self-esteem is how you feel about yourself or about things. The second part is somewhat of a Pandora’s box. Who are you and what are things? Why does “it” matter? What is perceived and what is understood?

**Slide 9x**
<br/>
At this point I recommend considering this mental model. Everything is true. That means multiple things can be true. You can be depressed and you can love life. You can have terrible focus and get an enormous amount of work done. You can hate someone and you can love them. Things can be personal or they can not be unserious. You can influence a lot around you and you have very little control over things.

**Slide 10x**
<br/>
Traditionally, these conflicts can cause people confusion. Here are interesting examples of this: Some families may not talk for weeks, months or even years. Some families talk daily. Neither is more correct or superior. Some cultures value eye contact, others do not. Neither is more correct or superior. You may meditate by lifting weights, doing chores or performing some other ritual - again, neither superior or more correct. Sometimes your perspective is informed only by a matter of the circumstance you were exposed to, but that does not necessarily mean that you have to operate or perform within the boundaries of those circumstances.

**Slide 11x**
<br/>
Self-acceptance is understanding that you can justly navigate the various perspectives about you or about things. Many people experience this as some form of liberation only because you’re removing one dominant or oppressive framework that guides your perspective in favor of the other universal ones that exist.


## Shame
**Slide 12x**
<br/>
It’s important to decouple our understanding of emotional health from systems of productivity because those systems produce some level of shame. It is omnipresent. Shame can be casted in many common forms, ranging from envy, to fear of rejection or to some other kind of inferiority.

**Slide 13x**
<br/>
One may wonder why such a cruel thing exists, but it’s ultimately a byproduct or waste of a competitive system. Systems of competition can or will produce some level of shame. There are winners and losers, one might say.

**Slide 13x**
<br/>
But fortunately for us, we’re reworking or improving our mental models here. The winners and losers concept is a popular default and we can spend time to alter it in meaningful ways.

**Slide 14x**
<br/>
So here’s the thing - not all shame is bad. Sometimes it’s justified. If you were a world champion athlete and you lost a high stakes game - well, what would you feel? It's clearly fine to feel some level of anger, disappointment or other intense negative emotion right? Sometimes it’s something we sign up for.

**Slide 15x**
<br/>
The real issue is when we are unaware with unknowns or when it embeds around us like some cosmic dark matter. We want to be aware that these systems of capital, competition and production are also systems that produce shame and we ought to be wiser to its influence. We still want to be appropriately discerning throughout this reality.

**Slide 16x**
<br/>
But in the beginning stages, it serves individuals to practice positive-self talk to immediately counteract some of these passive consequences and to improve the quality of our thoughts. One would probably agree that things are attuned toward negativity, pessimism or other easy default-mode and positive self-talk provides so healthy counterbalance to the pressures that be.

## Conclusion
In conclusion, I hope that these frameworks and models helped you consider or realize some of the complexities that you’re experiencing, have experienced or may experience. Take some time to work with these concepts to improve the quality of your thoughts or experiences. Try to resist creating a system of productivity along the way with it. It’s worth the time as it may alleviate excess symptoms of depression, anxiety or inability to focus along the journey.

Otherwise, if after enough work and practice, consider the opportunities to receive specialized help with those conditions. The work in this domain is far and wide and it's an important subject to respect. As difficult as it may be at times, we do have to have some level of accountability over our quality of life and there are inevitable choices we have to make when it comes to defining ourselves and our experiences.


# 7
## Interaction & Design
![image](https://github.com/RobotsBuildingEducation/Educate/assets/65219666/e1433e83-471d-46d8-b68b-ada52923067f)

first and foremost, UI/UX is short for user interfaces and user experiences. It’s a multi-disciplinary approach to research and design based on the study of human-computer interaction. It’s an excellent skill to have as it can take many different forms, shapes and sizes. For our intents and purposes, let’s define this skill as “Interaction Design” or simply as “Design”.

Some people refer to this profession as the psychology of technology or the therapy of technology. This is because an interaction designer is going to be interviewing and observing a lot of real input from people to gather deeper insights into a product. They will hold surveys, polls, interviews and any number of ways to communicate to people in order to accomplish this.

The key thing I want to highlight in this lecture is that the design work extends far beyond visual design and the brainstorming of good or clever ideas. It’s an incredibly thoughtful practice that can be applied to many environments. An interaction designer enjoys solving these types of questions

How do you improve this restaurant’s experience?
Do AirBnB hosts who value this skill perform better?
Which trailer in a movie produces the most anticipation?
Which video title is more likely to go viral?

As you can see, this skill, combined with some technical or business acumen, can be a pretty powerful amplifier!

#### Accessibility
<img width="660" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/3aeda922-471b-4cea-8683-ebd5d438303b">




Let’s start with accessibility, one of my favorite subjects as an engineer. In the study of computer science, we tend to approach problem-solving by accounting for the worst possible outcome. We do it as a way to practice building scalable solutions with information and data. Accessibility is a subject that has us working with design principles in that manner.

So let’s start with a basic website. It will have all the familiar bells and whistles that we’re used to; some navigation, some buttons and some text inputs. So what else does an interaction designer take a look at other than placing familiar elements on a screen?

Well, let’s consider folks that are blind. They interact with applications using intelligent tools and screen readers. So now we have to consider organizing the information in a way that makes sense for both visual and auditory users. Now the real benefit to this approach is that it’s often a win-win situation. Thoughtful creation for folks that experience limitations with accessibility often benefits folks without the limitation. 

For example, if a video lecture is organized in an effective way for blind folks, then people who are tuning in with just headphones can also experience information meaningfully! It’s considerations like this that made things like radio and podcasts such popular media formats for people of all backgrounds to consume.

## Multidisciplinary
![image](https://github.com/RobotsBuildingEducation/Educate/assets/65219666/d007965f-17de-4599-925b-47782ceb04cc)

So hopefully that conversation has you curious about what design even means. You may notice there’s an umbrella of sorts covering a lot of topics. This is because human-computer interaction is fundamentally multidisciplinary. We tend to just talk about it within the context of technology given that technology is also multidisciplinary.

However, it’s all the same if you're a chemical engineer, a business owner, an architect or even a teacher; you will be able to find enormous value integrating the principles of design in your work.

The choices you make have a serious impact. The key words you choose can influence how search engines and social media algorithms distribute your material or how it gets consumed by an audience. The intent behind the features, the tone or the expressions you use can affect how successful retention is. It can give you a significant competitive advantage. It's attention to detail.

Because of the scale of the umbrella, it can be easy to justify something as “good or bad design”. It lends itself to opinion. The best design tends to be whatever makes the people you’re designing for happy and if you want to make even more people happy, well, you’re gonna have to talk to them! The rest is just research, and research is largely meant for discovery.

Many folks may go in another direction, where they start with the discovery part first and then try to convince folks that their solution is superior in some way. Nascent technologies like cryptocurrencies are notorious for this.

However, the study of design also lends itself to the study of new technologies. So hype waves around things like Bitcoin or artificial intelligence is a great time for newcomers to jump in and make contributions toward large problems.

#### Heuristics
![image](https://github.com/RobotsBuildingEducation/Educate/assets/65219666/55a6dc61-5c0a-44f8-9e99-e6033b498759)


Now navigating new technologies is always going to be an exciting challenge. Heuristics are essentially guidelines you can use while you create something with constraints or limited feedback. Some things are inevitably repeatable, like considering how a user can correct a mistake or malfunction. These are simply guidelines rather than rules or regulations. There’s an added benefit since they have a tendency to build or bounce off one another.

And these guidelines really introduce you to the practice of interaction design. It’s at this point where you start to learn lower level concepts like the usage of affordances, which are the signals or properties of an object and how that informs a user of its possibilities or potential use cases.

In a rather absurd sense, these concepts are the things that remind you that a water pitcher is meant for pouring water rather than it being a glove to protect your hand. They’re the details that help us realize that pixels on a screen are supposed to represent buttons that we can interact with.

And if you take some time to ponder that idea, you can really start to appreciate the little things in design. Why is that when we see a glove, we know it’s meant to protect our hands? What inspired a fork and a pair of chopsticks? Why did the iPhone get rid of the headphone jack?!

#### Design Systems
<img width="707" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/9bf2436c-abf4-4e88-94b0-520fee6e4f33">

Ok. let’s take a step back and review. We value accessibility because it’s fundamentally about enabling more people to do things. We understand that design research is multidisciplinary and encourages us to talk to people directly to gain more insight. We use guidelines to give us a sense of direction when developing ideas or products.

With these fundamentals in mind, it’s worth reviewing the number of ways you can gather insight or communicate your ideas. Much like engineering, your tool of choice is going to carry tradeoffs and consequences.

For example, the outcomes of paper prototypes may range wildly based on where it’s being seen - a boardroom and a Tiktok video carry different results. Finding the resources and budget for surveying may lead to skewed or biased results. Doing personal interviews may mislead your direction and be costly on a schedule. You may find an inexpensive or free tool you found on the internet to be more effective or useful than some fancy enterprise software.

But over time you start to find what works well with you or with different teams. And it’s here where I can only advise you to think critically and keep an open mind when making your design choices.

#### Further Reading
<img width="1023" alt="image" src="https://github.com/RobotsBuildingEducation/Educate/assets/65219666/f594b0dc-2c2d-4a8d-95d7-f13590df6bbd">


Lastly, if you enjoyed this subject, I highly recommend a few more follow-up sources. It’s worth your time to check out “The Design of Everyday Things” by Don Norman, who is widely revered in the field of human-computer interaction.

I also recommend using the resources available at nngroup.com, which is the Nielsen Norman Group. This is a knowledge base meant for professionials concerned with standards.

If you’re curious to see what real-world UX research looks like, you’re encouraged to join Bitcoin.design, which is an open-source platform that supports usability research & development for Bitcoin.

These three resources in combination will provide a deeper introduction into the process and perspective of a designer. If you're part of the Robots Building Education community, feel free to use design principles to communicate ideas, improvements or case studies to gain experience here too! I'm happy to sit down with you and brain storm or progress on things that can improve our little AI mentoring platform here =)

# 8
### Story
One of the first problems I encountered after graduating from college was not getting any calls back from employers. This didn’t really make sense to me since I was a qualified and competitive candidate on paper.

The problem was my resume. It didn’t communicate that value well and I didn’t communicate it in a way that made it helpful for the person organizing out applicants. I thought about my skill in user experiences and focused heavily on improving the communication part.

These changes had significant outcomes. I started to get calls back from places like Tesla and other competitive employers after making the adjustments. So let’s break this down.

—

### Interface

The important lesson here is to remember that a resume is a document meant to communicate your value proposition for a business. So it’s fundamentally a communication problem. This means it follows the same structure as telling a story or idea.

The following interface is highly opinionated. Its intention and purpose is to educate a rookie resume writer on the challenge, since a competitive resume is often people’s first encounter with real-world business.

Here are some other things to consider while learning this:

Your LinkedIn profile should be optimized for recruiter search tools. Titles and years of experience are highly ranked.
Your resume should be effective in highlighting your candidacy in 6-10 seconds.
Your resume should offer a productive conversation about your career progress in 30 seconds to 2 minutes
Resume readers have inherent bias and expectations and are subject to uncontrollable conditions like mood or experience.
Not all good resumes pass and not all bad resumes fail! Don’t take things personally.

—

## Format

With that in place, let’s introduce the general format:

Spacing is strict
Font highlighting is strict
Order of information is strict
Alright so the first real rule is the 1 page rule. In short, you have to be able to communicate your value effectively. The right practice here is to avoid using fluff and filler since that often takes away from effective communication. Instead, leaning on honesty will either inspire more confidence in later stages of the interview process or inspire you to develop your background more competitively. 

One thing I often teach is that imposter syndrome is the result of holding yourself to a high standard while not always having all the resources to prepare enough for that standard. If you feel it while writing a resume, your best bet is to avoid using fluff or filler and to lean on honesty & confidence in order to guide your risk-taking & professional development.



—

### Education

Next up is the education part. This is your introduction. Keep it simple and move on. It doesn’t matter if it’s a community college, a vocational school, an online degree or an Ivy League. Slap it on and keep it moving.
—
### Skills

This is a follow-up section to your education introduction. This section may not be necessary for some professions that aren’t heavily based on usage of tools like software engineering. I recommend to segment into two or three sections labeled “Proficient”, “Explored” and “Spoken”. Proficient skills should be things you can talk shop about with a professional. It should be a skill you’re comfortable with. Explored skills should highlight curiosity and engagement with tools you’ve used in the past to accomplish meaningful things.

—

### Experience

This is the main part. It's going to be challenging to follow conventional resume advice about making a significant impact at organizations at the entry level. If you are unable to do that, then consider defining the impact of your role at the company followed by the type of experience you gained at that role.

—

### Volunteering & Open Source Work

The employment market is something that ebbs and flows with the conditions of the economy. Some career mentors will suggest things like projects, extracurriculars or other endeavors like I once have, but in the competitive market of 2023, I would highly recommend searching for volunteer and open source experience. 

There’s a number of reasons for this other than highlighting attributes about your candidacy. Doing so also allows you to expand your network in meaningful ways.


### Conclusion

With all of this in mind, what you’ll get is a one sheet document that allows employers to quickly and effectively evaluate your candidacy through the lifecycle of an interview process. Again, it helps to treat a resume like a story, a video or some other communication piece. It should see multiple word-by-word revisions and its flow should feel good to go through. And as always, if you need extra help or support on a resume, feel welcome to hit me up and schedule a meeting on Patreon 





