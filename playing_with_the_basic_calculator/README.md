# Playing with the Basic Calculator
So as we created a calculator back to chapter 11, we know how to to display information using the title. However we also know about **Stored Spaces** and **Functions**. We can now use them to add more awesome features to our tiny calculator. First, we can save our result in a file using Stored Spaces:

<!-- CLIFF HIGHLIGHTER 0.02 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">(</span>&nbsp;space&nbsp;<span style="color:#D60073">,</span><br><br>&nbsp;&nbsp;&nbsp;<span style="color:#A0A0A0">//&nbsp;something&nbsp;here</span><br><br><span style="color:#D60073">)</span>&nbsp;<span style="color:#D60073">(</span>&nbsp;<span style="color:#4E00FC">$result</span>&nbsp;<span style="color:#D60073">,</span>&nbsp;<span style="color:#4E00FC">@space</span>&nbsp;<span style="color:#D60073">)</span><br><span style="color:#BD00AD">'ANS: \(@space)'</span></pre>

<!-- CLIFF HIGHLIGHTER 0.02 DEV GENERATED CODE BLOCK--><br>

Let’s create some functions for our calculator. Do you remember the `!pow(number,power)` function we wrote together? If you put the `pow.arendelle` file into the folder where your `calc.arendelle` file is you can then use it in our calc:

<!-- CLIFF HIGHLIGHTER 0.02 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073">(</span>&nbsp;space&nbsp;<span style="color:#D60073">,</span><br><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">!pow</span>&nbsp;<span style="color:#D60073">(</span>&nbsp;2&nbsp;<span style="color:#D60073">,</span>&nbsp;7&nbsp;<span style="color:#D60073">)</span><br><br><span style="color:#D60073">)</span>&nbsp;<span style="color:#D60073">(</span>&nbsp;<span style="color:#4E00FC">$result</span>&nbsp;<span style="color:#D60073">,</span>&nbsp;<span style="color:#4E00FC">@space</span>&nbsp;<span style="color:#D60073">)</span><br><span style="color:#BD00AD">'ANS: \(@space)'</span></pre>

<!-- CLIFF HIGHLIGHTER 0.02 DEV GENERATED CODE BLOCK--><br>

And you will see the **ANS: 128** in the title! Something I want to show you are recursive functions:

<br><br>
## Recursive Functions
Do you know the **factorial** operator? It’s like this: When you write `5!` ( *! is the factorial sign* ) you get this:

```
5! = 5 × 4 × 3 × 2 × 1
```

And so the factorial of 12 will be:

```
12! = 12 × 11 × 10 … 3 × 2 × 1
```

So as you saw `5!` was `5 × 4 × 3 × 2 × 1` just like the end of the `12!` and that’s why we can write this:

```
12! = 12 × 11 × 10 × 9 × 8 × 7 × 6 × 5!
```

Or even this

```
12! = 12 × 11!
```

You see each factorial is connected to it’s preview factorials for example if you want to calculate factorial of 4, you have to do `4 × 3!` and then you have to calculate `3!` using `3! × 2!` till you get to `1!` which you know it’s `1`.<br>

In the programming there is a very fun thing called **Recursive Function** which is a function that uses itself! Each math operator like factorial is a function. So as you saw we used factorial to calculate factorial which means we used a function in itself!<br>

Let’s write factorial using recursive technique to see how can you use a function in itself. First create the function `!fact(number)` and then write this code for it:

<!-- CLIFF HIGHLIGHTER 0.02 DEV GENERATED CODE BLOCK--><br>

<pre style="font-family: Monospace;">
<span style="color:#D60073"><</span>&nbsp;number&nbsp;<span style="color:#D60073">></span><br><span style="color:#D60073">{</span>&nbsp;<span style="color:#4E00FC">@number</span>&nbsp;=&nbsp;1&nbsp;<span style="color:#D60073">,</span><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">(</span>&nbsp;return&nbsp;<span style="color:#D60073">,</span>&nbsp;1&nbsp;<span style="color:#D60073">)</span><br><span style="color:#D60073">,</span><br>&nbsp;&nbsp;&nbsp;<span style="color:#D60073">(</span>&nbsp;return&nbsp;<span style="color:#D60073">,</span>&nbsp;<span style="color:#4E00FC">@number</span>&nbsp;*&nbsp;<span style="color:#D60073">!fact</span><span style="color:#D60073">(</span>&nbsp;<span style="color:#4E00FC">@number</span>&nbsp;-&nbsp;1&nbsp;<span style="color:#D60073">)</span>&nbsp;<span style="color:#D60073">)</span><br><span style="color:#D60073">}</span></pre>

<!-- CLIFF HIGHLIGHTER 0.02 DEV GENERATED CODE BLOCK--><br>

You see? We’re calling for function `!fact()` from the function `!fact()`! It’s really an amazing possibility we have in programming to call a function from itself!


<br><br><hr>
<h4>Exercise</h4>
Do you know the **Fibonacci sequence**? It’s a sequence of numbers which each number is the sum of it’s two previous number like:

```
1  1  2  3  5  8  13  21 …
```

You see `2` is the sum of `1` and `1`, `13` is the sum of `5` and `8`, `5` is the sum of `2` and `3` and so on… Write a recursive function named `!sumOfFibonacci(number)` that calculate the sum of the `@number` first members of the sequence like:

```
!sumOfFibonacci( 4 ) = sum ( 1 , 1 , 2 , 3 ) = 7
!sumOfFibonacci( 7 ) = sum ( 1 , 1 , 2 , 3 , 5 , 8 , 13 ) = 33
```

<hr>

