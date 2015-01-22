
<!-- Copyright 2014 Pouya Kary k@arendelle.org -->

# Loops

## A bit of speech

Programming is based on 4 foundations: Variables, Grammars, Commands and Functions. We have learned about Arendelle commands

The commands you know are cool but you can only create *static* shapes with them. There is this very big difference between programming and creating static shapes, If we were doing so we had to call ourselves illustrator or something but why we say we're learning to become a programmer? I will tell you this secret in the next chapter for now I only tell you that commands with no grammars are no programs! Grammars are what makes our codes smart, efficient and soon enough you'll see they makes programming 'Possible'<br>

Just like in movies, At first each superhero is just an ordinary someone then after something so extraordinary they transfer into something amazing! Today I have magnificent news for you! You're about to become someone very interesting! The prophecy states that you're the one! The most talented, Most special, Most extraordinary 'Master' of Arendelle! And how I knew it? This chapter will start your transformation!


## Simple Loops

Ladies and gentlemen! We're about to meet the most important the the most well known grammar, part and signature of Arendelle, Please! Meet the great and only Loop!<br>

What is a loop? Well lets begin with something else... Imagine you're going to write the image below:

<center>
	![](https://raw.githubusercontent.com/pmkary/pmkary.github.io/master/GitHubWideImages/Arendelle/book/rrprrprrprrprrprrprrp.png)
</center>
<br>

You may end up with this code:

```
RRP RRP RRP RRP RRP RRP RRP
```

And you are all right! Now image if we wanted 200 of this dots! then we had to write `RRP` for 200 times! A wise man once said : "Holly mother of god!" then he invented loops! Loops are grammars that you write to **repeat** a code as much as you want! Isn't this idea brilliant? I know right? However! If you let me I'll talk hours about my love for loops so let's finally meet this loop, Loops are like this:

```
[ NUMBER , CODE ]
```

You write the loops with opening it with a `[` and then you write the number of how much repeat you want then you write a `,` to start writing the repeating code and then you finish the loop via one `]`. You have to do this for any other rules. Loops are codes two so you can use them just like other codes between them like `...command command loop command command...` at any place like `prp [10, d] p`.<br>

With the things we have learned about loops we can rewrite our previews code much more efficient like this:

```
[ 7 , RR P ]
```

And if you ever wanted what happened to the wise man? He wrote the `[ 200 , rrp ]` code in less than a second and his fella developers worshiped him for reset of his life, He got the girl and a happy ever after fairy tale!<br>

When you have loops you can do huge magics! for example in computers; displays thus the Arendelle lines are sequences of dots. To create a line we need to fill a part of the sequence:

```
[ 10 , P R ]
```

<center>
	![](https://raw.githubusercontent.com/pmkary/pmkary.github.io/master/GitHubWideImages/Arendelle/book/[10,pr].png)
</center>
<br>

And lets try this line:


```
[ 10 , P RD ]
```

<center>
	![](https://raw.githubusercontent.com/pmkary/pmkary.github.io/master/GitHubWideImages/Arendelle/book/[10,prd].png)
</center>
<br>

You see loops are very awesome!

<hr><h4>Exercise</h4>
Please write a `V` like the image bellow (Why V? well I was going to say because you'll need to use two loops and in the next example it helps us to see the big image however I'm going to say because of V for Vendetta!)

<center>
	![](https://raw.githubusercontent.com/pmkary/pmkary.github.io/master/GitHubWideImages/Arendelle/book/[7,prd][7,pru]p.png)
</center>

---

<br><br>

## Loops inside loops!
There are automobiles designed to move automobiles, There are trains for moving trains and in this one special case there is this one airplane that is designed to transfer NASA's space shuttle. Just like I said before the loop rule is:

```
[ NUMBER , CODE ]
```

The loop itself is a code! The rule says you can write codes in the loop so you can use loops in loops in loops in...! Just like the Inception movie where at last minutes Cobb and Ariadne goes to a dream inside a dream inside a dream inside a dream to find Fischer; You can do this with loops just like that! Look at this code:

```
[ NUMBER,

   [ NUMBER,

      [ NUMBER,

         [ NUMBER , CODE ]

      ]

   ]

]
```

I have teched Arendelle and programming in general to many people and all of them just like you asked "Why on Earth do I need loops inside loops?". Well we will write many loops inside loops! Pay attention to this one: Answer for the last exercise 'writing a V' :

```
[ 7 , PRD ] [ 7 , PRU ] P
```

Writing a V is something beautiful and you know what is more beautiful? Writing a W! Write it! Be fast! That's it...! Now are you done? I have my code; take a look:

```
[ 7 , PRD ] [ 7 , PRU ] [ 7 , PRD ] [ 7 , PRU ] P
```

<center>
	![](https://raw.githubusercontent.com/pmkary/pmkary.github.io/master/GitHubWideImages/Arendelle/book/[2,[7,prd][7,pru]]p.png)
</center>
<br>

It's a quite awesome code, It's fun and does the job but as you see there is a repeating part : `[ 7 , PRD ] [ 7 , PRU ]` in our code! What do we do when we find repeating things? Yes! We code them with loops:

```
[ 2 , [ 7 , PRD ] [ 7 , PRU ] ] P
```

Observe the code in any level you can, Do you see how pretty they are? Imagine if you were in the previews page and you were willing create this W! That could be a bad bad bad Idea! When I started Arendelle I created that 5 first commands and I wanted to play with so bad that I started creating my name! It took about 20 minutes and I wrote about 500 commands to do my job! At last I couldn't even read and understand my code.<br>

We wrote a good code with loops in a loop to illustrate W. That code was a beauty but from now on please write your codes in a file, You have learned how to run a file in Arendelle but if you don't know how; check out the first chapters. Or if you're using Arendelle Studio you don't need to because you can write multi line codes<br>

When we want to use grammars inside grammars we write them like this:

```
[ 2,

	[ 7 , PRD ]
	[ 7 , PRU ]

] P
```

Please try hard to stick to this style. Each language and each notation system has a style.Using a style makes your code natural and friendly to other developers while also makes it easier for other developers to read and for you to remember what did you when you're trying desperately 6 moths after you wrote your code!<br>

I believe we're done with basics of loops! Now the fun part is on: Playing a bit with the knowledge we have now!<br>

<hr><h4>Exercise</h4>
Write a rectangle with more than one line! It will be so much of fun!

<center>
	![](https://raw.githubusercontent.com/pmkary/pmkary.github.io/master/GitHubWideImages/Arendelle/book/%5B3,%5B20,pr%5D%5B20,l%5Dd%5D.png)
</center>

---

#### Exercise
Write a program for a line like this:

<center>
	![](https://raw.githubusercontent.com/pmkary/pmkary.github.io/master/GitHubWideImages/Arendelle/book/[5,[8,pr]d].png)
</center>

---

<!-- Copyright 2014 Pouya Kary k@arendelle.org -->
