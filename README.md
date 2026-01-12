# Python-43
Write a Python class to convert an integer to a roman numeral.
class roman_solution:
def int_to_Roman(num):
val = [1000, 900, 500, 400, 100, 90, 50, 40, , 9, 5, 4, 1]

syb = [&quot;M&quot;, &quot;CM&quot;, &quot;D&quot;, &quot;CD&quot;, &quot;C&quot;, &quot;XC&quot;, &quot;L&quot;, &quot;XL&quot;,&quot;X&quot;, &quot;IX&quot;, &quot;V&quot;, &quot;IV&quot;, &quot;I” ]
roman_num = “”
i = 0
if(n&lt;1 or n&gt;3999):
print(&quot;ENTER A GOOD VALUE!&quot;)
else:
while num &gt; 0:
if(num-val[i]&gt;=0):
roman_num+=syb[i]
num-=val[i]
else:
i+=1

return roman_num n=int(input(&quot;ENTER A NUMBER:&quot;))
print(&quot;roman numeral of given number is:&quot;,roman_solution.int_to_Roman(n))


Output:
ENTER A NUMBER:
Roman numeral of given number is: MMCDVIII

