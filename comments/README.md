# Comments
Okay what are comments? Its sure that they are not what we post and like on social networks. Its also not what we “comment” about someone’s opinion or attitude or so… In the real programming-life they are not even comments!<br>

<br><br>
## What is this “comment” thing anyway?
Good question! Well, in programming comments are what we use to explain how our code works. Comments are some texts you write inside your code so when someone is reading the code, the code be easy to understand. Look at this code for example:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#i</span>&nbsp;/&nbsp;2&nbsp;-&nbsp;8&nbsp;<span style="color:#D60073">,</span>&nbsp;r&nbsp;<span style="color:#D60073">]</span>&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#j</span>&nbsp;/&nbsp;2&nbsp;-&nbsp;4&nbsp;<span style="color:#D60073">,</span>&nbsp;d&nbsp;<span style="color:#D60073">]</span><br><span style="color:#D60073">[</span>&nbsp;3&nbsp;<span style="color:#D60073">,</span>&nbsp;rp&nbsp;<span style="color:#D60073">]</span>&nbsp;d&nbsp;<span style="color:#D60073">[</span>&nbsp;3&nbsp;<span style="color:#D60073">,</span>&nbsp;l&nbsp;<span style="color:#D60073">]</span>&nbsp;p&nbsp;rp&nbsp;rr&nbsp;p&nbsp;d&nbsp;p<br><span style="color:#D60073">[</span>&nbsp;2&nbsp;<span style="color:#D60073">,</span>&nbsp;lp&nbsp;<span style="color:#D60073">]</span>&nbsp;d&nbsp;p&nbsp;<span style="color:#D60073">[</span>&nbsp;3&nbsp;<span style="color:#D60073">,</span>&nbsp;rp&nbsp;<span style="color:#D60073">]</span>&nbsp;d&nbsp;<span style="color:#D60073">[</span>&nbsp;4&nbsp;<span style="color:#D60073">,</span>&nbsp;l&nbsp;<span style="color:#D60073">]</span><br><span style="color:#D60073">[</span>&nbsp;7&nbsp;<span style="color:#D60073">,</span>&nbsp;rp&nbsp;<span style="color:#D60073">]</span>&nbsp;d&nbsp;<span style="color:#D60073">[</span>&nbsp;6&nbsp;<span style="color:#D60073">,</span>&nbsp;lp&nbsp;<span style="color:#D60073">]</span>&nbsp;d&nbsp;p&nbsp;<span style="color:#D60073">[</span>&nbsp;3&nbsp;<span style="color:#D60073">,</span>&nbsp;rp&nbsp;<span style="color:#D60073">]</span><br>d&nbsp;ll&nbsp;p</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

What it is and what it does are two really hard problems to solve. So what it is? Actually, it is the code for the Arendelle’s Logo “Birdy”. But it’s really hard to read, right? That’s why we use comments! Arendelle has two kinds of comments. They are the only thing Arendelle uses from another language. Arendelle uses the C style comments. First is what we call in Arendelle **slash-slash** comment. An slash-slash comment starts with two slashes “slash-slash!” like this:


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#A0A0A0">//&nbsp;comment&nbsp;</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

What ever that is in the right side of the slashes till the end of the line will be ignored by Arendelle. So if you write a code like this:


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
p&nbsp;<span style="color:#A0A0A0">//&nbsp;rp&nbsp;</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

You will only see one dot, not two dots because Arendelle ignores what’s after the slashes and it reads the code like this:

```
p
```

No more `// rp` - We use slash-slash comments for one-line comments which we use to explain what’s happening in the next line. Look at this code for example:


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#A0A0A0">//&nbsp;This&nbsp;line&nbsp;goes&nbsp;to&nbsp;#x&nbsp;=&nbsp;4&nbsp;and&nbsp;#y&nbsp;=&nbsp;4:&nbsp;</span><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;5&nbsp;<span style="color:#D60073">,</span>&nbsp;rd&nbsp;<span style="color:#D60073">]</span>&nbsp;<br><br><span style="color:#A0A0A0">//&nbsp;This&nbsp;line&nbsp;paints&nbsp;the&nbsp;dot&nbsp;with&nbsp;#x&nbsp;,&nbsp;#y&nbsp;of&nbsp;4:&nbsp;</span><br>&nbsp;&nbsp;&nbsp;p</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

Now let’s see how the Birdy’s code will look like if we add comments:


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#A0A0A0">//&nbsp;First&nbsp;Spacings&nbsp;</span><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#i</span>&nbsp;/&nbsp;2&nbsp;-&nbsp;8&nbsp;<span style="color:#D60073">,</span>&nbsp;r&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#j</span>&nbsp;/&nbsp;2&nbsp;-&nbsp;4&nbsp;<span style="color:#D60073">,</span>&nbsp;d&nbsp;<span style="color:#D60073">]</span>&nbsp;<br><br><span style="color:#A0A0A0">//&nbsp;Line&nbsp;1&nbsp;</span><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;3&nbsp;<span style="color:#D60073">,</span>&nbsp;rp&nbsp;<span style="color:#D60073">]</span>&nbsp;<br><br><span style="color:#A0A0A0">//&nbsp;Line&nbsp;2&nbsp;</span><br>&nbsp;&nbsp;&nbsp;d&nbsp;<span style="color:#D60073">[</span>&nbsp;3&nbsp;<span style="color:#D60073">,</span>&nbsp;l&nbsp;<span style="color:#D60073">]</span>&nbsp;prprrp<br><br><span style="color:#A0A0A0">//&nbsp;Line&nbsp;3&nbsp;</span><br>&nbsp;&nbsp;&nbsp;dp&nbsp;<span style="color:#D60073">[</span>&nbsp;2&nbsp;<span style="color:#D60073">,</span>&nbsp;lp&nbsp;<span style="color:#D60073">]</span>&nbsp;<br><br><span style="color:#A0A0A0">//&nbsp;Line&nbsp;4&nbsp;</span><br>&nbsp;&nbsp;&nbsp;dp&nbsp;<span style="color:#D60073">[</span>&nbsp;3&nbsp;<span style="color:#D60073">,</span>&nbsp;rp&nbsp;<span style="color:#D60073">]</span>&nbsp;<br><br><span style="color:#A0A0A0">//&nbsp;Line&nbsp;5&nbsp;</span><br>&nbsp;&nbsp;&nbsp;d&nbsp;<span style="color:#D60073">[</span>&nbsp;4&nbsp;<span style="color:#D60073">,</span>&nbsp;l&nbsp;<span style="color:#D60073">]</span>&nbsp;<span style="color:#D60073">[</span>&nbsp;7&nbsp;<span style="color:#D60073">,</span>&nbsp;rp&nbsp;<span style="color:#D60073">]</span>&nbsp;<br><br><span style="color:#A0A0A0">//&nbsp;Line&nbsp;6&nbsp;</span><br>&nbsp;&nbsp;&nbsp;d&nbsp;<span style="color:#D60073">[</span>&nbsp;6&nbsp;<span style="color:#D60073">,</span>&nbsp;lp&nbsp;<span style="color:#D60073">]</span>&nbsp;<br><br><span style="color:#A0A0A0">//&nbsp;Line&nbsp;7&nbsp;</span><br>&nbsp;&nbsp;&nbsp;dp&nbsp;<span style="color:#D60073">[</span>&nbsp;3&nbsp;<span style="color:#D60073">,</span>&nbsp;rp&nbsp;<span style="color:#D60073">]</span>&nbsp;<br><br><span style="color:#A0A0A0">//&nbsp;Line&nbsp;8&nbsp;</span><br>&nbsp;&nbsp;&nbsp;dllp</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

You see how more clear is the code when you add comments to it? You now can see that as Birdy has 8 rows of dots you can divide the code to 8 lines and then simply write each line and name it. Now if you want to edit line 6 you know where you have to edit.

<br><br>
## Multi Line Comment
In the C way, We have this other comment which people know it as “Multi Line Comment” and in Arendelle we call it slash-star comment. This comment starts with a `/*` ( slash-star ) and ends with a `*/` ( star-slash ) what ever you write between two these two `/*` and `*/` elements will be easily ignored. so the code like this:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
p&nbsp;<span style="color:#A0A0A0">/*&nbsp;[&nbsp;10&nbsp;,&nbsp;r&nbsp;]&nbsp;*/</span>&nbsp;rp</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

Will result two connected dots, not two dots with 11 dots distance because what Arendelle see is this:

```
prp
```

Nothing more. However there is a common culture about using slash-star comments in the multi line star which is this: When you write a multi line comment. You may write it like this:

```
/* line 1
line 2
line 3 */
```

But as you see it’s really ugly! That’s why developers use this style for a multi line comment:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#A0A0A0">/*<br>&nbsp;&#42;&nbsp;&nbsp;&nbsp;line&nbsp;1<br>&nbsp;&#42;&nbsp;&nbsp;&nbsp;line&nbsp;2<br>&nbsp;&#42;&nbsp;&nbsp;&nbsp;line&nbsp;3<br>&nbsp;*/</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

Remember to keep asterisks in a line. So as you see this kind of comments are very pretty in multi line. So look at this example:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#A0A0A0">/*<br>&nbsp;&#42;&nbsp;&nbsp;Copyright&nbsp;2014&nbsp;Pouya&nbsp;Kary&nbsp;k@arendelle.org&nbsp;<br>&nbsp;&#42;&nbsp;&nbsp;This&nbsp;sketch&nbsp;generates&nbsp;a&nbsp;a&nbsp;simple&nbsp;star&nbsp;for&nbsp;you<br>&nbsp;*/</span>&nbsp;</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

**NOTE : ** Many people like me prefers to use only slash-slash comments. So it’s obvious that you can use them to also write multi line comments line this:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#A0A0A0">//&nbsp;Copyright&nbsp;2014&nbsp;Pouya&nbsp;Kary&nbsp;k@arendelle.org&nbsp;</span><br><span style="color:#A0A0A0">//&nbsp;This&nbsp;sketch&nbsp;generates&nbsp;a&nbsp;a&nbsp;simple&nbsp;star&nbsp;for&nbsp;you&nbsp;</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<br><br>
## Copyright in Your App
In almost any programming system we write one or a few lines of comment in the start of our app. Explaining the copyright. We also name the developer and we share our emails so if someone wanted to report a problem, or share a bugfix, or a code patch to use find us easily. For example this is a starting comment in Apple’s Swift Language:


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#A0A0A0">//&nbsp;Copyright&nbsp;year&nbsp;firstName&nbsp;lastName&nbsp;</span><br><span style="color:#A0A0A0">//&nbsp;one&nbsp;line&nbsp;that&nbsp;explains&nbsp;the&nbsp;code&nbsp;</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

As you see it’s a very good starting comment. It says what is the copyright, when the last edit was and what file and project this code is. <br><br>

In Arendelle we have our own way. This is the template of our starting:


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#A0A0A0">//&nbsp;Copyright&nbsp;year&nbsp;firstName&nbsp;lastName&nbsp;</span><br><span style="color:#A0A0A0">//&nbsp;one&nbsp;line&nbsp;that&nbsp;explains&nbsp;the&nbsp;code&nbsp;</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

For example:

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#A0A0A0">//&nbsp;Copyright&nbsp;2014&nbsp;Pouya&nbsp;Kary&nbsp;k@arendelle.org&nbsp;</span><br><span style="color:#A0A0A0">//&nbsp;Birdy&nbsp;-&nbsp;Arendelle’s&nbsp;Logo&nbsp;</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

Okay. Let’s look at a real Arendelle app’s code:


<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#A0A0A0">//&nbsp;Copyright&nbsp;2014&nbsp;Pouya&nbsp;Kary&nbsp;k@arendelle.org&nbsp;</span><br><span style="color:#A0A0A0">//&nbsp;Birdy&nbsp;-&nbsp;Arendelle’s&nbsp;cute&nbsp;logo!&nbsp;</span><br><br><span style="color:#A0A0A0">//&nbsp;First&nbsp;Spacings&nbsp;</span><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#i</span>&nbsp;/&nbsp;2&nbsp;-&nbsp;8&nbsp;<span style="color:#D60073">,</span>&nbsp;r&nbsp;<span style="color:#D60073">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;<span style="color:#4E00FC">#j</span>&nbsp;/&nbsp;2&nbsp;-&nbsp;4&nbsp;<span style="color:#D60073">,</span>&nbsp;d&nbsp;<span style="color:#D60073">]</span>&nbsp;<br><br><span style="color:#A0A0A0">//&nbsp;Line&nbsp;1&nbsp;</span><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;3&nbsp;<span style="color:#D60073">,</span>&nbsp;rp&nbsp;<span style="color:#D60073">]</span>&nbsp;<br><br><span style="color:#A0A0A0">//&nbsp;Line&nbsp;2&nbsp;</span><br>&nbsp;&nbsp;&nbsp;d&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;3&nbsp;<span style="color:#D60073">,</span>&nbsp;l&nbsp;<span style="color:#D60073">]</span>&nbsp;&nbsp;prprrp<br><br><span style="color:#A0A0A0">//&nbsp;Line&nbsp;3&nbsp;</span><br>&nbsp;&nbsp;&nbsp;dp&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;2&nbsp;<span style="color:#D60073">,</span>&nbsp;lp&nbsp;<span style="color:#D60073">]</span>&nbsp;<br><br><span style="color:#A0A0A0">//&nbsp;Line&nbsp;4&nbsp;</span><br>&nbsp;&nbsp;&nbsp;dp&nbsp;<span style="color:#D60073">[</span>&nbsp;3&nbsp;<span style="color:#D60073">,</span>&nbsp;rp&nbsp;<span style="color:#D60073">]</span>&nbsp;<br><br><span style="color:#A0A0A0">//&nbsp;Line&nbsp;5&nbsp;</span><br>&nbsp;&nbsp;&nbsp;d&nbsp;<span style="color:#D60073">[</span>&nbsp;4&nbsp;<span style="color:#D60073">,</span>&nbsp;l&nbsp;<span style="color:#D60073">]</span>&nbsp;<span style="color:#D60073">[</span>&nbsp;7&nbsp;<span style="color:#D60073">,</span>&nbsp;rp&nbsp;<span style="color:#D60073">]</span>&nbsp;<br><br><span style="color:#A0A0A0">//&nbsp;Line&nbsp;6&nbsp;</span><br>&nbsp;&nbsp;&nbsp;d&nbsp;&nbsp;<span style="color:#D60073">[</span>&nbsp;6&nbsp;<span style="color:#D60073">,</span>&nbsp;lp&nbsp;<span style="color:#D60073">]</span>&nbsp;<br><br><span style="color:#A0A0A0">//&nbsp;Line&nbsp;7&nbsp;</span><br>&nbsp;&nbsp;&nbsp;dp&nbsp;<span style="color:#D60073">[</span>&nbsp;3&nbsp;<span style="color:#D60073">,</span>&nbsp;rp&nbsp;<span style="color:#D60073">]</span>&nbsp;<br><br><span style="color:#A0A0A0">//&nbsp;Line&nbsp;8&nbsp;</span><br>&nbsp;&nbsp;&nbsp;dllp</pre>

<!-- CLIFF HIGHLIGHTER 0.01 DEV GENERATED CODE BLOCK--><br>

So the code that you’re looking at is the original code for Arendelle’s cute bird! You now can write the original Arendelle’s logo from scratch!
