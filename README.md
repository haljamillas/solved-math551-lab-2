Download Link: https://assignmentchef.com/product/solved-math551-lab-2
<br>
<strong>Goals: </strong>In this assignment you will learn how to determine whether a system of linear equations has a solution, how to reduce a system to a row echelon form and how to visualize the solution. During the lab session, your lab instructor will teach you the necessary Matlab code to complete the assignment, which will be discussed in the lab.

<strong>To get started: </strong>Create a new Matlab script file and save it as “lab02.m”.

<strong>Matlab commands to learn: </strong>magic, rref, rank, transpose, plot, figure, hold on, grid on, grid off, subplot, meshgrid, surf, view

<strong>What you have to submit: </strong>The file lab02.m, which you will create during the lab session.

<strong>Reminders About the Grading Software</strong>

Remember, the labs are graded with the help of software tools. If you do not follow the instructions, you will lose points. If the instructions ask you to assign a value to a variable, you must <strong>use the variable name given in the instructions</strong>. If the instructions ask you to make a variable named x1 and instead you make a variable named x or X or X1 or any name other than x1, the grading software will not find your variable and you <em>will </em>lose points. Required variables are listed in the lab instructions in a gray box like this:

<h1>Variables: x1, A, q</h1>

At times you will also be asked to answer questions in a comment in your M-file. You must <strong>format your text answers correctly</strong>. Questions that you must answer are shown in gray boxes in the lab. For example, if you see the instruction

Q7: What does the Matlab command lu do? your file must contain a line similar to the following somewhere

% Q7: It computes the LU decomposition of a matrix.

The important points about the formatting are

<ul>

 <li>The answer is on a single line.</li>

 <li>The first characters on the line is the comment character %.</li>

 <li>The answer is labeled in the form Q<em>n</em>:, where <em>n </em>stands for the question number from the gray box.</li>

</ul>

If you do not format your answers correctly, the grading software will not find them and you <em>will </em>lose points.

<strong>TASKS</strong>

<ol>

 <li>Create a 5 × 5 matrix <em>A </em>using the magic command. Type help magic in the command line to learn about the magic command.</li>

</ol>

<h1>Variables: A</h1>

<ol start="2">

 <li>Create a column-vector <em>B </em>with entries 1<em>,</em>3<em>,</em>2<em>,</em>−1<em>,</em> Variables: B</li>

 <li>Create a matrix <em>M </em>by adding the vector <em>B </em>as the last column of the matrix <em>A</em>. Variables: M</li>

 <li>Check the rank of <em>A </em>and <em>M </em>using the rank Type help rank in the command line to learn about the rank command.</li>

</ol>

<table width="339">

 <tbody>

  <tr>

   <td width="163">Variables: rank A, rank M</td>

   <td width="176"></td>

  </tr>

  <tr>

   <td colspan="2" width="339">Q1: Is the system with augmented matrix <em>M </em>consistent?</td>

  </tr>

 </tbody>

</table>

<ol start="5">

 <li>Produce a reduced row echelon form of <em>M </em>by using the rref Type help rref in the command line to learn about the rref command. Variables: rref M</li>

 <li>Create a 7 × 7 matrix <em>C </em>using the rand Type help rand in the command line to learn about the rand command. Variables: C</li>

 <li>Create a row vector <em>D </em>with 7 elements using the rand Variables: D</li>

 <li>Apply the transpose command to <em>D</em>. Type help transpose in the command line to learn about the transpose</li>

</ol>

<table width="273">

 <tbody>

  <tr>

   <td width="141">Variables: transpose D</td>

   <td width="132"></td>

  </tr>

  <tr>

   <td colspan="2" width="273">Q2: What does the transpose command do?</td>

  </tr>

 </tbody>

</table>

<ol start="9">

 <li>Create an augmented matrix <em>N </em>of the system with coefficient matrix <em>C </em>and right-hand side <em>D</em>. Variables: N</li>

 <li>Apply the rref command to <em>N</em>.</li>

</ol>

<h1>Variables: rref N</h1>

<ol start="11">

 <li>Consider the system of two equations:</li>

</ol>

( <em>x </em>+ 2<em>y </em>= 3 <em>x </em>− <em>y </em>= 0

Plot the lines representing each of the equations on one graph using the plot command on the interval [0<em>,</em>5]. Use the color red for the first equation and the color blue for the second.

Type in the commands

<table width="599">

 <tbody>

  <tr>

   <td width="27">1</td>

   <td width="572">figure;</td>

  </tr>

  <tr>

   <td width="27">2</td>

   <td width="572">x = [0:0.1:5];</td>

  </tr>

  <tr>

   <td width="27">3</td>

   <td width="572">y1=(3-x)/2;</td>

  </tr>

  <tr>

   <td width="27">4</td>

   <td width="572">y2=x;</td>

  </tr>

  <tr>

   <td width="27">5</td>

   <td width="572">plot(x,y1,’red’);</td>

  </tr>

  <tr>

   <td width="27">6</td>

   <td width="572">hold on;</td>

  </tr>

  <tr>

   <td width="27">7</td>

   <td width="572">plot(x,y2,’blue’);</td>

  </tr>

  <tr>

   <td width="27">8</td>

   <td width="572">grid on;</td>

  </tr>

 </tbody>

</table>

<ol start="12">

 <li>Consider the system</li>

</ol>

<sup> </sup>2<em>x </em>+ <em>y </em>+ <em>z </em>= 4



−<em>x </em>+ <em>y </em>− <em>z </em>= 1

<sup></sup>3<em>x </em>+ 2<em>y </em>− <em>z </em>= 6

Note that this system of equations cooresponds to the following augmented matrix:

Type in the commands

<table width="599">

 <tbody>

  <tr>

   <td colspan="2" width="27">1</td>

   <td colspan="3" width="572">figure;</td>

  </tr>

  <tr>

   <td colspan="2" width="27">2</td>

   <td colspan="3" width="572">[x,y]=meshgrid(-5:0.1:5,-5:0.1:5);</td>

  </tr>

  <tr>

   <td colspan="2" width="27">3</td>

   <td colspan="3" width="572">z1=4-2*x-y;</td>

  </tr>

  <tr>

   <td colspan="2" width="27">4</td>

   <td colspan="3" width="572">z2=-x+y-1;</td>

  </tr>

  <tr>

   <td colspan="2" width="27">5</td>

   <td colspan="3" width="572">z3=3*x+2*y-6;</td>

  </tr>

  <tr>

   <td colspan="2" width="27">6</td>

   <td colspan="3" width="572">surf(x,y,z1);</td>

  </tr>

  <tr>

   <td colspan="2" width="27">7</td>

   <td colspan="3" width="572">hold on;</td>

  </tr>

  <tr>

   <td colspan="2" width="27">8</td>

   <td colspan="3" width="572">surf(x,y,z2);</td>

  </tr>

  <tr>

   <td colspan="2" width="27">9</td>

   <td colspan="3" width="572">hold on;</td>

  </tr>

  <tr>

   <td colspan="2" width="27">10</td>

   <td colspan="3" width="572">surf(x,y,z3);</td>

  </tr>

  <tr>

   <td width="4"></td>

   <td colspan="3" width="266">Q8: What does the meshgrid command do?</td>

   <td width="330"></td>

  </tr>

  <tr>

   <td width="4"></td>

   <td colspan="2" width="238">Q9: What does the surf command do?</td>

   <td width="28"></td>

   <td width="330"></td>

  </tr>

  <tr>

   <td width="4"></td>

   <td width="23"></td>

   <td width="215"></td>

   <td width="28"></td>

   <td width="330"></td>

  </tr>

 </tbody>

</table>

<ol start="13">

 <li>Come up with three systems of linear equations in three variables (with three equations each) representing all possible situations: no solution, a unique solution, infinitely many solutions. For each system of equations, create the corresponding augmented matrix, respectively naming them no sol, uni sol, inf sol. Apply the commands above to produce a visual picture for each of the systems (each on a separate figure). Use appropriate limits for variables <em>x </em>and <em>y </em>and a command view to present each case clearly.</li>

</ol>

<h1>Variables: no sol, uni sol, inf sol</h1>