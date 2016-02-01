# Loops

## A bit of speech

Programming is based on four foundations: Variables, Grammars, Commands and Functions. We have learned about Arendelle´s commands.<br>

The commands you know are cool but you can only create static shapes with them. There is this very big difference between programming and creating static shapes. If we are doing so we had to call ourselves illustrator or something but why we say we're learning to become a programmer? I will tell you this secret in the next chapter for now I only tell you that commands with no grammars are no programs! Grammars are what makes our codes smart, efficient and soon enough you'll see they makes programming 'possible'!<br>

Just like in movies: at first each superhero is just an ordinary someone. Then after something so extraordinary they transform into something amazing! Today I have magnificent news for you! You're about to become someone very interesting! The prophecy states that you're the one! The most talented, most special, most extraordinary **Master of Arendelle!** And how I knew it? Believe me I'm right! This chapter will start your transformation!

<br><br>
## Simple Loops
Ladies and gentlemen! We're about to meet the most important the the most well known grammar, part and signature of Arendelle. Meet the great and only Loop!<br>

What is a loop? Well lets begin with something else... Imagine you're going to write the image below:

<center><br>
<img src="rrprrprrprrprrprrprrp.png" style="box-shadow: 0px 0px 10px #888888; width:99%;"></img>
</center><br>

You may end up with this code: `rrp rrp rrp rrp rrp rrp rrp`. And you are all right! Now imagine if we wanted `200` of this dots! then we had to write `rrp` for `200` times! But programming should not be like punishments in school and so there are Loops. They are grammars that you write to repeat a code as much as you want! Isn't this idea brilliant? I know right? However! If you let me I'll talk hours about my love for loops so let's finally meet this loop, Loops are like this: `[ number , code ] `. You write the loops with opening it with a `[` and then you write the number of how much repeat you want. Then you write a `,` to start writing the repeating code. Finally, you finish the loop via one `]`. You have to do this for any other rules. Loops are codes too, so you can use them just like other codes between them like ...command command loop command command... at any place like `prp [10, d] p`.<br>

With the things we have learned about loops we can rewrite our previews code much more efficient like this: `[ 7 , rr p ]`.<br>

When you have loops you can do a lot of magic! For example to create a line which is actually a sequence of dots we write: `[ 10 , p r ]`

<center><br>
<img src="[10,pr].png" style="box-shadow: 0px 0px 10px #888888; width:99%;"><img>
</center><br>

And lets try this line: `[ 10 , p rd ]`

<center><br>
<img src="[10,prd].png" style="box-shadow: 0px 0px 10px #888888; width:99%;"><img>
</center><br>

You see loops are very awesome!

<hr>
#### Exercise
Please write a `V` like the image below (Why V? Well I was going to say because you'll need to use two loops and in the next example it helps us to see the big image. However, I'm going to say because of V for Vendetta!).

<center><br>
<img src="[7,prd][7,pru]p.png" style="box-shadow: 0px 0px 10px #888888; width:99%;"><img>
</center><br>
<hr><br><br><br>

<br><br>
## Loops inside loops!
There are automobiles designed to move automobiles, trains for moving trains and in this one special case there is this one airplane that is designed to transfer NASA's space shuttle. Just like I said before the loop rule is:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
<pre style="font-family: Monospace;">
<span style="color:#D60073">[</span>&nbsp;number&nbsp;<span style="color:#D60073">,</span>&nbsp;code&nbsp;<span style="color:#D60073">]</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br><br>

The loop itself is a code! The rule says you can write codes in the loop so you can use loops in loops in loops in...! Just like the Inception movie where at last minutes Cobb and Ariadne goes to a dream inside a dream inside a dream inside a dream to find Fischer. You can do this with loops just like that! Look at this code:



<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
<pre style="font-family: Monospace;">
<span style="color:#D60073">[</span>&nbsp;number&nbsp;<span style="color:#D60073">,</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;number&nbsp;<span style="color:#D60073">,</span><br>&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;number&nbsp;<span style="color:#D60073">,</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;number&nbsp;<span style="color:#D60073">,</span>&nbsp;code&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;<br><span style="color:#D60073">]</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
I have taught Arendelle and programming in general to many people and all of them just like you asked "Why on Earth do I need loops inside loops?". Well, we will write many loops inside loops! Pay attention to this one (Answer for the last exercise 'writing a V'):


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
<pre style="font-family: Monospace;">
<span style="color:#D60073">[</span>&nbsp;7&nbsp;<span style="color:#D60073">,</span>&nbsp;pru&nbsp;<span style="color:#D60073">]</span>&nbsp;<span style="color:#D60073">[</span>&nbsp;7&nbsp;<span style="color:#D60073">,</span>&nbsp;pru&nbsp;<span style="color:#D60073">]</span>&nbsp;p</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
Writing a V is something beautiful and you know what is more beautiful? Writing a W! Give it a shot! Be fast! That's it...! Now, are you done? I have my code! Take a look:


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
<pre style="font-family: Monospace;">
<span style="color:#D60073">[</span>&nbsp;7&nbsp;<span style="color:#D60073">,</span>&nbsp;prd&nbsp;<span style="color:#D60073">]</span>&nbsp;<span style="color:#D60073">[</span>&nbsp;7&nbsp;<span style="color:#D60073">,</span>&nbsp;pru&nbsp;<span style="color:#D60073">]</span>&nbsp;<br><span style="color:#D60073">[</span>&nbsp;7&nbsp;<span style="color:#D60073">,</span>&nbsp;prd&nbsp;<span style="color:#D60073">]</span>&nbsp;<span style="color:#D60073">[</span>&nbsp;7&nbsp;<span style="color:#D60073">,</span>&nbsp;pru&nbsp;<span style="color:#D60073">]</span>&nbsp;p<br></pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
<center><br>
<img src="[2,[7,prd][7,pru]]p.png" style="box-shadow: 0px 0px 10px #888888; width:99%;"><img>
</center><br>

It's a quite awesome code. It's fun and does the job but as you see there is a repeating part: `[ 7 , prd ] [ 7 , pru ]` in our code! What do we do when we find repeating things? Yes! We code them with loops: `[ 2 , [ 7 , prd ] [ 7 , pru ] ] p`. Observe the code in any level you can. Do you see how pretty they are? Imagine if you were in the previews page and you were willing create this W! That could be a bad bad bad idea! When I started Arendelle I created that five first commands and I wanted to play with so bad that I started creating my name! It took about 20 minutes and I wrote about `500` commands to do my job! At last I couldn't even read and understand my code.<br>

We wrote a good code with loops in a loop to illustrate W. That code was a beauty but from now on please write your codes in a file. You have learned how to run a file in Arendelle but if you don't know how, check out the first chapters. Or if you're using Arendelle Studio you don't need to because you can write multi line codes<br>

When we want to use grammars inside grammars we write them like this: `[ 2, [ 7 , prd ] [ 7 , pru ] ] p` Please try hard to stick to this style. Each language and each notation system has a style. Using a style makes your code natural and friendly to other developers while also making it easier for you to read and fremember what did you when you're trying desperately 6 months after you wrote your code!<br>

I believe we're done with basics of loops! Now the fun part is on: Playing a bit with the knowledge we have now!

<hr>
#### Exercise
Write a rectangle with more than one line! It will be so much of fun!

<center>
<img src="[3,[10,pr][10,l]d].png" style="box-shadow: 0px 0px 10px #888888; width:99%;"></img>
</center><br>

<hr>
#### Exercise
Write a program for a line like this:

<center>
<img src="[5,[8,pr]d].png" style="box-shadow: 0px 0px 10px #888888; width:99%;"></img>
</center><br>
<hr>
