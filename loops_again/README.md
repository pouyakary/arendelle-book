# Loops again!
As you have seen and as the way I said, Loops are the most important part of the Arendelle language. When something is such important, it has to be powerful too. So the one thing that is true about loops is that they are designed to be smart and detect what you want. In order to create this goal we have created something very new called conditional loops<br>

In other programming languages loops divides into two major types: the "For" loop and the "While" loop. However Arendelle had only one loop which is called “Loop”! Arendelle itself detects what you wrote and operates the way you want. You really don’t have to worry about learning a new grammar!<br><br>

The idea of this loops are really simple. Look at this rule for the conditional loop:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">[</span>&nbsp;condition&nbsp;<span style="color:#D60073">,</span>&nbsp;code&nbsp;<span style="color:#D60073">]</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

What is that and what does it? Simple! In the simple loop you enter how many times you want it to do the job and it does the job for you like when you type:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">[</span>&nbsp;10&nbsp;<span style="color:#D60073">,</span>&nbsp;pr&nbsp;<span style="color:#D60073">]</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

A very classic code: painting and going right for 10 times. But in the conditional loop you create something that does the job for as long as the condition is true like:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">[</span>&nbsp;1=1&nbsp;<span style="color:#D60073">,</span>&nbsp;p&nbsp;<span style="color:#D60073">]</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

As its obvious to anyone anything is always equals to itself so `1=1` is always a true expression, So the code values for an infinity number of times! As long as your app is open and your system is plugged or it's charged the loop goes and goes and goes and goes and goes and... Actually, if everything be all right it never stops working! That is why we have the `e` command. `e` stands for `exit`. When your app reaches the `e` if  there be a while running it stops and you get out of it.

So as you see when you're running an infinity loop like `[ 1=1 , p ]` it evaluates for an infinity times which means if you write a code like this:


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">[</span>&nbsp;1=1&nbsp;<span style="color:#D60073">,</span>&nbsp;p&nbsp;<span style="color:#D60073">]</span>&nbsp;nrp</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

Because its an infinity loop you never see the next color because the as it's an infinity loop it never gets out of the loop so the `nrp` never actually evaluates but when you use the `e` command like this one:


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">[</span>&nbsp;1=1&nbsp;<span style="color:#D60073">,</span>&nbsp;<br><br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#A0A0A0">//&nbsp;some&nbsp;codes&nbsp;here&nbsp;</span><br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">{</span>&nbsp;1&nbsp;<span style="color:#D60073"><</span>&nbsp;2&nbsp;<span style="color:#D60073">,</span>&nbsp;e&nbsp;<span style="color:#D60073">}</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;<br><span style="color:#D60073">]</span><br><br><span style="color:#D60073">[</span>&nbsp;10&nbsp;<span style="color:#D60073">,</span>&nbsp;pr&nbsp;<span style="color:#D60073">]</span></pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

What you see here is that your code evaluates only once! Why? Because the code reaches the `e` command and gets out of the loop like this image:

<center><br>
<img src="img1.png" style="box-shadow: 0px 0px 10px #888888; width:99%;"><img>
</center><br>


So what have we learned? The conditional loop is a loop with a condition with it and we learned about infinity loops and the fact that you should never make fun of them because they are deadly!<br><br>

Now let’s focus on our conditional loops. Imagine you’re going to have a line in size of 10 which is one of my most favorite Arendelle codes. So we can write it like this:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">[</span>&nbsp;10&nbsp;<span style="color:#D60073">,</span>&nbsp;pr&nbsp;<span style="color:#D60073">]</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

It works awesome and if you remember in the conditions we could wrote a code like this to do the same thing:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#width</span>&nbsp;<span style="color:#D60073">,</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">{</span>&nbsp;<span style="color:#4E00FC">#x</span>&nbsp;<span style="color:#D60073"><</span>&nbsp;10&nbsp;<span style="color:#D60073">,</span>&nbsp;p&nbsp;<span style="color:#D60073">}</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;r<br>&nbsp;&nbsp;&nbsp;<br><span style="color:#D60073">]</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

And now in conditional loops we can write:


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#x</span>&nbsp;<span style="color:#D60073"><</span>&nbsp;10&nbsp;<span style="color:#D60073">,</span>&nbsp;pr&nbsp;<span style="color:#D60073">]</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

So I know what are you thinking of! You’re saying when there is `[ 10 , pr ]` why on earth should I even use something that complex? I know, well, (have you noticed how often I use well?). Well, yes that’s too complex and we just did it because we wanted to see how the conditional loops actually operates. However, we use them many of the times for some really cool things.
