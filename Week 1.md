Reading:<br>
Booting a fakezod https://urbit.org/docs/using/creating-a-development-ship/
Intro to Dojo https://urbit.org/docs/using/shell/
Nouns https://urbit.org/docs/learn/hoon/hoon-tutorial/nouns/

Videos:<br>
Areology with ~rapfyr-diglyt: Booting a Fakezod https://youtu.be/Abh54Uce6f8
Areology with ~rapfyr-diglyt: Nouns https://youtu.be/W7OZK9YzqXc

Walkthrough:<br>
List of Numbers  https://urbit.org/docs/learn/hoon/hoon-tutorial/list-of-numbers/

Assignment:<br>
Build a naked generator that takes an atom from the user and returns that atom with a different aura. See the first section of https://urbit.org/docs/learn/hoon/hoon-tutorial/generators/ for information on naked generators.


My answer:<br>
cd zod/home/gen cat > echo.hoon <br>
|=  [a=@ud] <br>
`@p`a <br>
<br>
<br>
/CNTRL D to save file <br>
cd <br>
urbit zod <br>
+echo 2 /we can check that results in: <br>
~bec / different aura
