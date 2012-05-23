<script type="text/javascript">// <![CDATA[
var iRandom;
function Restart()
{
iRandom = Math.floor(Math.random()*10)+1;
alert('OK, I am thinking of a number between 1 and 10');
}
function Guess()
{
var yourGuess = document.getElementById('myGuess').value;
if (yourGuess>iRandom)
    alert('Too High.');
if (yourGuess<iRandom)
    alert('Too Low.');
if (yourGuess==iRandom)
    {
    alert('Well done! You guessed it.');
    Restart();
    }
}
// ]]></script></pre>
<div>Enter your guess between 1 and 10: <input id="myGuess" type="text" name="myGuess" />
<input onclick="Guess()" type="button" value="Guess" />
 
<input onclick="Restart()" type="button" value="Start Again" />
<script type="text/javascript">// <![CDATA[
Restart();
// ]]></script>