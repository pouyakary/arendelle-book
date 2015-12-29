# Spaces
Spaces are somehow the most important part of programming. In some languages like Assembly you will understand this however their actual name outside Arendelle is not spaces, but “Variables”. As I hate that name we have this much more pretty name “Space”.

<br><br>
## Why we call them space? What are they anyway?
Think of when someone asks: What is the 2 + 3?<br>

While the answer is obvious, the path you take to get into that answer has some points to think about how this thing actually happens in your mind?<br>

In your mind, you create a memory box called “the first number” and then another box with the name “the second number”. Now you put 2 in your first box and then 3 in your second box of memory.<br>

Now your mind creates a new memory box called “Result” and then it reads the 2 and 3 from those boxes, calculates the sum of them and then it creates the 5 and stores the 5 into the result box.<br>

This is the way that our minds memory works. And as the computer systems are based on our minds they have memory too! We can store data and well this is the definition of a computer: ***A device that does an operation based on instructions by the user on some data*** in this section we will learn how to work with datas.

<br><br>
## Computer memories
A space is a memory space in your computer’s temporary data storage called a ***RAM***, Just like the way our mind has two separated memories our computers got them too, This two memory systems are “Temporary Memory” and “Long-time Memory”. What are those? Well, the temporary memory is a small memory which is fast so when your system is thinking it uses that memory. This memory erases each time you shutdown your system. There is also another memory which stores your large amount of data as long as you want and those data stays there till you manually delete them. This memory is much slower than RAM but it can keep large data and those data remains there while your system is turned down. There are many different kinds of this memories but Hard Disk Drives and SSD (flash drives) are the most well-known.<br>

Till today you have used the long time memory for storing your files, applications, anything. But from now on you will learn how to use RAM to create your blueprints.

<br><br>
## Data
You have learned how to use sources in your blueprints. They are prepended with a hash ( `#` ) that represents data. Now spaces are like sources but they start with an `@` instead of `#` so a space name may looks like:<br>

<center>
<!-- ARENDELLE CODE BLOCK -->
<div style="font-family: Monospace;">
<span style="color:#000000"> <span style="color:#4E00FC">@space </span>    <span style="color:#4E00FC">@spaceName </span>    <span style="color:#4E00FC">@spaceNumber12</span><br><br>
</div>
<!-- ARENDELLE CODE BLOCK -->
</center>

The difference between space and source is a source is a data that your system gives you but space is a data that you enter its value, Now you should ask how can I create a space and then how can I add some data to it. Well, in Arendelle we have this rule:


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">(</span>&nbsp;spaceName&nbsp;<span style="color:#D60073">,</span>&nbsp;value&nbsp;<span style="color:#D60073">)</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
<br>

Now you may say what? Look at this examples:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">(</span>&nbsp;age&nbsp;<span style="color:#D60073">,</span>&nbsp;19&nbsp;<span style="color:#D60073">)</span>&nbsp;<br><span style="color:#D60073">(</span>&nbsp;year&nbsp;<span style="color:#D60073">,</span>&nbsp;2014&nbsp;<span style="color:#D60073">)</span>&nbsp;<br><span style="color:#D60073">(</span>&nbsp;size&nbsp;<span style="color:#D60073">,</span>&nbsp;42&nbsp;<span style="color:#D60073">)</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
<br>

Now as you see we have created a space with the name of @age and the value of 19 so `@age = 19` and then we have `@year = 2014` and then `@size = 42`.<br>

A good question is : “Why should I name a number and write something like ` [ @size , pr ] ` 	when I can write [ 19 , pr ]` well yes but now imagine this code:


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">[</span>&nbsp;5&nbsp;<span style="color:#D60073">,</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;5&nbsp;<span style="color:#D60073">,</span>&nbsp;pr&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;5&nbsp;<span style="color:#D60073">,</span>&nbsp;pd&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;5&nbsp;<span style="color:#D60073">,</span>&nbsp;pl&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;5&nbsp;<span style="color:#D60073">,</span>&nbsp;pu&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;<br><span style="color:#D60073">]</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
<br>

Now imagine you want to change the 5 to 10 you have to replace all the 5s, but you can write a code like this:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">(</span>&nbsp;number&nbsp;<span style="color:#D60073">,</span>&nbsp;10&nbsp;<span style="color:#D60073">)</span>&nbsp;<br><span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">@number</span>&nbsp;<span style="color:#D60073">,</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">@number</span>&nbsp;<span style="color:#D60073">,</span>&nbsp;pr&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">@number</span>&nbsp;<span style="color:#D60073">,</span>&nbsp;pd&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">@number</span>&nbsp;<span style="color:#D60073">,</span>&nbsp;pl&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">@number</span>&nbsp;<span style="color:#D60073">,</span>&nbsp;pu&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;<br><span style="color:#D60073">]</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
<br>

So now you want to change 10 to 1000 just all you need is to change the 10 in the `( number , 10 )`.

<br><br>
## Is that what sources are all about?
No! The whole point of spaces is this fact that you can edit the information inside them, Look at this code:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">(</span>&nbsp;space&nbsp;<span style="color:#D60073">,</span>&nbsp;12&nbsp;<span style="color:#D60073">)</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
<br>

As you see we have defined a space with the value of 12. If we write one more line like this :


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">(</span>&nbsp;space&nbsp;<span style="color:#D60073">,</span>&nbsp;12&nbsp;<span style="color:#D60073">)</span>&nbsp;<br><span style="color:#D60073">(</span>&nbsp;space&nbsp;<span style="color:#D60073">,</span>&nbsp;24&nbsp;<span style="color:#D60073">)</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
<br>

When Arendelle sees your code it first creates a space with the value of 12, Now in line 2, The we have created the space for second time! Is it possible? Hell yes! It’s not about creating the space for the second time! Once `@space` is defined the code: `( space , 24)` just changes the value of `@space`. <br>

You can even write mathematical expressions in the value side, Look at this:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">(</span>&nbsp;halfOfScreen&nbsp;<span style="color:#D60073">,</span>&nbsp;<span style="color:#4E00FC">#width</span>&nbsp;/&nbsp;2&nbsp;<span style="color:#D60073">)</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
<br>

You can use a spaces in expressions of course:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">(</span>&nbsp;spaceNo1&nbsp;<span style="color:#D60073">,</span>&nbsp;12&nbsp;<span style="color:#D60073">)</span>&nbsp;<br><span style="color:#D60073">(</span>&nbsp;spaceNo2&nbsp;<span style="color:#D60073">,</span>&nbsp;<span style="color:#4E00FC">@spaceNo1</span>&nbsp;+&nbsp;3&nbsp;<span style="color:#D60073">)</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
<br>

Now imagine you have created a space with value of 12 like this:


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">(</span>&nbsp;space&nbsp;<span style="color:#D60073">,</span>&nbsp;12&nbsp;<span style="color:#D60073">)</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
<br>

Now imagine you want to add 5 units to @space, you can change the current value using:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">(</span>&nbsp;space&nbsp;<span style="color:#D60073">,</span>&nbsp;12&nbsp;<span style="color:#D60073">)</span>&nbsp;<br><span style="color:#D60073">(</span>&nbsp;space&nbsp;<span style="color:#D60073">,</span>&nbsp;<span style="color:#4E00FC">@space</span>&nbsp;+&nbsp;5&nbsp;<span style="color:#D60073">)</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
<br>

So when Arendelle evaluates the code, It creates @space with the value of 12 and then when it’s going to run `( space , @space + 5 )` It first reads the `@space + 5` and as the `@space` is signed with `12` it changes the expression to `12 + 5`, After it evaluates the code it gives `17` back from the math engine and then changes the `@space` value to `17`.<br>

Now sometimes you want to add some numbers to your space like when you’re counting and you want to add one unit to the code, So you have to write :


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">(</span>&nbsp;space&nbsp;<span style="color:#D60073">,</span>&nbsp;<span style="color:#4E00FC">@space</span>&nbsp;+&nbsp;1&nbsp;<span style="color:#D60073">)</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
<br>

There are some shortcuts for this operations but Arendelle only comes with the five basic arithmetic operations :

```
+     -     /     *     ^    %
```

And to do so all you have to do is to write them with a Polish notation style as follows :


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">(</span>&nbsp;space&nbsp;<span style="color:#D60073">,</span>&nbsp;+&nbsp;5&nbsp;<span style="color:#D60073">)</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

And you should know the fact that :

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">(</span>&nbsp;space&nbsp;<span style="color:#D60073">,</span>&nbsp;+&nbsp;5&nbsp;<span style="color:#D60073">)</span>&nbsp;=&nbsp;<span style="color:#D60073">(</span>&nbsp;space&nbsp;<span style="color:#D60073">,</span>&nbsp;<span style="color:#4E00FC">@space</span>&nbsp;+&nbsp;5&nbsp;<span style="color:#D60073">)</span></pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

And so :

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">(</span>&nbsp;space&nbsp;<span style="color:#D60073">,</span>&nbsp;-&nbsp;5&nbsp;<span style="color:#D60073">)</span>&nbsp;=&nbsp;<span style="color:#D60073">(</span>&nbsp;space&nbsp;<span style="color:#D60073">,</span>&nbsp;<span style="color:#4E00FC">@space</span>&nbsp;-&nbsp;5&nbsp;<span style="color:#D60073">)</span><br><span style="color:#D60073">(</span>&nbsp;space&nbsp;<span style="color:#D60073">,</span>&nbsp;&nbsp;5&nbsp;<span style="color:#D60073">)</span>&nbsp;=&nbsp;<span style="color:#D60073">(</span>&nbsp;space&nbsp;<span style="color:#D60073">,</span>&nbsp;<span style="color:#4E00FC">@space</span>&nbsp;&nbsp;5&nbsp;<span style="color:#D60073">)</span><br><span style="color:#D60073">(</span>&nbsp;space&nbsp;<span style="color:#D60073">,</span>&nbsp;5&nbsp;<span style="color:#D60073">)</span>&nbsp;=&nbsp;<span style="color:#D60073">(</span>&nbsp;space&nbsp;<span style="color:#D60073">,</span>&nbsp;<span style="color:#4E00FC">@space</span>&nbsp;5&nbsp;<span style="color:#D60073">)</span><br><span style="color:#D60073">(</span>&nbsp;space&nbsp;<span style="color:#D60073">,</span>&nbsp;^&nbsp;5&nbsp;<span style="color:#D60073">)</span>&nbsp;=&nbsp;<span style="color:#D60073">(</span>&nbsp;space&nbsp;<span style="color:#D60073">,</span>&nbsp;<span style="color:#4E00FC">@space</span>&nbsp;^&nbsp;5&nbsp;<span style="color:#D60073">)</span></pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<br><br>
## Doing something with what we’ve learned
You still may don’t understand why you should have spaces and what you can do with them! Look at this image:

<center><br>
<img src="space2.png" style="box-shadow: 0px 0px 10px #888888; width:99%;"><img>
</center><br>

To go and create this thing you need to create random sized lines and how can you create a random number in Arendelle? We do the job using `#rnd` source. How? Each time you write a `#rnd` Arendelle generates a random number in format of `0.XXXXX` Like:

```
0.02343
0.34534
0.00835
0.65789
```

Now you may ask how to create a line with random size? All you need is to do :

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>
<div style="font-family: Monospace;">
<span style="color:#4E00FC">#rnd</span>&nbsp;*&nbsp;<span style="color:#4E00FC">#width</span>
</div>
<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

And this way you get a random number to draw a line with random size! Now to draw this image you have to first move to the right line but how can you remember the right line? There will be another solution and it’s when you draw a line you back to it’s first and then move to the next line. But in both ways we have a problem in the first one we need to know what line we are and in the second one we have to remember what random number we generated right? As you see this is possible to do it with a space look at this code :<br>

Way one:


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">(</span>&nbsp;line&nbsp;<span style="color:#D60073">,</span>&nbsp;0&nbsp;<span style="color:#D60073">)</span>&nbsp;<br><span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#height</span>&nbsp;<span style="color:#D60073">,</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;i<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">@line</span>&nbsp;<span style="color:#D60073">,</span>&nbsp;d&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#rnd</span>&nbsp;*&nbsp;<span style="color:#4E00FC">#width</span>&nbsp;<span style="color:#D60073">,</span>&nbsp;pr&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">(</span>&nbsp;line&nbsp;<span style="color:#D60073">,</span>&nbsp;+1&nbsp;<span style="color:#D60073">)</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;<br><span style="color:#D60073">]</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

Way two:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#height</span>&nbsp;<span style="color:#D60073">,</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">(</span>&nbsp;randomSize&nbsp;<span style="color:#D60073">,</span>&nbsp;<span style="color:#4E00FC">#rnd</span>&nbsp;*&nbsp;<span style="color:#4E00FC">#width</span>&nbsp;<span style="color:#D60073">)</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">@randomSize</span>&nbsp;<span style="color:#D60073">,</span>&nbsp;pr&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">@randomSize</span>&nbsp;<span style="color:#D60073">,</span>&nbsp;l&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;d<br>&nbsp;&nbsp;&nbsp;<br><span style="color:#D60073">]</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>


You can do so much magic with spaces! Look at this example:

<center><br>
<img src="snail.png" style="box-shadow: 0px 0px 10px #888888; width:99%;"><img>
</center><br>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#A0A0A0">//&nbsp;First&nbsp;spacings&nbsp;</span><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#i</span>&nbsp;/&nbsp;2&nbsp;<span style="color:#D60073">,</span>&nbsp;r&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#j</span>&nbsp;/&nbsp;2&nbsp;<span style="color:#D60073">,</span>&nbsp;d&nbsp;<span style="color:#D60073">]</span>&nbsp;<br><br><span style="color:#A0A0A0">//&nbsp;Starting&nbsp;dot&nbsp;</span><br>&nbsp;&nbsp;&nbsp;p<br><br><span style="color:#A0A0A0">//&nbsp;Level&nbsp;counter&nbsp;</span><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">(</span>&nbsp;level&nbsp;<span style="color:#D60073">,</span>&nbsp;2&nbsp;<span style="color:#D60073">)</span>&nbsp;<br><br><span style="color:#A0A0A0">//&nbsp;How&nbsp;many&nbsp;times?&nbsp;</span><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">(</span>&nbsp;times&nbsp;<span style="color:#D60073">,</span>&nbsp;<span style="color:#4E00FC">#j</span>&nbsp;/&nbsp;4&nbsp;<span style="color:#D60073">)</span>&nbsp;<br><br><span style="color:#A0A0A0">//&nbsp;Main&nbsp;body&nbsp;</span><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">@times</span>&nbsp;<span style="color:#D60073">,</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">@level</span>&nbsp;-&nbsp;1&nbsp;<span style="color:#D60073">,</span>&nbsp;rp&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">@level</span>&nbsp;<span style="color:#D60073">,</span>&nbsp;dp&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">(</span>&nbsp;level&nbsp;<span style="color:#D60073">,</span>&nbsp;+&nbsp;2&nbsp;<span style="color:#D60073">)</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">@level</span>&nbsp;-1&nbsp;<span style="color:#D60073">,</span>&nbsp;lp&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">@level</span>&nbsp;<span style="color:#D60073">,</span>&nbsp;up&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">(</span>&nbsp;level&nbsp;<span style="color:#D60073">,</span>&nbsp;+&nbsp;2&nbsp;<span style="color:#D60073">)</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">]</span>&nbsp;<br><br><span style="color:#A0A0A0">//&nbsp;Cleaning&nbsp;up&nbsp;</span><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">(</span>&nbsp;level&nbsp;<span style="color:#D60073">,</span>&nbsp;+&nbsp;2&nbsp;<span style="color:#D60073">)</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">@level</span>&nbsp;-1&nbsp;<span style="color:#D60073">,</span>&nbsp;rp&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;4&nbsp;<span style="color:#D60073">,</span>&nbsp;cl&nbsp;<span style="color:#D60073">]</span>&nbsp;<br><br><span style="color:#A0A0A0">//&nbsp;done&nbsp;</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

As you observed this blueprints are more advanced than what you have seen till now. Its like you get super hero powers when you use spaces!<br>

So now its time for you to practice!<br>

<br><br><hr>
<h4>Exercise</h4>
Okay let’s begin with something easy. Code the following image:

<center><br>
<img src="space1.png" style="box-shadow: 0px 0px 10px #888888; width:99%;"><img>
</center><br>

<hr>
