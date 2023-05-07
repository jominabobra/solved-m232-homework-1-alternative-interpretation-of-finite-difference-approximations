Download Link: https://assignmentchef.com/product/solved-m232-homework-1-alternative-interpretation-of-finite-difference-approximations
<br>
<ol>

 <li><em>This problem provides an alternative interpretation of finite difference approximations.</em></li>

</ol>

Derive approximations for <em>u</em><sup>0</sup>(<em>x</em>) by (i) fitting each of the sets of data below to the highest order polynomial you are able to consider, and then (ii) taking the exact derivative of that polynomial and evaluating that result at <em>x</em>.

<ul>

 <li>{<em>u</em>(<em>x</em>)<em>,u</em>(<em>x </em>+ <em>h</em>)}</li>

 <li>{<em>u</em>(<em>x </em>− <em>h</em>)<em>,u</em>(<em>x</em>)}</li>

 <li>{<em>u</em>(<em>x </em>− <em>h</em>)<em>,u</em>(<em>x</em>)<em>,u</em>(<em>x </em>+ <em>h</em>)}</li>

</ul>

Show that your results correspond exactly to <em>D</em><sub>+</sub><em>u</em>(<em>x</em>), <em>D</em><sub>−</sub><em>u</em>(<em>x</em>) and <em>D</em><sub>0</sub><em>u</em>(<em>x</em>), respectively. Discuss how this alternative derivation of these finite difference formulas informs your understanding of their respective truncation errors.

<ol start="2">

 <li><em>This problem provides an introduction to the </em>m <em>code that we will use for other problems in this class.</em>

  <ul>

   <li>Use the method of undetermined coefficients to set up the 5 × 5 Vandermonde system that would determine a fourth-order accurate finite difference approximation to <em>u</em><sup>00</sup>(<em>x</em>) based on 5 equally spaced points,</li>

  </ul></li>

</ol>

<em>u</em><sup>00</sup>(<em>x</em>) = <em>c</em><sub>−2</sub><em>u</em>(<em>x </em>− 2<em>h</em>) + <em>c</em><sub>−1</sub><em>u</em>(<em>x </em>− <em>h</em>) + <em>c</em><sub>0</sub><em>u</em>(<em>x</em>) + <em>c</em><sub>1</sub><em>u</em>(<em>x </em>+ <em>h</em>) + <em>c</em><sub>2</sub><em>u</em>(<em>x </em>+ 2<em>h</em>) + <em>O</em>(<em>h</em><sup>4</sup>)<em>.</em>

<ul>

 <li>Compute the coefficients using the Matlab code m available from the CatCourses website, and check that they satisfy the system you determined in part (a).</li>

 <li>Test this finite difference formula to approximate <em>u</em><sup>00</sup>(1) for <em>u</em>(<em>x</em>) = sin(2<em>x</em>) with values of <em>h </em>from the array hvals = logspace(-1, -4, 13). Make a table of the error vs. <em>h </em>for several values of <em>h </em>and compare against the predicted error from the leading term of the expression printed by fdstencil. You may want to look at the m-file m for guidance on how to make such a table.</li>

</ul>

Also produce a log-log plot of the absolute value of the error vs. <em>h</em>. Be sure to label axes, include a legend, and any other items needed to make this plot clear and understandable.

You should observe the predicted accuracy for larger values of <em>h</em>. For smaller values, numerical cancellation in computing the linear combination of <em>u </em>values impacts the accuracy observed.