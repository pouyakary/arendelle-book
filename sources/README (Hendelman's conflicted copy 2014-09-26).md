
<!-- Copyright 2014 Pouya Kary k@arendelle.org -->

# Sources

## A bit more of loops

What are resources? Before learning about resource, source, references or what ever me or others call them let's learn a bit more about our friend loop! Loop is a nice guy and I know him for such a long time, something very awesome about him is you never know all the things he is capable of because he's always full of surprises. Let's see a bit more of his tricks!<br>

Loop does many tasks, tasks that other languages has special grammars for each of them but the loop in Arendelle is smart enough to take care of all of them.<br>

One of those superhero powers of loop is he's very very good with math. I have to tell you a truth: I lied when I introduced you to the loop, Loop's actual rule is:

```
[ Mathematical Expression , Code ]
```

By mathematical expression I mean something like `2 * 3 + 1` it's my most favorite expression! An expression is a combination of numbers, arithmetic operators and functions. Numbers are fine and forget the functions now but let's talk about 'Arithmetic Operators'. Arendelle supports the basic ones:

| Operators  | Job              |
|:-----------|:-----------------|
| `+`        | Addition         |
| `-`        | Subtraction      |
| `*` or `×` | Multiplication   |
| `/` or `÷` | Division         |

Just for fun Arendelle supports `×` and `÷` characters but as we *CAN Not* type those characters Arendelle and every other language and calculator uses `*` and `/` instead. Now let's see what we can do, We can use them just the way we used numbers:

```
[ 2 * 3 + 1 , pr ]
```

And it works just perfect! Now enough with arithmetic operators, let's see what sources can do!

## The Sources
What are these sources we're talking about so much? For starter they do exactly what numbers does! You can divide them, add them to other numbers. And everything else a number does but what are them seriously?<br>

Imagine you're going to write a software (actual, serious software) and many people with many different systems are dieing to get their hands on it. Your software's job is to create a line in size of your screen's width like this:

<center>
	![](https://raw.githubusercontent.com/pmkary/pmkary.github.io/master/GitHubWideImages/Arendelle/book/%5B%23width,pr%5D.png)
</center>

To do so you can launch your Arendelle tool and it always says what your screen size is that most of the times it's 80, Then your awesome record breaking software will be:

```
[ 80 , pr ]
```

Well it's good if screen size be 80 in any possible device but unfortunately they are not! And worse in our case is that others can change their window's screen size. So if they do so our software still make an 80 dot line... BOOM!!! As the first person finds out the software's bug the software makes it to the top of the news on every single channel and everyone will know how bad is the bug! Soon people will remove the app!!! What an unfortunate mistake<br>

That's bad and it's obvious that no one wants that! We don't exactly know who but there was a very gifted man who could see the future. He knew we're going to fail to write that software so he invented a very mysterious tool! It's obvious! That was the Sources! Actually they were not sources, I created sources, But there was this idea that invented that day and it was creating something like a word that represents screen size or something else like that<br>

As in algebra you write words and read them as numbers like when you say let `x` be 2 and then you can use `x` as 2 and write `x + 5 = 7`. Sources are just and exactly like them!<BR>

Sources are words or sometimes characters that comes with an `#` (Octothorpe) in their start  so something like `#source` can be a source but some stuff like `source` or `#    source` can not. These words we write represent an actual number like the screen size.<br>

Arendelle reads your expressions and if it finds any source it replaces them with the data they are representing, for example we have a source for screen width witch is `#width`, By using it on our previews software we'll have something like this:

```
[ #width , pr ]
```

Arendelle reads the code and then when it finds the `#width` checks what the screen size is and then replaces it with the `#width` so if the screen width be 80 what you type will be:

```
[ #width , pr ]
```

But to Arendelle it actually is:

```
[ 80 , pr ]
```

We know what sources are, we know what they do and we know how to use them. You may expect me to tell you the list of all sources but it's not good for you! We only go with one or two at the time so you can practice and discover all the possibilities. I said what `#width` is and now I'm going to introduce you `#width` and `#height`. Pay attention to this table:

| Name 				| What it does															|
|:------------------|:----------------------------------------------------------------------|
| `#width` or `#i`	| Returns the screen width, You can use `#i` if you're lazy like me 	|
| `#height` or `#j`	| Returns the screen height, You can use `#j` if you're lazy like me 	|

As I said before Arendelle looks at sources just like numbers and that's why you can apply all the arithmetic operations on them. Imagine a line in size of half of the screen width, You can use this code:

```
[ #width / 2 , pr ]
```

You want to fill all the screen? this will be a good code:

```
[ #height / 2 ,

   [ #width  , pr ] d
   [ #height , lp ] d

]
```

---

#### Exercise
Pick up a one of those notebooks with grid papers and then try to interpret this code. Remember you can always run the code on your system but it's much better if you first do the exercise and then run the code to see if you did it right, So let's do this!

```
[ #width / #height + 1 ,

   [ #height - 1 , prd ]
   [ #height - 1 , pru ]

]
```

---

## Meet a new commands
There is a cool command called inception commands represented with an `i`. Inception is where something starts so as the pointer. When you write inception command the pointer moves to the very first place it was the starting of the software the very left top dot. Look at this code for example:

```
[ 10 , pr ]
[ 10 , pd ]
```

<center>
	![](https://raw.githubusercontent.com/pmkary/pmkary.github.io/master/GitHubWideImages/Arendelle/book/%5B10,pr%5D%5B10,pd%5D.png)
</center>

Now try this one and see what happens when you use an `i`:

```
[ 10 , pr ] i
[ 10 , pd ]
```

<center>
	![](https://raw.githubusercontent.com/pmkary/pmkary.github.io/master/GitHubWideImages/Arendelle/book/%5B10,pr%5Di%5B10,pd%5D.png)
</center>

See how fun is that? you get back to the first place! Inception is the only jump you have in Arendelle, With the inception command we can do many magics look at this one:

```
[ 10 , pr    ] i
[ 5  , pd    ] i
[ 5  , prprd ] i
[ 5  , prd   ]
```

<center>
	![](https://raw.githubusercontent.com/pmkary/pmkary.github.io/master/GitHubWideImages/Arendelle/book/%5B10,pr%5Di%5B5,pd%5Di%5B5,prprd%5Di%5B5,prd%5D.png)
</center>

---

#### Exercise
Are you asking why did I taught you inception in middle of sources? Well because I wanted you to write the for this sketch, We have written codes like this but this one is a bit more trickier:

<center>
	![](https://raw.githubusercontent.com/pmkary/pmkary.github.io/master/GitHubWideImages/Arendelle/book/%5B%23width%C3%B7%23height+1,%5B%23height-1,prd%5D%5B%23height-1,pru%5D%5Di%5B%23height-1,d%5D%5B%23width%C3%B7%23height+1,%5B%23height-1,pru%5D%5B%23height-1,prd%5D%5D.png)
</center>

---


<!-- Copyright 2014 Pouya Kary k@arendelle.org -->
