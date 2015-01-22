
<!-- Copyright 2014 Pouya Kary k@arendelle.org -->

# Conditions
Well their names says everything about them. Let me start this with an example: You're telling someone to choose cloths and you say "If you want to wear a black t-shirt you obviously need a blue Jeans but if you're going to wear a tux you should wear it with it's own pants" conditions are just like that. If something happened or if someone did something then do something. Conditions in Arendelle are like this:


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">{</span>&nbsp;Condition&nbsp;<span style="color:#D60073">,</span>&nbsp;Code&nbsp;<span style="color:#D60073">}</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>


If condition happens then the Arendelle runs the code but and else way nothing happens.

<br><br><hr>
<h4>Example</h4>

Look at this code:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">{</span>&nbsp;1&nbsp;=&nbsp;1&nbsp;<span style="color:#D60073">,</span>&nbsp;p&nbsp;<span style="color:#D60073">}</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

It's most obvious that 1 is equal to itself so when Arendelle sees that the equations is true it runs the `p` code:
<hr>
<h4>Example</h4>


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">{</span>&nbsp;1&nbsp;<span style="color:#D60073"><</span>&nbsp;2&nbsp;<span style="color:#D60073">,</span>&nbsp;p&nbsp;<span style="color:#D60073">}</span></pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

Because the 1 is less than 2 Arendelle runs the code:

<hr>
<h4>Example</h4>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">{</span>&nbsp;1&nbsp;=&nbsp;10&nbsp;<span style="color:#D60073">,</span>&nbsp;p&nbsp;<span style="color:#D60073">}</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

Well 1 is to equals to 10 so Arendelle never runs the code.
<hr><br><br>

<br><br>
## How to write a condition
You may ask what are other other condition operators? There are few of them:

| operators 	| What they does				|
|:--------------|:------------------------------|
| `=` or `==`	| Equals to						|
| `!=`			| Not equals 					|
| `>`			| Greater than					|
| `<`			| Less than						|
| `>=`			| Greater than or equals to 	|
| `<=`			| Less than or equals  			|

You may ask why there is `==` available!? As my opinion it's one of the most funny things about programming. Have you seen *Spy Kids 2* movie? There is a watch in the movie that has more than 10000 but it can tell you the time because developers were so buzzy creating all those functions and they forget to write a clock for the watch! There is the same story in programming. In other languages programmers chose `=` to be the operator for defining a variable (no rush we will learn what is a variable) and when it came the time to build conditions they just remembered they have to find a new replacement for `=` because it was token! So they created `==` instead of `=` to make conditions possible! To take care for programmers who used `==` there are two ways for `Equals to` in Arendelle.

<br><br><hr>
<h4>Example</h4>
`!=` means if the equation was `false` do something so look at the following code:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">{</span>&nbsp;1&nbsp;<span style="color:#D60073">!</span>=&nbsp;2&nbsp;<span style="color:#D60073">,</span>&nbsp;p&nbsp;<span style="color:#D60073">}</span></pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

Arendelle read your code and because 1 is not equals to 2 it runs the code.
<hr><br><br>
Also there is something very fun about not using any operators for example:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">{</span>&nbsp;2458&nbsp;<span style="color:#D60073">,</span>&nbsp;p&nbsp;<span style="color:#D60073">}</span></pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

I said condition, condition is about being `true` and `false`. If something is not `false` then it's surely `true` so do you think that 2458 is `false`. You may say: "It's a number! How can a number be false?" and you're right so what that is not `false` is `true`! When Arendelle reads your code it passes the number as `true` and it evaluates the code.<br>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">{</span>&nbsp;1&nbsp;=&nbsp;1&nbsp;<span style="color:#D60073">,</span>&nbsp;p&nbsp;<span style="color:#D60073">}</span><br><span style="color:#D60073">{</span>&nbsp;1&nbsp;=&nbsp;2&nbsp;<span style="color:#D60073">,</span>&nbsp;p&nbsp;<span style="color:#D60073">}</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
<br><br>



<h2>And / Or operators</h2>

`And` and `Or` are what we use to handle multi conditions for example look at the code below:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">{</span>&nbsp;1&nbsp;=&nbsp;1&nbsp;and&nbsp;2&nbsp;<span style="color:#D60073">></span>&nbsp;1&nbsp;<span style="color:#D60073">,</span>&nbsp;p&nbsp;<span style="color:#D60073">}</span></pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
<br>

As you see there are two equations `1 = 1` and `2 > 1`, so when Arendelle reads them it evaluates them and finds out that they are both true. `And` operator says that both equations must be `true` and they are so Arendelle runs the code. Now look at the following code:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">{</span>&nbsp;1&nbsp;=&nbsp;2&nbsp;and&nbsp;1&nbsp;=&nbsp;1&nbsp;<span style="color:#D60073">,</span>&nbsp;p&nbsp;<span style="color:#D60073">}</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>


As you see because not both sides of the `and` are `true` Arendelle never runs the code, Meanwhile the `or` says at least one side of me must be true so for example :

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">{</span>&nbsp;1&nbsp;=&nbsp;2&nbsp;or&nbsp;1&nbsp;=&nbsp;1&nbsp;<span style="color:#D60073">,</span>&nbsp;p&nbsp;<span style="color:#D60073">}</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>


Runs because one side of the or is `true` but the following code never runs because there is no `true` in each side of the `or`:


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">{</span>&nbsp;1&nbsp;=&nbsp;2&nbsp;or&nbsp;1&nbsp;=&nbsp;1&nbsp;<span style="color:#D60073">,</span>&nbsp;p&nbsp;<span style="color:#D60073">}</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>


<br><br>

<h2>Else</h2>

The more complete rule of condition is:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">{</span>&nbsp;Condition&nbsp;<span style="color:#D60073">,</span><br><br>&nbsp;&nbsp;&nbsp;Code&nbsp;for&nbsp;when&nbsp;the&nbsp;condition&nbsp;is&nbsp;true<br>&nbsp;<br><span style="color:#D60073">,</span><br><br>&nbsp;&nbsp;&nbsp;Code&nbsp;for&nbsp;when&nbsp;the&nbsp;condition&nbsp;is&nbsp;false<br><br><span style="color:#D60073">}</span></pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

So as you see the grammar has a one optional part, So if the condition's answer be `true` Arendelle will run the second part of the grammar like the previews one but here's the new thing. If the condition's answer be `false` Arendelle will run the last part.

<br><br><hr>
<h4>Example</h4>
The fun thing about programming is to understand anything you can just try them! do you see this code:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">{</span>&nbsp;1&nbsp;=&nbsp;2&nbsp;<span style="color:#D60073">,</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;10&nbsp;<span style="color:#D60073">,</span>&nbsp;r&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;<br><span style="color:#D60073">}</span>&nbsp;p</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>


Because the condition is `true` you will see this image:

<center><br>
<img src="1.png" style="box-shadow: 0px 0px 10px #888888; width:99%;"><img>
</center><br>

Now look at this code :

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">{</span>&nbsp;1&nbsp;=&nbsp;1&nbsp;<span style="color:#D60073">,</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;10&nbsp;<span style="color:#D60073">,</span>&nbsp;r&nbsp;<span style="color:#D60073">]</span><br><span style="color:#D60073">,</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;5&nbsp;<span style="color:#D60073">,</span>&nbsp;d&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;<br><span style="color:#D60073">}</span>&nbsp;p</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>


Because the condition is `false` you will see this result:

<center><br>
<img src="2.png" style="box-shadow: 0px 0px 10px #888888; width:99%;"><img>
</center><br>

But when you add `else` to your condition you can say *What to do if the condition is true* and also *What to do if the condition is false* like this:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">{</span>&nbsp;1&nbsp;=&nbsp;1&nbsp;<span style="color:#D60073">,</span>&nbsp;rrr&nbsp;<span style="color:#D60073">,</span>&nbsp;ddd&nbsp;<span style="color:#D60073">}</span>&nbsp;p</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

Because the condition is not `true` Arendelle will run the code `ddd` and if the condition be `true` instead of `false` Arendelle will run `rrr` code. That is what else does

<hr><br><br>

<br><br>
<h2>New sources</h2>
Well you know `#width` and `#height` but it's time we go a little further and learn two awesome new sources `#x` and `#y`, As we said before Arendelle is a grid system something like a chess. In the we have a row of numbers from 1 to 8 and row of characters from A to H we use them to specify an exact place in chess like when we say: *Move the knight from G1 to F3*.<br>

Just like chess Arendelle uses this technique, Each dot in screen has an address comprised of two coordinates, The x-coordinate and y-coordinate. What are those? Look at this photo:


<br><br><center>
	![](https://raw.githubusercontent.com/pmkary/pmkary.github.io/master/GitHubWideImages/Arendelle/book/Coordinates.png)
</center><br>

Now what are `#x` and `#y` sources? They tell where is the pointer in the screen. for example look at this code we did together in the basics chapter:

```
rp rdp dp lp lp
```

If you run the code this will be the result in the coordinated screen:

<br><br><center>
	![](https://raw.githubusercontent.com/pmkary/pmkary.github.io/master/GitHubWideImages/Arendelle/book/coordinated-rprdpdplplp.png)
</center><br>

All codes begin from the origin ( `#x` = 0 and `#y` = 0 ) then in our code pointer moves right and then paints the `#x` = 1 and `#y` = 0, pointer then moves to right and then down and paints the `#x` = 2 and `#y` = 1 after that pointer goes down and paints the `#x` = 2 and `#y` = 2 so on till it finish on the lighter gray dot with address of `#x` = 0 and `#y` = 2:

<br><br><center>
	![](https://raw.githubusercontent.com/pmkary/pmkary.github.io/master/GitHubWideImages/Arendelle/book/coordinated-withlastdothighlighted-rprdpdplplp.png)
</center><br>

Now we can always use `#x` and `#y` to understand where we are. You may ask how can we actually use it? When look at this example!

<br><br><hr>
<h4>Example</h4>

Imagine we're going to paint the dots with these addresses:

- Dot 1 : `#x` = 3 and `#y` = 0
- Dot 2 : `#x` = 6 and `#y` = 0
- Dot 3 : `#x` = `#width` - 5 and `#y` = 0

As you see they are all in one line because their all `#y` coordinate is zero so we can create a code like this:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">[</span>&nbsp;3&nbsp;<span style="color:#D60073">,</span>&nbsp;r&nbsp;<span style="color:#D60073">]</span>&nbsp;p<br><span style="color:#D60073">[</span>&nbsp;3&nbsp;<span style="color:#D60073">,</span>&nbsp;r&nbsp;<span style="color:#D60073">]</span>&nbsp;p<br><span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#width</span>&nbsp;-&nbsp;11&nbsp;<span style="color:#D60073">,</span>&nbsp;r&nbsp;<span style="color:#D60073">]</span>&nbsp;p</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

And if you run the code you'll see it works fine:

<center><br>
<img src="3.png" style="box-shadow: 0px 0px 10px #888888; width:99%;"><img>
</center><br>

But you can write your code a bit more fun this way:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#width</span>&nbsp;<span style="color:#D60073">,</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">{</span>&nbsp;<span style="color:#4E00FC">#x</span>&nbsp;=&nbsp;3&nbsp;or&nbsp;<span style="color:#4E00FC">#x</span>&nbsp;=&nbsp;6&nbsp;or&nbsp;<span style="color:#4E00FC">#x</span>&nbsp;=&nbsp;<span style="color:#4E00FC">#width</span>&nbsp;-&nbsp;5&nbsp;<span style="color:#D60073">,</span>&nbsp;p&nbsp;<span style="color:#D60073">}</span>&nbsp;r<br>&nbsp;&nbsp;&nbsp;<br><span style="color:#D60073">]</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>


As you see the code moves the pointer to all the dots in the line with `#y` = 0 and then if `#x` was address of one of those 3 dots Arendelle paints that dot, Now look at this code's result:

<center><br>
<img src="3.png" style="box-shadow: 0px 0px 10px #888888; width:99%;"><img>
</center><br>

Results are same but the final code is much more readable to a human eye.

<hr><br><br>

<br><br>
<h2>What can we do with all this stuff?</h2>

That's a good question. In other languages conditions are the most used grammars but in Arendelle loops are the most used ones, However conditions are still in the second place. We will use them so much, Since you know everything about conditions we will start experimenting our knowledge.

<br><br><hr>
<h4>Example</h4>
As I said in the Hello World chapter you can show messages in Arendelle's title by writing them between two apostrophes like this:<br>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#BD00AD">'message'</span></pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

Now have you seen those apps that says you're screen size is too small for the software to run? Let's build one of those! If the screen be more than 50 we will get yes and if the screen be less than 50 we will get an error saying you're screen is too small:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">{</span>&nbsp;<span style="color:#4E00FC">#width</span>&nbsp;<span style="color:#D60073">></span>=&nbsp;50&nbsp;<span style="color:#D60073">,</span>&nbsp;<span style="color:#BD00AD">'Yes!'</span>&nbsp;<span style="color:#BD00AD">'ERROR: Screen width is too small'</span></pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
<hr><br><br>

Oh! You just wrote you're error message! wasn't it fun? I have coded too much for you today so let's continue by some field work!

<br><br><hr>
<h4>Exercise</h4>
Write a code with conditions to paint half of the first line like this (and remember to use a condition to do it!)

<center><br>
<img src="5.png" style="box-shadow: 0px 0px 10px #888888; width:99%;"><img>
</center><br>
<hr>

<br><br><hr>
<h4>Exercise</h4>
Create a script to check all the dots of the screen and then if their `#x` address was less than 11
and their `#y` address was less than 6 paint those dots like this:

<center><br>
<img src="6.png" style="box-shadow: 0px 0px 10px #888888; width:99%;"><img>
</center><br>

<hr><br><br>

Actually condition is so important and we are going to use them to do extra ordinary things do the last example because I'm going to show you something very very special in the next chapter!! We are going to create a Graphing Engine!!! You can show other people you created one in your first programming lessons!!!

<!-- Copyright 2014 Pouya Kary k@arendelle.org -->
