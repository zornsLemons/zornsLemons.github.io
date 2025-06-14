---
title: "How to read a math book"
description: "Math books are terse, and often opaque. Here is how I get through them" 
theme_version: '2.8.2'
---

There are many ways to read math, Here is my strategy, it works for me, others do this differently with great success. I can't tell you how to live your life but my suggestion is to try it this way and adapt it to your style. I read with the book, a pen, and a legal pad (or a white board/chalk board, or if you're so inclined a TeX editor). You want to make it cheap to write stuff down because you'll be writing a lot more than you're reading so  do whatever you need to achieve that.

The general form of a math book is to define something, prove a bunch of stuff about it, and then define something else. **GENERALLY** (this is not true of every book), a section is dedicated to facts about a particular object that is defined from jump, a chapter is a collection of sections discussing associated objects that are defined and discussed in the sections, and then there are some sections scattered throughout where they prove some big results. Definitions, examples, theorems, and proofs are how we communicate mathematical concepts, they are the beginning, middle and end of mathematics.

## If you feel like your reading slowly, then you're reading too fast. Slow down. 

this isn't a race, no one is handing our medals, no one will be at the finish line to wrap you in a tin foil blanket and give you a coke and a smile. You're doing this for **You**. 

Let's get really concrete for a Moment. When I was in undergrad, I took a class covering Axler's *Linear Algebra Done Right* over the course of a 10-week quarter. We finished the term with the Spectral Theorems and unitary operators which is half way through chapter 7, finishing on page 270. That's 27 pages of reading per week in a 4-credit class, which assumes 12 hours of outside work per week in addition to the 4 hours of class time. **27 pages over 16 hours** was the expected rate. When I took Analysis out of Rudin I was in grad school and we read the first 9 chapters over a 16-week semester, That's 244 pages (and we skipped a few non-essential sections). 15 pages per week was the expectation for a class of *PhD students* to cover the most fundamental concepts of analysis. There were times that I would spend a whole day working out a single page, often times with friends. 

You have to give each page, each definition, each example, each proposition and theorem, the time that it needs. Don't move on until you understand *exactly* what's going on. 

## Definitions

When you reach a new definition you're likely to encounter the format: *Definition*: a particular thing is a broad thing with property(ies) X. This declaration is followed shortly in most cases by some list of examples and non examples that elucidate the definition. After you read the definition, Immediately stop reading and grab your legal pad and consider (IN WRITING)
- Why is **THIS** the definition we care about? Sometimes you won't know this until later but make an honest attempt at figuring this out, often the author will provide some exposition immediately following the definition to clarify things like why tf you should care.
- What is it about property X that makes the particular thing special compared to the broad thing?
- What examples can I think of that satisfy the definition? 
- What are some non-examples?

Once you've spent some time struggling with these questions, it is time to start wrestling with the examples. Go one by one through the provided examples and prove to yourself that each one of them satisfies the definition. If the author gives you a bunch of examples it's likely because each one of them is instructive about the particular details captured in the definition or will be evocative cases that motivate later theorems.

Let me give you an example *Definition*:  a function $f :A \rightarrow B$ is 1 Injective if for any $a_1,a_2$ in A  If $f(a_1) = f(a_2)$ then $a_1 = a_2$. Examples :(1) $f(x) = x^3 $ is injective. (2) There are no injective functions $f:\lbrace a,b,c\rbrace \rightarrow \lbrace d,e \rbrace$  . 
Why this? 
- well a function is one to one if it sends each input to exactly 1 output. That's nice because if I can send elements of $B$ back to where they come from in A if I want (I get a weak notion of an inverse). 
- This property is the one I care about because it gives me a concrete test for injectivity, so If I'm ever in a position where I need to test that a function is injective, I have a tool to do it. 
- $f(x)=x$ is injective 
- $g(x) = x^2$ isn't (2 and -2 both map to 4 and 2 $\neq$ -2), but $g(x)$ is injective if my domain is defined to be $\mathbb{R}^+$. 
- in (1) every $x \in \mathbb{R}$ has exactly one cube root
- (2) a and b can map to unique elements but we run our of unique elements once we get to where c maps. 

## Propositions and Theorems
This is where the meat is. Propositions and Theorems are how we communicate facts about the objects we've defined. When armed with these facts, any time you are working with a new object but you know it fits a certain definition, you get all the facts you've proven about the general case for free. 

When reading past the definitions, each time you come to a proposition or a theorem, read the statement and stop immediately. Ask yourself these questions (answer them in writing). 
- Why is this property useful?
- What does it tell me about why the definition I just studied is important? 
- If the theorem applies to *particular thing*, why doesn't it hold for *broad thing*?
- How would I prove this?

A particular example -  *theorem*: if $f$ $A \rightarrow B$  is a linear transformation then $f$ is injective is and only if  $Ker(f) = \lbrace 0 \rbrace$.
why do I care
- This property is useful because it's sometimes hard to prove injectivity directly from the definition (mostly it's just annoying index chasing but still, I want to avoid the accounting when possible)
- We likely just learned about kernels, if the kernel determines whether the transformation is injective, then that's pretty darn important as a concept. Further more, this is telling me that where a linear transformation fails to be injective, it does so by hitting the origin more than once.
- why doesn't this apply to any old transformation? well some transformations have non-trivial kernel.
- the forward direction is simple, if f is injective then only 1 vector can map to the origin (0) so it will be the sole vector in the kernel. Going backwards, I would assume the kernel is only {0} then note that for $f(a_1) = f(a_2 ) \implies f(a_1-a_2) = 0$  so $a_1-a_2$ is in the kernel of $f$ and so must equal 0 by assumption and so $a_1=a_2$ . 

Give this process time. If you can't come up with a proof yourself after wrestling with it for an hour, that's OK, move on to reading the proof. You should read the proof slowly, understand why every line is true, understand how each line implies the next. Do not move on until you fully grok the proof. Come back tomorrow and try to re-produce the proof.

## 'Left as an exercise to the reader' is not a suggestion
Rudin, Axler, Ross, Munkers, Dummit and/or Foote, Papadimitriou, and the authors of every other math text book under the sun have at least one thing in common. THEY WERE NOT LAZY. They aren't leaving the exercise to the reader because they don't want to take the extra few mins it would take to write it. They left it as an exercise because there is some pedagogical value to proving that particular thing. 

## Do every single damn problem
You're self studying math to learn math. the only way to learn math is to do math. Do the math. If you skip the problems you're passing over the most important part of the process. If you're going to invest the time to learn, the INVEST THE TIME TO LEARN.

## Do them twice
Do it again to make sure it stuck.

## If you're not using the theorems and definitions from the chapter to do the problems, you're doing it wrong.

No one cares about some novel way you came up with to do a proof from Rudin without using the tooling he's presented. He posed the problem because it's instructive with respect to the tooling he's provided. Don't be so clever that you blow an opportunity to learn. The problems in higher math books aren't designed to torture calculus students with endless computation. the problems in the book are there to teach you the nuances of the content. 

# Concluding Remarks

I owe a great deal of this knowledge to my friend George who I met in undergrad. He was a grad student while I was getting my bachelors and he put me on game with alot of this. I've adapted his advice to come up with my approach and **you should do the same**. No two people learn in exactly the same way, but we're all similar enough that the advice above should at least give you a good starting point. 
