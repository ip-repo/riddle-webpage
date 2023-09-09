# riddle-webpage: Example of JavaScript obfuscation.
<hr>

In this example there is a wepage with a photo ,input box and button.<br>
The user need to solve a riddle based on the photo and he is encouraged to use the browser <b>inspect tool </b>.
<h2><a href="https://ip-repo.github.io/riddle-webpage/">Go ahead and try solve the riddle </a></h2>
The answer box and button are html elements so when the button is clicked a Javascript function loacted in <b>script.js</b> will compare the box input to the correct answer.<br>
The Javascript function look somthing like this:

```javascript
function compareUserInputToCorrectAnswer(userInput) {
	var userInput = userInput.toLowerCase();
	if ( userInput== 'correct answer') {
		alert(userInput + ' is the correct answer!');
	} else {		
		alert('wrong! try again.');
	}	
 }

```
Now ,if one inspected the Javascript script he could find the answer.<br>
So by using Javascript obfuscation we can make it harder to read the webpage Javascript code.<br>
In this example <a href="https://javascriptobfuscator.com/">js-obfuscator</a> was used.<br>
Now after the obfuscation that function should look somthing like this:

```javascript
var _0x6b22=["\x74\x6F\x4C\x6F\x77\x65\x72\x43\x61\x73\x65","\x77\x68\x69\x74\x65",
"\x20\x69\x73\x20\x74\x68\x65\x20\x63\x6F\x72\x72\x65\x63\x74\x20\x61\x6E\x73\x77\x65\x72\x21",
"\x77\x72\x6F\x6E\x67\x21\x20\x74\x72\x79\x20\x61\x67\x61\x69\x6E\x2E"];
function  compareUserInputToCorrectAnswer(_0xf4cbx2){var _0xf4cbx2=_0xf4cbx2[_0x6b22[0]]();
if(_0xf4cbx2== _0x6b22[1]){alert(_0xf4cbx2+ _0x6b22[2])}else {alert(_0x6b22[3])}}

```
This can make the user attempet to solve the riddle by inspecting the webpage harder.
