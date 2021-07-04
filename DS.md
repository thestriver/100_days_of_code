## Data Structures Crash Course (Algoexpert)

Complexity Analysis: <p>The process of determining how efficient an algorithm is. Complexity analysis usually involves finding both the
    <b>time complexity</b> and the <b>space complexity</b> of an algorithm.
</p>  

----

<h2>Big O notation 
</h2> - a powerful tool that allows us to generalize the space-time complexity of an algorithm as a function of its input size.

<div class><p>
  The notation used to describe the <b>time complexity</b> and
  <b>space complexity</b> of algorithms.
</p>
<p>
  Variables used in Big O notation denote the sizes of inputs to algorithms. For
  example, <b>O(n)</b> might be the time complexity of an algorithm that
  traverses through an array of length <b>n</b>; similarly,
  <b>O(n + m)</b> might be the time complexity of an algorithm that traverses
  through an array of length <b>n</b> and through a string of length <b>m</b>.
</p>
<p>
  The following are examples of common complexities and their Big O notations,
  ordered from fastest to slowest:
</p>
<ul>
  <li><b>Constant</b>: O(1)</li>
  <li><b>Logarithmic</b>: O(log(n))</li>
  <li><b>Linear</b>: O(n)</li>
  <li><b>Log-linear</b>: O(nlog(n))</li>
  <li><b>Quadratic</b>: O(n<sup>2</sup>)</li>
  <li><b>Cubic</b>: O(n<sup>3</sup>)</li>
  <li><b>Exponential</b>: O(2<sup>n</sup>)</li>
  <li><b>Factorial</b>: O(n!)</li>
</ul>
<p>
  Note that in the context of coding interviews, Big O notation is usually
  understood to describe the
  <b>worst-case</b> complexity of an algorithm, even though the worst-case
  complexity might differ from the <b>average-case</b> complexity.
</p>
<p>
  For example, some sorting algorithms have different time complexities
  depending on the layout of elements in their input array. In rare cases, their
  time complexity will be much worse than in more common cases. Similarly, an
  algorithm that takes in a string and performs special operations on uppercase
  characters might have a different time complexity when run on an input string
  of only uppercase characters vs. on an input string with just a few uppercase
  characters.
</p>
<p>
  Thus, when describing the time complexity of an algorithm, it can sometimes be
  helpful to specify whether the time complexity refers to the average case or
  to the worst case (e.g., "this algorithm runs in O(nlog(n)) time on average
  and in O(n<sup>2</sup>) time in the worse case").
</p></div>

Brief overwiew: https://www.youtube.com/watch?v=__vX2sjlpXU 


----

<h2>Logarithm</h2> 

<p><b>log<sub>b</sub>(x) = y</b> if and only if <b>b<sup>y</sup> = x</b></p>

Thus => <p><b>log(n) = y</b> if and only if <b>2<sup>y</sup> = n</b></p>

Key point:

<u>To find the (binary) logarithm of base of a number We have to say <b>2</b> to the **power** of **?** is that number. </u>  if we solve that, **?** is the **log of N**

Thus, To double **N**, we only need to increase **y** by 1. E.g:  2<sup>2</sup> = 4; 2<sup>2+1</sup> = 2<sup>3</sup> which **6**

If n doubles, log(n) only increases by 1

<p>In plain English, if an algorithm has a logarithmic time complexity (<b>O(log(n))</b>, where n is the size of the input), then whenever the algorithm's input doubles in size (i.e., whenever <b>n</b> doubles), the number of
operations needed to
complete the algorithm only increases by one unit. Conversely, an algorithm with a linear time complexity would
see its number of operations double if its input size doubled.</p>