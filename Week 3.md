Reading: <br>
Gates. https://urbit.org/docs/learn/hoon/hoon-tutorial/gates <br>
Lists. https://urbit.org/docs/learn/hoon/hoon-tutorial/lists/ <br>

Walkthrough:<br>
Recursion https://urbit.org/docs/learn/hoon/hoon-tutorial/recursion/<br>
Fibonacci https://urbit.org/docs/learn/hoon/hoon-tutorial/fibonacci/<br>

Video:<br>
Areology with ~rapfyr-diglyt: Debugging https://www.youtube.com/watch?v=DkUIhhq6O24<br>

Assignment:<br>
Comment each line of code from the tail-call optimized recursion example to explain what the code is doing. https://pastebin.com/ac3Yc1ky <br>
Build a naked generator that accepts a list as its argument, and returns the third element of that list. Do not use any standard-library functions. Lists are kinds of nouns that are written as [1 2 3 4 ~].<br>


My Answer: <br>
<br>
|=  n=@ud :: creating a gate that takes the argument "n" and nests it inside an unsigned-integer type <br>
=/  t=@ud  1 :: add a new element into account with the face an unsigned-integer type of 1 <br>
|- :: create a gate with one arm and call it immediatly <br>
?:  =(n 1) :: check if n is 1 <br>
t :: return the value of the second added element <br>
$(n (dec n), t (mul t n)) :: performing a recursion with buc in the gate we are inside of in order to evalute the element n, in order to see if it is 1 or anythign else but 1. To do that we are multiplying the elements t and n in order to get the new value of t and then decrement the element n <br>
== <br>
<br>
|=  [a=@ b=(list @)]<br>
?~  b  !!<br>
?:  =(3 a)  i.b<br>
$(a (dec a), b t.b)
