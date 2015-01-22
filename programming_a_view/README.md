# Programming a View

This chapter is somehow an example for the functions chapter. In this chapter we will create a very simple world generator. As you have played with 2D games. There are always worlds. So let’s create world ourselves like this:<br><br>

<center><br>
<img src="world.png" style="box-shadow: 0px 0px 10px #888888; width:99%;"><img>
</center><br>


As you see in the image, our world has a surface, some trees, stars, and rock under it’s surface, So how to implement all of them? Let’s code!

<br><br><br>
## Where to start?
If you look closely you see **4** four different **layers**. The back layer is the **Stars**, and then **tress**, **ground** and the most front layer **rocks**. That’s why we start with stars. So we need a `!drawStars(number)` function. Let’s create it.

<br><br>
### !drawStars(number)
So our first function is `!drawStars(number)` this function draws `@number` times of stars so like `!drawStarts(20)` draws `20` stars, So we have to first implement the `@number` in our header and then set the color to `#n = 3` then print stars.

Something you should know is half of the screen is going to be under the *surface layer* so we don’t need to draw stars there. All we have to do is to draw stars for the half of the screen:

<!-- CLIFF HIGHLIGHTER 0.02 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073"><</span>&nbsp;number&nbsp;<span style="color:#D60073">></span><br><br><span style="color:#A0A0A0">//&nbsp;Setting&nbsp;#n&nbsp;to&nbsp;3</span><br>&nbsp;&nbsp;&nbsp;nnn<br><br><span style="color:#A0A0A0">//&nbsp;Printing&nbsp;50&nbsp;dots</span><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">@number</span>&nbsp;<span style="color:#D60073">,</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#i</span>&nbsp;&nbsp;<span style="color:#4E00FC">#rnd</span>&nbsp;<span style="color:#D60073">,</span>&nbsp;r&nbsp;<span style="color:#D60073">]</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#j</span>&nbsp;&nbsp;<span style="color:#4E00FC">#rnd</span>&nbsp;2&nbsp;<span style="color:#D60073">,</span>&nbsp;d&nbsp;<span style="color:#D60073">]</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;pi<br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">]</span><br><br><span style="color:#A0A0A0">//&nbsp;done</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.02 DEV GENERATED CODE BLOCK--><br>


Now what we need is to have a way to create trees…

<br><br>
### !drawTree()
So we need to create a few trees so we need to program a tree on a function and then use the func to have create trees as much as we need. A tree should look like this. And remember we need a long trunk for it because we will generate it with random heights and when we do so we need the trunk to be so long to still be covered by the surface. So a trunk will look like this:<br><br>

<center><br>
<img src="tree.png" style="box-shadow: 0px 0px 10px #888888; width:99%;"><img>
</center><br>


To create this tree we have to write this very simple function:<br><br>

<!-- CLIFF HIGHLIGHTER 0.02 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073"><</span><span style="color:#D60073">></span><br><span style="color:#D60073">[</span>&nbsp;3&nbsp;<span style="color:#D60073">,</span>&nbsp;rp&nbsp;<span style="color:#D60073">]</span>&nbsp;rd<br><br><span style="color:#D60073">[</span>&nbsp;3&nbsp;<span style="color:#D60073">,</span><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;5&nbsp;<span style="color:#D60073">,</span>&nbsp;pl&nbsp;<span style="color:#D60073">]</span><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;5&nbsp;<span style="color:#D60073">,</span>&nbsp;r&nbsp;<span style="color:#D60073">]</span><br>&nbsp;&nbsp;&nbsp;d<br><span style="color:#D60073">]</span><br><br><span style="color:#D60073">[</span>&nbsp;3&nbsp;<span style="color:#D60073">,</span>&nbsp;lp&nbsp;<span style="color:#D60073">]</span>&nbsp;r<br><span style="color:#D60073">[</span>&nbsp;20&nbsp;<span style="color:#D60073">,</span>&nbsp;pd&nbsp;<span style="color:#D60073">]</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.02 DEV GENERATED CODE BLOCK--><br>

So now that we have two of our functions ready let’s implement them to the our main blueprint. So I’ll name the main blueprint `world.arendelle` At the first of the app we will need maybe 50 stars so I start the file with this:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK-->
<div style="font-family: Monospace;">
<span style="color:#D60073">!drawStars</span><span style="color:#D60073">(</span>50<span style="color:#D60073">)</span>
</div>
<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK-->

And now I need to put random trees in the page. How can I do that? look at this:<br><br>

<center><br>
<img src="dotsSpacings.png" style="box-shadow: 0px 0px 10px #888888; width:99%;"><img>
</center><br>

Also we render them randomly between 1 to 7 dot in the height. So let’s look how my code does that:

<!-- CLIFF HIGHLIGHTER 0.02 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">!drawStars</span><span style="color:#D60073">(</span>50<span style="color:#D60073">)</span><br><br><span style="color:#A0A0A0">//&nbsp;Trees</span><br><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">(</span>&nbsp;spacing&nbsp;<span style="color:#D60073">,</span>&nbsp;0&nbsp;<span style="color:#D60073">)</span><br><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#i</span>&nbsp;3<span style="color:#D60073">,</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;i<br><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#A0A0A0">//&nbsp;we&nbsp;set&nbsp;a&nbsp;random&nbsp;color</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#rnd</span>&nbsp;&nbsp;4&nbsp;<span style="color:#D60073">,</span>&nbsp;n&nbsp;<span style="color:#D60073">]</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#A0A0A0">//&nbsp;random&nbsp;height</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;&nbsp;<span style="color:#D60073">(</span>&nbsp;<span style="color:#4E00FC">#rnd</span>&nbsp;&nbsp;-7&nbsp;<span style="color:#D60073">)</span>&nbsp;-&nbsp;5&nbsp;+&nbsp;<span style="color:#4E00FC">#j</span>&nbsp;2&nbsp;<span style="color:#D60073">,</span>&nbsp;d&nbsp;<span style="color:#D60073">]</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#A0A0A0">//&nbsp;and&nbsp;we&nbsp;keep&nbsp;where&nbsp;we&nbsp;are&nbsp;using</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#A0A0A0">//&nbsp;@spacing,&nbsp;This&nbsp;way&nbsp;we&nbsp;can&nbsp;count</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#A0A0A0">//&nbsp;how&nbsp;many&nbsp;6&nbsp;dot&nbsp;should&nbsp;we&nbsp;add</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">@spacing</span>&nbsp;<span style="color:#D60073">,</span>&nbsp;r&nbsp;<span style="color:#D60073">]</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">!drawTree</span>&nbsp;<span style="color:#D60073">(</span><span style="color:#D60073">)</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#A0A0A0">//&nbsp;6&nbsp;dot&nbsp;is&nbsp;not&nbsp;the&nbsp;real</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#A0A0A0">//&nbsp;displacement&nbsp;but&nbsp;the&nbsp;7&nbsp;is&nbsp;look</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#A0A0A0">//&nbsp;at&nbsp;the&nbsp;image&nbsp;and&nbsp;you&nbsp;see&nbsp;why</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">(</span>&nbsp;spacing&nbsp;<span style="color:#D60073">,</span>&nbsp;+&nbsp;7&nbsp;<span style="color:#D60073">)</span><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">]</span></pre>

<!-- CLIFF HIGHLIGHTER 0.02 DEV GENERATED CODE BLOCK--><br>

<br><br>
### !drawGround()
The ground is easy. We create some lines with a random difference in height like this:

<!-- CLIFF HIGHLIGHTER 0.02 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073"><</span><span style="color:#D60073">></span><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">(</span>&nbsp;col&nbsp;<span style="color:#D60073">,</span>&nbsp;0&nbsp;<span style="color:#D60073">)</span><br><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#n</span>&nbsp;<span style="color:#D60073">></span>&nbsp;0&nbsp;<span style="color:#D60073">,</span>&nbsp;n&nbsp;<span style="color:#D60073">]</span><br><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#i</span>&nbsp;<span style="color:#D60073">,</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;i&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">@col</span>&nbsp;<span style="color:#D60073">,</span>&nbsp;r&nbsp;<span style="color:#D60073">]</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#rnd</span>&nbsp;*&nbsp;5&nbsp;+&nbsp;<span style="color:#4E00FC">#j</span>&nbsp;2&nbsp;<span style="color:#D60073">,</span>&nbsp;d&nbsp;<span style="color:#D60073">]</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#j</span>&nbsp;<span style="color:#D60073">,</span>&nbsp;pd&nbsp;<span style="color:#D60073">]</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">(</span>&nbsp;col&nbsp;<span style="color:#D60073">,</span>&nbsp;+1&nbsp;<span style="color:#D60073">)</span><br><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">]</span><br><br>&nbsp;&nbsp;&nbsp;n</pre>

<!-- CLIFF HIGHLIGHTER 0.02 DEV GENERATED CODE BLOCK--><br>

<br><br>
### !drawRocks()
We have to put some random dots like the way we did it in the `!drawStart(number)` but this time the other half of the screen. So:

<!-- CLIFF HIGHLIGHTER 0.02 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073"><</span><span style="color:#D60073">></span><br><br><span style="color:#D60073">(</span>&nbsp;col&nbsp;<span style="color:#D60073">,</span>&nbsp;1&nbsp;<span style="color:#D60073">)</span><br><br><span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#width</span>&nbsp;3&nbsp;-&nbsp;1&nbsp;<span style="color:#D60073">,</span><br><br>&nbsp;&nbsp;&nbsp;i&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">@col</span>&nbsp;<span style="color:#D60073">,</span>&nbsp;r&nbsp;<span style="color:#D60073">]</span><br><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#j</span>&nbsp;2&nbsp;+&nbsp;6&nbsp;+&nbsp;<span style="color:#4E00FC">#rnd</span>&nbsp;&nbsp;4&nbsp;<span style="color:#D60073">,</span>&nbsp;d&nbsp;<span style="color:#D60073">]</span><br><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#rnd</span>&nbsp;&nbsp;10&nbsp;<span style="color:#D60073">,</span>&nbsp;d&nbsp;<span style="color:#D60073">]</span>&nbsp;p<br><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">(</span>&nbsp;col&nbsp;<span style="color:#D60073">,</span>&nbsp;+&nbsp;3&nbsp;+&nbsp;<span style="color:#4E00FC">#rnd</span>&nbsp;*&nbsp;2&nbsp;<span style="color:#D60073">)</span><br><br><span style="color:#D60073">]</span></pre>

<!-- CLIFF HIGHLIGHTER 0.02 DEV GENERATED CODE BLOCK--><br>

And we need to draw this rocks for quite a few times to be sure it happens cool so we add it to the main code with a loop: `[ 4 , !drawRocks() ]`

<br><br>
## And it’s done!
You see the app is ready! You should have this main blueprint by now:

<!-- CLIFF HIGHLIGHTER 0.02 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">!drawStars</span><span style="color:#D60073">(</span>50<span style="color:#D60073">)</span><br><br><span style="color:#A0A0A0">//&nbsp;Trees</span><br><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">(</span>&nbsp;spacing&nbsp;<span style="color:#D60073">,</span>&nbsp;0&nbsp;<span style="color:#D60073">)</span><br><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#i</span>&nbsp;3<span style="color:#D60073">,</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;i<br><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#A0A0A0">//&nbsp;we&nbsp;set&nbsp;a&nbsp;random&nbsp;color</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#rnd</span>&nbsp;&nbsp;4&nbsp;<span style="color:#D60073">,</span>&nbsp;n&nbsp;<span style="color:#D60073">]</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#A0A0A0">//&nbsp;random&nbsp;height</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;&nbsp;<span style="color:#D60073">(</span>&nbsp;<span style="color:#4E00FC">#rnd</span>&nbsp;&nbsp;-7&nbsp;<span style="color:#D60073">)</span>&nbsp;-&nbsp;5&nbsp;+&nbsp;<span style="color:#4E00FC">#j</span>&nbsp;2&nbsp;<span style="color:#D60073">,</span>&nbsp;d&nbsp;<span style="color:#D60073">]</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#A0A0A0">//&nbsp;and&nbsp;we&nbsp;keep&nbsp;where&nbsp;we&nbsp;are&nbsp;using</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#A0A0A0">//&nbsp;@spacing,&nbsp;This&nbsp;way&nbsp;we&nbsp;can&nbsp;count</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#A0A0A0">//&nbsp;how&nbsp;many&nbsp;6&nbsp;dot&nbsp;should&nbsp;we&nbsp;add</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">@spacing</span>&nbsp;<span style="color:#D60073">,</span>&nbsp;r&nbsp;<span style="color:#D60073">]</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">!drawTree</span>&nbsp;<span style="color:#D60073">(</span><span style="color:#D60073">)</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#A0A0A0">//&nbsp;6&nbsp;dot&nbsp;is&nbsp;not&nbsp;the&nbsp;real</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#A0A0A0">//&nbsp;displacement&nbsp;but&nbsp;the&nbsp;7&nbsp;is&nbsp;look</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#A0A0A0">//&nbsp;at&nbsp;the&nbsp;image&nbsp;and&nbsp;you&nbsp;see&nbsp;why</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#D60073">(</span>&nbsp;spacing&nbsp;<span style="color:#D60073">,</span>&nbsp;+&nbsp;7&nbsp;<span style="color:#D60073">)</span><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">]</span><br><br><span style="color:#A0A0A0">//&nbsp;Ground</span><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">!drawGround</span><span style="color:#D60073">(</span><span style="color:#D60073">)</span><br><br><span style="color:#A0A0A0">//&nbsp;Rocks</span><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;4&nbsp;<span style="color:#D60073">,</span>&nbsp;<span style="color:#D60073">!drawRocks</span><span style="color:#D60073">(</span><span style="color:#D60073">)</span>&nbsp;<span style="color:#D60073">]</span><br><br><span style="color:#A0A0A0">//&nbsp;done</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.02 DEV GENERATED CODE BLOCK--><br>

So run it and see your world!


<br><br><hr>
<h4>Exercise</h4>
Add functions to draw birds, clouds and a sun to the world!
<hr>

