<div align="center">

## Sidd Calc 2\.1


</div>

### Description

Sid calc is a simple calculator, with graphics n sh!t. Anyways download it and i dont give a sh!t.
 
### More Info
 
Calculation

Dont mess around with the script unless you know javascript, one slight change on the coding might ruin the script, my script can be really confusing to understand sometimes.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Siddharth Sur](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/siddharth-sur.md)
**Level**          |Advanced
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |
**Category**       |[Controls/ Forms/ Graphics/ Menus](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/controls-forms-graphics-menus__2-59.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/siddharth-sur-sidd-calc-2-1__2-3389/archive/master.zip)





### Source Code

```
<html>
<head>
	<title>SidCal 2002</title>
<body bgcolor=black>
<style>
#rightclick
{
background:red;
border=solid 2px #0099ff;
width:150;
color=#ffffff;
font-size:13pt;
visibility:hidden;
}
input.backNtext
{
background-color:black;
color:"#00ff00";
font-family:System;
font-size:13pt;
border:0;
}
input.oprBackNtext
{
background-color:"#0099ff";
color:"#00ff00";
font-family:System;
font-size:13pt;
border:0;
}
#calBack
{
position:absolute;
left=350;
top=120;
background:"#696969";
border:solid 2px;
border-color:"#B3B6B6";
width=164;
height=100;
}
#logo
{
color:blue;
position:absolute;
left=350;
top=95;
background-image=url(C:\My Documents\Sid\New_site\calseculator\Sqr_Qnd_calc\calc.jpg);
filter: glow(strength = 5, color=red);
font-family:System;
font-size=16pt;
width=164;
height=24;
border=solid 1px;
border-color:"#B3B6B6";
}
body
{
scrollbar-3dlight-color:#ffffff;
scrollbar-arrow-color:#577C93;
scrollbar-base-color:#577C93;
scrollbar-track-color:#222222;
scrollbar-darkshadow-color:#ffffff;
scrollbar-face-color:#E2E9ED;
scrollbar-highlight-color:#577C93;
scrollbar-shadow-color:#577C93;
}
#helpPower
{
background:"#000000";
border:solid 1px;
border-color:"a9a9a9";
position:absolute;
color:"#0099ff";
font-family:Bell MT;
font-size:13pt;
visibility: hidden;
width: 200;
}
a.howTolink:link, a.howTolink:visited
{
text-decoration:none;
color:"0099ff";
font-family:system;
font-size:5px;
}
a.howTolink:hover, a.howTolink:active
{
text-decoration:overline underline;
color:"#0081a8";
font-family:system;
font-size:5px;
cursor:help;
}
#madeBySid
{
position:absolute;
left:10;
top:400;
background:"#0099ff";
color:"0000ff";
border:solid 2px;
border-color:"red";
font-family:system;
font-size:12pt;
width:"120";
height:"20";
filter:glow(strength= 5, color=yellow);
}
#helpSidCal
{
position:absolute;
background:"#FFFF8D";
color:black;
font-family:Times;
left:10;
top:50;
font-size:13pt;
visibility:hidden;
width:280;
z-index:1;
}
#helpSidCalContents
{
background:"#B4B4B4";
font-family:system;
width=100;
font-size:12pt;
visibility:hidden;
}
#othersMenu
{
background:"#B4B4B4";
font-family:system;
width=100;
height=60;
font-size:12pt;
visibility:hidden;
position:absolute;
left:50;
top:34;
}
font.helpSidCalHeading
{
font-family:Times;
font-size:14pt;
color:"#0C4E8D";
text-decoration:underline;
}
#menuBar
{
background:"#BCBCBD";
width:200;
}
#newVersionHead
{
position:absolute;
left:10;
top:130;
background:"0099ff";
color:"#ABAAAA";
width:210;
font-family:arial;
font-size:25pt;
border:solid 1px;
border-color:red;
}
#sidCalShadow
{
position:absolute;
left:60;
top:10;
font-family:arial;
font-size:25pt;
color:red;
filter: glow(strength = 5, color=white);
}
a.download:link, a.download:visited
{
color:red;
text-decoration:none;
font-family:Verdana;
font-size:12pt;
}
a.download:hover, a.download:active
{
color:"#AB4240";
text-decoration:underline;
font-family:Verdana;
font-size:12pt;
}
a.sourceCode:link, a.sourceCode:visited
{
color:orange;
text-decoration:none;
font-family:bell mt;
font-size:12pt;
}
a.sourceCode:hover, a.sourceCode:active
{
color:"#00ff00";
text-decoration:underline;
font-family:bell mt;
font-size:12pt;
background:"#0079FF";
border:solid 1px;
border-color:#a9a9a9;
}
</style>
<script language="javascript">
window.defaultStatus="Sid Calc 2002"
function sqrIt(form)
{
var number=sidcal.answer.value;
var get= eval(number*number);
sidcal.answer.value=get;
}
function squareRt(form)
{
var sqr=sidcal.answer.value;
var get= Math.sqrt(sqr);
sidcal.answer.value=get;
}
function pieIt(form)
{
var pie= sidcal.answer.value;
var get= eval(pie*3.14);
sidcal.answer.value=get;
}
function cubeIt(form)
{
var cube= sidcal.answer.value;
var get= eval(cube*cube*cube);
sidcal.answer.value=get;
}
function power_2(form)
{
var power1=eval(sidcal.pow1.value);
var power2=eval(sidcal.pow2.value);
var get= Math.pow(power1, power2);
sidcal.answer.value=get;
}
function menus (whichMenu,state){
if (navigator.appName == "Microsoft Internet Explorer"){
document.all[whichMenu].style.visibility = state;
}
else {document[whichMenu].visibility = state;}
	}
function helpexample(form, text1, text2, text3)
{
sidcal.pow1.value=text1;
sidcal.pow2.value=text2;
sidcal.answer.value=text3;
}
function howTobtn(text, back)
{
sidcal.howTo.style.color=text;
sidcal.howTo.style.background=back;
}
function contactbtn(text, back)
{
sidcal.mailSid.style.color=text;
sidcal.mailSid.style.background=back;
}
function closebtn(text, back)
{
sidcal.closeHelp.style.color=text;
sidcal.closeHelp.style.background=back;
}
function promptCalc()
{
var calc= prompt("Enter calculation","");
var get= eval(calc);
if(calc==null || calc=="" || calc==get)
{
alert("No calculation done");
}
else
{
alert(calc + " = " + get);
}
}
function otherStyle(text, back)
{
sidcal.otherBtn.style.color=text;
sidcal.otherBtn.style.background=back;
}
function nomouse()
{
if (event.button >1)
{
menus('rightclick', 'visible');
}
}
document.onmousedown =nomouse;
</script>
<!====================ON RIGHT CLICK=========================>
<div id="rightclick" style="position=absolute; right=10" onMouseOver="menus('rightclick', 'visible')" onMouseOut="menus('rightclick', 'hidden')">
About SidCal
<br>
More Sid Programs
<br>
Calculator 2
<br>
Sid Cal update info
</div>
<!============================VERSION INFO/DOWNLOAD==================>
<div id="newVersionHead" align="center">
<div id="sidCalShadow">SidCalc</div>
SidCalc Version 2.1!<br>
<a href="#" class="download">Download SidCalc 2.1</a>
</div>
<!========================HOW TO USE SIDCAL & OTHER CALC====================>
<form name="sidcal">
<div id="menuBar">
<input type="button" name="helpbtn" value="Help" onClick="javascript:menus('helpSidCalContents', 'visible')" style="background=#bcbcbd; border=0" onMouseOver="document.sidcal.helpbtn.style.background='#a9a9a9'" onMouseOut="document.sidcal.helpbtn.style.background='#bcbcbd'">
<input type="button" name="other" value="Other" onClick="javascript:menus('othersMenu', 'visible')" style="background=#bcbcbd; border=0" onMouseOver="document.sidcal.other.style.background='#a9a9a9'" onMouseOut="document.sidcal.other.style.background='#bcbcbd'">
</div>
<div id="othersMenu" align="center" onMouseOver="javascript:menus('othersMenu', 'visible')" onMouseOut="javascript:menus('othersMenu', 'hidden')">
<input type="button" name="otherBtn" value="Other Calc" onClick="javascript:promptCalc()" onMouseOver="javascript:otherStyle('white', '#4E32A8')" onMouseOut="javascript:otherStyle('black','#b4b4b4')" style="border=0">
<hr width="100%">
</div>
<div id="helpSidCalContents" align="center" onMouseOver="javascript:menus('helpSidCalContents', 'visible')" onMouseOut="javascript:menus('helpSidCalContents', 'hidden')">
<input type="button" name="howTo" value="How To" onClick="javascript:menus('helpSidCal', 'visible')" onMouseOver="javascript:howTobtn('white', '#4E32A8')" onMouseOut="javascript:howTobtn('black', '#b4b4b4')" style="border=0">
<hr widht="100%">
<input type="button" name="mailSid" value="Contact Sid" onClick="javascript:window.location='http://junk_yark_dawg.tripod.com/first.html'" onMouseOver="javascript:contactbtn('white', '#4E32A8')" onMouseOut="javascript:contactbtn('black', '#b4b4b4')" style="border=0">
<hr>
<input type="button" name="closeHelp" value="Exit" onClick="javascript:menus('helpSidCalContents', 'hidden')" onMouseOver="javascript:closebtn('white', '#4E32A8')" onMouseOut="javascript:closebtn('black', '#b4b4b4')" style="border=0">
</div>
<div id="helpSidCal">
<center><font class="helpSidCalHeading">HOW TO USE SIDCALC 2002</font></center><input type="button" name="close" value="X" onClick="javascript:menus('helpSidCal', 'hidden')" style="font-family=Arial; font-size=10pt; widht=16; height=20; position:absolute; left=265; top=0">
<br>
Sid Calc 2002 is an easy to use calculator. You probably understand the basics, like how to add, subtract, multiply and divide. What this help is for is how to use the more advanced functions in this calculator.<br>
The <font color=red>††</font> button you see is the pie button. It multiplies the number by 3.14. <br>
The <font color=red>X²</font> button is the square button. It times the number twice by itself. And, <font color=red>X³</font> times the number three times by itself.<br>
The <font color=red>_/&#8254;</font> button is to find square root of a number<br>
If you want to know what the two white boxes are there for, then click on the <b>how to?</b> button below it. <br>
<b>Thats all the functions you needed to know. Enjoy!</b>
<br>
<br>
</div>
<!===========================LOGO WITH MARQUEE=========================>
<div id="logo" align="center" valign="center">
<marquee behavior=slide width=55% scrollamount=6 scrolldelay=300>Sid Calc 2002</marquee>
</div>
<div id="calBack">
<table border="0" cellspacing="3" bordercolor="black" bordercolorlight="black" bordercolordark="black">
<tr><td align="center">
<!================================TEXT BOX===============================>
<input type="text" name="answer" size="20" value="" style="background-color:black; border=solid 1px; border-color:#c0c0c0; color:#00ff00; cursor:hand; font-family=system; background-image=url(back_tesaxt.gif)">
</tr></td></table>
<table border="0" cellspacing="5" bordercolor="black" bordercolorlight="black" bordercolordark="black">
	<tr>
<td align="center" valign="center">
<input type="button" name="plus" size="100" class="oprBackNtext" value=" + " onClick="document.sidcal.answer.value+='+'" onMouseOver="document.sidcal.plus.style.background='#ff0000'" onMouseOut="document.sidcal.plus.style.background='#0099ff'" onMouseDown="document.sidcal.plus.style.background='#a9a9a9'">
<td align="center" valign="center">
<input type="button" name="minus" size="100" class="oprBackNtext" value=" - " onClick="document.sidcal.answer.value+='-'" onMouseOver="document.sidcal.minus.style.background='#ff0000'" onMouseOut="document.sidcal.minus.style.background='#0099ff'" onMouseDown="document.sidcal.minus.style.background='#a9a9a9'">
<td align="center" valign="center">
<input type="button" name="times" size="100" class="oprBackNtext" value=" * " onClick="document.sidcal.answer.value+='*'" onMouseOver="document.sidcal.times.style.background='#ff0000'" onMouseOut="document.sidcal.times.style.background='#0099ff'" onMouseDown="document.sidcal.times.style.background='#a9a9a9'">
<td align="center" valign="center">
<input type="button" name="divide" size="100" class="oprBackNtext" value=" / " onClick="document.sidcal.answer.value+='/'" onMouseOver="document.sidcal.divide.style.background='#ff0000'" onMouseOut="document.sidcal.divide.style.background='#0099ff'" onMouseDown="document.sidcal.divide.style.background='#a9a9a9'">
</td></td></td></td>
	</tr>
	<tr>
<td align="center">
<input type="button" name="one" size="100" class="backNtext" value=" 1 " onClick="document.sidcal.answer.value+='1'" onMouseOver="document.sidcal.one.style.background='#0081A8'" onMouseOut="document.sidcal.one.style.background='black'" onMouseDown="document.sidcal.one.style.background='#a9a9a9'">
<td align="center">
<input type="button" name="two" class="backNtext" value=" 2 " onClick="document.sidcal.answer.value+='2'" onMouseOver="document.sidcal.two.style.background='#0081A8'" onMouseOut="document.sidcal.two.style.background='black'" onMouseDown="document.sidcal.two.style.background='#a9a9a9'">
<td align="center">
<input type="button" name="three" class="backNtext" value=" 3 " onClick="document.sidcal.answer.value+='3'" onMouseOver="document.sidcal.three.style.background='#0081A8'" onMouseOut="document.sidcal.three.style.background='black'" onMouseDown="document.sidcal.three.style.background='#a9a9a9'">
<td align="center">
<input type="button" name="four" class="backNtext" value=" 4 " onClick="document.sidcal.answer.value+='4'" onMouseOver="document.sidcal.four.style.background='#0081A8'" onMouseOut="document.sidcal.four.style.background='black'" onMouseDown="document.sidcal.four.style.background='#a9a9a9'">
</td></td></td></td>
	</tr>
	<tr>
<td align="center">
<input type="button" name="five" class="backNtext" value=" 5 " onClick="document.sidcal.answer.value+='5'" onMouseOver="document.sidcal.five.style.background='#0081A8'" onMouseOut="document.sidcal.five.style.background='black'" onMouseDown="document.sidcal.five.style.background='#a9a9a9'">
<td align="center">
<input type="button" name="six" class="backNtext" value=" 6 " onClick="document.sidcal.answer.value+='6'" onMouseOver="document.sidcal.six.style.background='#0081A8'" onMouseOut="document.sidcal.six.style.background='black'" onMouseDown="document.sidcal.six.style.background='#a9a9a9'">
<td align="center">
<input type="button" name="seven" class="backNtext" value=" 7 " onClick="document.sidcal.answer.value+='7'" onMouseOver="document.sidcal.seven.style.background='#0081A8'" onMouseOut="document.sidcal.seven.style.background='black'" onMouseDown="document.sidcal.seven.style.background='#a9a9a9'">
<td align="center">
<input type="button" name="eight" class="backNtext" value=" 8 " onClick="document.sidcal.answer.value+='8'" onMouseOver="document.sidcal.eight.style.background='#0081A8'" onMouseOut="document.sidcal.eight.style.background='black'" onMouseDown="document.sidcal.eight.style.background='#a9a9a9'">
</td></td></td></td>
</tr>
	<tr>
<td align="center">
<input type="button" name="nine" class="backNtext" value=" 9 " onClick="document.sidcal.answer.value+='9'" onMouseOver="document.sidcal.nine.style.background='#0081A8'" onMouseOut="document.sidcal.nine.style.background='black'" onMouseDown="document.sidcal.nine.style.background='#a9a9a9'">
<td align="center">
<input type="button" name="zero" class="backNtext" value=" 0 " onClick="document.sidcal.answer.value+='0'" onMouseOver="document.sidcal.zero.style.background='#0081A8'" onMouseOut="document.sidcal.zero.style.background='black'" onMouseDown="document.sidcal.zero.style.background='#a9a9a9'">
<td align="center">
<input type="button" name="clear" value=" C " onClick="document.sidcal.answer.value=''" style="background=#ff0000; color=#00ff00; border=0; font-family=System; font-size=13pt" onMouseOver="document.sidcal.clear.style.background='#C60000'" onMouseOut="document.sidcal.clear.style.background='#ff0000'" onMouseDown="document.sidcal.clear.style.background='#FFFF00'">
<td align="center">
<input type="button" name="equal" value=" = " onClick="document.sidcal.answer.value=eval(document.sidcal.answer.value)" style="background=white; border=0; color=#a9a9a9; font-family=System; font-size=14px" onMouseOver="document.sidcal.equal.style.background='black'" onMouseOut="document.sidcal.equal.style.background='white'" onMouseDown="document.sidcal.equal.style.background='#c9c9c9'">
</td></td></td></td>
</tr>
	<tr>
<td align="center">
<input type="button" name="square" value="X²" onClick="sqrIt(this.form)" style="background=#a9a9a9; color=black; font-family=System; font-size=11pt; width=30; border=0" onMouseOver="document.sidcal.square.style.background='#BA2B2C'" onMouseOut="document.sidcal.square.style.background='#a9a9a9'" onMouseDown="document.sidcal.square.style.background='#BA2B2C'">
<td align="center">
<input type="button" name="sqr_route" value="_/&#8254;" onClick="squareRt(this.form)" style="background=#a9a9a9; color=black; font-family=System; font-size=11pt; width=30; border=0" onMouseOver="document.sidcal.sqr_route.style.background='#BA2B2C'" onMouseOut="document.sidcal.sqr_route.style.background='#a9a9a9'" onMouseDown="document.sidcal.sqr_route.style.background='#BA2B2C'">
<td align="center">
<input type="button" name="cube" value="X³" onClick="cubeIt(this.form)" style="background=#a9a9a9; color=black; font-family=System; font-size=11pt; width=30; border=0" onMouseOver="document.sidcal.cube.style.background='#BA2B2C'" onMouseOut="document.sidcal.cube.style.background='#a9a9a9'" onMouseDown="document.sidcal.cube.style.background='#BA2B2C'">
<td align="center">
<input type="button" name="pie" value=" †† " onClick="pieIt(this.form)" style="background=#a9a9a9; color=black; font-family=System; font-size=11pt; width=30; border=0" onMouseOver="document.sidcal.pie.style.background='#BA2B2C'" onMouseOut="document.sidcal.pie.style.background='#a9a9a9'" onMouseDown="document.sidcal.pie.style.background='#BA2B2C'">
</td></td></td></td>
	</tr>
<table border=0 cellspacing="3">
<hr color=black>
	<tr>
<td align="center">
<input type="text" name="pow1" value="" size="8" style="background:#FFF1F1; color:black; font-family:system; font-size:12pt; border:0">
<td align="center">
<input type="text" name="pow2" value="" size="8" style="background:#FFF1F1; color:black; font-family:system; font-size:12pt; border=0">
</td></td>
</tr>
<tr>
<td align="center">
<input type="button" name="powAnswer" value="Calculate" onClick="power_2(this.form)" style="background=#a9a9a9; color=black; font-family=System; font-size=11pt; width=80; border=0" onMouseOver="document.sidcal.powAnswer.style.background='#BA2B2C'" onMouseOut="document.sidcal.powAnswer.style.background='#a9a9a9'" onMouseDown="document.sidcal.powAnswer.style.background='#BA2B2C'">
<td align="center">
<a href="javascript:menus('helpPower','visible')" class="howTolink">How To?</a>
<div id="helpPower">
Put a number in the first box.
In the second box, put the
number of times you want the
first box to be mutiplied by itself.<br>
<a href="javascript:menus('helpPower','hidden')">Close</a>   <input type="button" name="example" value="Example" onClick="helpexample(this.form, '2', '3', '8')" style="background=#C13534; color=black; font-family=System; font-size=11pt; width=60; border=0">
</div>
</td></td>
</tr>
</table>
</table>
</div>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<div id="madeBySid" align="center">Made By Sid<br><a href="C:\My Documents\Sid\SidCal\SidCal.txt" class="sourceCode">Source Code</a></div>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
</body>
</html>
```

