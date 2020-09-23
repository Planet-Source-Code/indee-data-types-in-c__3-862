<div align="center">

## Data Types In C


</div>

### Description

As I discussed in an earlier article, I am writing a series of articles explaining C

for beginners. I am very careful to avoid the use of technical jargon so that it is

simpler for beginners. And also I will be writing very simple codes and then explain

about it. If you are an expert please skip this article.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Indee](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/indee.md)
**Level**          |Beginner
**User Rating**    |4.3 (13 globes from 3 users)
**Compatibility**  |C, C\+\+ \(general\)
**Category**       |[Documents](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/documents__3-27.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/indee-data-types-in-c__3-862/archive/master.zip)





### Source Code

<HTML>
<HEAD>
<META HTTP-EQUIV="Keywords" CONTENT="C Language">
<META NAME="Generator" CONTENT="RCEdit 32-bit HTML Editor">
<META NAME="Author" CONTENT="Inder Mohan Singh">
<TITLE>Data Types in C</TITLE>
<STYLE type=text/css>
<!--
 BODY{font-family: Arial; font-size:12pt;margin-left:0.5cm}
 TABLE{margin-left:1cm}
 P{margin-left:0.5cm; margin-right:0.5cm;}
 H1{color:#5f9ea0; font-size:20pt}
 H4{margin-left:0.5cm;color:#0000FF}
 B{background:#fffacd}
-->
</STYLE>
</HEAD>
<BODY>
<CENTER>
<H1><B>DATA TYPES IN C</B></H1></CENTER><BR>
<H4>Introduction</H4>
<P>As I discussed in an earlier article, I am writing a series of articles explaining C
for beginners. I am very careful to avoid the use of technical jargon so that it is
simpler for beginners. And also I will be writing very simple codes and then explain
about it. If you are an expert please skip this article.</P>
<P> Ok lets start with the real business. Here is another sample code for you.</P><BR>
<H4>Another Example of C Program</H4>
<TABLE border=0 cellPadding=0 cellSpacing=0 width="70%">
 <TBODY>
 <TR>
  <TD align=left bgColor=#f0f8ff><FONT color=#ff0000>
<P>#Include &lt; stdio.h &gt;<br><BR>
/* Sample Program - feet to metres. */<BR><BR>
void main(void)<BR><BR>
{<BR>
&nbsp;&nbsp;&nbsp; int feet;<BR>
&nbsp;&nbsp;&nbsp; float metres;<BR>
&nbsp;&nbsp;&nbsp;printf("Enter number of feet: ");<BR>
&nbsp;&nbsp;&nbsp;scanf("%d", &feet);<BR>
&nbsp;&nbsp;&nbsp;metres = feet * 0.3048; /* feet to metre conversion */<BR>
&nbsp;&nbsp;&nbsp;printf ("%d feet is %f metres\n", feet, metres);<BR><BR>
}<BR></P></TD></TR></FONT></TBODY></TABLE><BR>
<H4>Explanation</H4>
<P>Some important new concepts are introduced. First, two variables are declared:feet
is an <B>integer</B> and metres is of type <B>float</B>, which means that it can have a fractional
component.</P>
<P>The library function <B>scanf()</B> is used to read an integer entered at the keyboard.
The <B>%d</B> in the first argument causes <B>scanf()</B> to read an <B>integer</B> and to place the results
in the variable that follows. The <B>& </B>in front of feet is necessary for <B>scanf()</B> to work
properly.</P>
<P>The next statement converts the number of feet to metres. Notice that even though
feet is an <B>integer</B>, it may be divided by <B>floating-point </B>number and assigned to a
<B>floating-pont</B> variable. C allows different types of data to be used in an expresssion.
</P>
<P>The conversion is displayed using a call to <B>printf()</B>. In this statement, <B>printf()</B> takes three arguments: the<I> control string,</I> and the variables feet and metres. The general rule for <B>printf() </B>is that there are as many arguments following the control string as there are format codes in the control string. Since there are two format codes, two additional arguments are needed. These arguments are matched in order, from left to right, with the format codes. If you look closely, you will notice that <B>%f </B>is used to print metres, not <B>%d.</B> This is because <B>printf()</B> must know precisely what type of data it is going to display.</P>
<P>One limitations to this sample program is that it can convert only whole numbers of feet into metres. A more flexible program would also be able to convert floating-point values into integers. That I will leave it to you guys to think and convert this program. Ok!!</P>
<H4>Choosing Data Types</H4>
<P>There are six basic data types in C:</P>
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <B>chararcter</B><BR>
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <B>short integer</B><BR>
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <B>long integer</B><BR>
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <B>floting point</B><BR>
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <B>double floting point</B><BR>
<P>The keywords used to declare variables of these types are <I>char, short,, int, long, float </I>and <I>double</I>.</P>
<P>The following table summarises the sizes for the C data types on an IBM PC or compatible.</P>
<CENTER><TABLE BORDER="0" CELLSPACING="0" CELLPADDING="0">
<TR>
	<TD bgColor=#f0f8ff><B>Type</B></TD>&nbsp; &nbsp;&nbsp; &nbsp;
	<TD bgColor=#f0f8ff ALIGN="RIGHT"><B>Number of Bits</B></TD>
</TR>
<TR>
	<TD bgColor=#f0f8ff>char</TD>
	<TD bgColor=#f0f8ff ALIGN="RIGHT">8</TD>
</TR>
<TR>
	<TD bgColor=#f0f8ff>short</TD>
	<TD bgColor=#f0f8ff ALIGN="RIGHT">16</TD>
</TR>
<TR>
	<TD bgColor=#f0f8ff>int</TD>
	<TD bgColor=#f0f8ff ALIGN="RIGHT">32</TD>
</TR>
<TR>
	<TD bgColor=#f0f8ff>long</TD>
	<TD bgColor=#f0f8ff ALIGN="RIGHT">32</TD>
</TR>
<TR>
	<TD bgColor=#f0f8ff>float</TD>
	<TD bgColor=#f0f8ff ALIGN="RIGHT">32</TD>
</TR>
<TR>
	<TD bgColor=#f0f8ff>double</TD>
	<TD bgColor=#f0f8ff ALIGN="RIGHT">64</TD>
</TR>
</TABLE>
</CENTER>
<P>The <B>int</B>, <B>short</B> and long<B></B> types are signed, with one bit used to indicate the sign. An unsigned integer has the full number of bits available to store the number itself. If storage is concern, you can take advantage of the size differences among the types. </P>
<P>Type <B>char </B>may be used for very small values (0 to 255) because it requires less storage space - 8 bits only rather than 16 bits for <B>short </B>or 32 bits for type <B>int</B>. For example <B>ASCII</B> ( American Standard Code for Information Interchange) codes are usually stored in char variables. Type char may be used for true/false and yes/no situations, where true or yes is represented by a value 1, and false or no is represented by a value of 0. Finallly, type <B>char </B>is used to store character strings.</P>
<P>Floating-point variables are used to store real numbers (numbers involving decimals). The above table showed type float provides 32 bits while type double provides 64 bits. Size is not the only factor when choosing between type float and type double. You must also consider the precision required. Type float provides approx. 7 digits of precision while double provides 15 digits of precision.(Precision is the number of digits storef before the value is rounded off.)</P>
<P>All types of variables are declared in the same way. Simply enter the variable type followed by one or more variables names and semi-colon. The following are examples:</P>
<CENTER><TABLE BORDER="0" CELLSPACING="0" CELLPADDING="0">
<TR>
	<TD BGCOLOR="#80FFFF">char keypress;
</TD>
</TR>
<TR>
	<TD BGCOLOR="#80FFFF">int length, width, area;</TD>
</TR>
<TR>
	<TD BGCOLOR="#80FFFF">long distance;</TD>
</TR>
<TR>
	<TD BGCOLOR="#80FFFF">float average;</TD>
</TR>
<TR>
	<TD BGCOLOR="#80FFFF">double mass;</TD>
</TR>
</TABLE>
</CENTER>
<P>A variables can be initialise by giving it an initial value. Constants are often used for initialisation. An integer constant is any number without a decimal point or an exponent. A character constant must be enclosed be enclosed by single quotes unless it is part of a string of characters encloed by double quotes. Types int, char and long can all be initialised with character constants.</P>
<P>A floating point constant is a signed series of digits including a decimal p oint and/or an E oe e(for exponent) followed by a signed exponent indicating the power of 10 to be used. It cannot contains spaces. Below are two formats that can be used to initialise a variable with a constant:</P>
<CENTER><TABLE BORDER="0" CELLSPACING="0" CELLPADDING="0">
<TR>
	<TD BGCOLOR="#80FFFF">int kilograms = 21;</TD>
</TR>
</TABLE>
</CENTER>
<P>or</P>
<CENTER><TABLE BORDER="0" CELLSPACING="0" CELLPADDING="0">
<TR>
	<TD BGCOLOR="#80FFFF">int kilograms;</TD>
</TR>
<TR>
	<TD BGCOLOR="#80FFFF">kilograms = 21;</TD>
</TR>
</TABLE>
</CENTER>
<P>Be sure the constants used meet the various type requirements.</P>
<P>Ok guys! thats enough for this tutorial next tutorial will be about <B>Characters And Strings</B>.</P>
<P>Bye for now!</P>
</BODY>
</HTML>

