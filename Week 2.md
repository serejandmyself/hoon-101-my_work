Reading:
Hoon Syntax https://urbit.org/docs/learn/hoon/hoon-tutorial/hoon-syntax/

Walkthrough:
Conditionals https://urbit.org/docs/learn/hoon/hoon-tutorial/conditionals/

Video:
Areology with ~rapfyr-diglyt: Runes
https://www.youtube.com/watch?v=GdlSXQE67yA

Assignment:
Build a naked generator that takes a noun and checks if that noun is a cell or an atom. If that input noun is an atom, check if it’s even or odd.  The output should be of the tape type. A tape is a string.

My answer:

|=  a=*
?@  a
?:  =(0 (mod a 2))
"Even atom"
"Odd atom"
"Cell"
