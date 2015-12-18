# Thaana-Typing-on-Webforms
Use the JavaScript to convert English alphabet to Unicode Thaana. 

Typing Unicode Thaana on webforms
---------------------------------
<!--
<script>
// used to convert english alphabet to unicode thaana
function toThaana() {
	var englishUnicode = [104,83,110,114,98,76,107,119,118,109,102,100,116,108,103,78,115,68,122,84,121,112,106,99,88,72,75,74,82,67,66,77,89,90,87,71,81,86,97,65,105,73,117,85,101,69,111,79,113,70];
  var typedStr = document.getElementById("typedText").value;
	var convertedStr = "";
	for(var i=0; i < typedStr.length; i++ )
	{
		var n = typedStr.charCodeAt(i), uniChar; 
		if((n>96 && n<123) || (n>64 && n<91) || n==70){
			switch(n){
				case 70:    // special char
						uniChar = String.fromCharCode(65010);
						break;
				default:
						n= englishUnicode.indexOf(n);
						uniChar = String.fromCharCode(n + 1920);
			}
		}else{
			uniChar = String.fromCharCode(n);			
		}		
		convertedStr = convertedStr.concat(uniChar);
	}
	document.getElementById("typedText").value; = convertedStr;
}
</script>

--------------------------------------------------------------

<input type="textbox" id="typedText" onkeypress="toThaana();" />
-->
--------------------------------------------------------------
Original implementation at: www.nclhr.com/index.php
