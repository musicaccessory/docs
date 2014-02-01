{{Page_Title}}
{{Flags
|State=Ready to Use
|Editorial notes=
|Checked_Out=No
}}
{{Summary_Section|Right shifts the value of a variable by the number of bits specified in the value of an expression, without maintaining sign, and assigns the result to the variable.}}
{{JS_Syntax
|Formats={{JS Syntax Format
|Format=result '''&gt;&gt;&gt;=''' expression
}}
|Values={{JS Syntax Parameter
|Name=result
|Required=
|Description=Any variable.
}}{{JS Syntax Parameter
|Name=expression
|Required=
|Description=Any expression.
}}
}}
{{JS_Return_Value
|Description=
}}
{{Examples_Section
|Not_required=No
|Examples={{Single Example
|Language=JavaScript
|Description=See Remarks.
|Code=var temp;
temp = -14;
temp >>>= 2;
//result: temp = 1073741820

|LiveURL=
}}
}}
{{Remarks_Section
|Remarks=Using the &gt;&gt;&gt;= operator is exactly the same as doing the following:

 result = result &gt;&gt;&gt; expression
The '''&gt;&gt;&gt;=''' operator shifts the bits of result right by the number of bits specified in expression. Zeroes are filled in from the left. Digits shifted off the right are discarded.

The variable temp has an initial value of -14 (11111111 11111111 11111111 11110010 in two's complement binary). When shifted right two bits, the value equals 1073741820 (00111111 11111111 11111111 11111100 in binary).
}}
{{Notes_Section
|Usage=
|Notes=
|Import_Notes=
}}
{{JS Object Listing}}
{{Topics | JS Basic}}
{{See_Also_Section
|Manual_links=* [[javascript/operators/unsigned right shift{{!}}Unsigned Right Shift Operator (&#62;&#62;&#62;)]]
* [[javascript/operators/bitwise left shift{{!}}Bitwise Left Shift Operator (&#60;&#60;)]]
* [[javascript/operators/bitwise right shift{{!}}Bitwise Right Shift Operator (&#62;&#62;)]]
|External_links=
|Manual_sections=
}}
{{JS Topics
|JS Page Type=JS Basic
|Applies to=
}}
{{External_Attribution
|Is_CC-BY-SA=No
|Sources=MSDN
|MDN_link=
|MSDN_link=http://msdn.microsoft.com/en-us/library/ie/2ked96yw(v=vs.94).aspx
|HTML5Rocks_link=
}}