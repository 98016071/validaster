# validaster
## Examples
Read two lengths and two strings of this lengths
```
#a:int #b:int
[a + b <= 1000000]
#string(a, a) #string(b, b)
```
Read n and n integers
```
#n:int
{int }*{n - 1} #int
```
Read n, m, then m edges with vertexes from 1 to n without edge from vertex to itself
```
#n:int #m:int
{#a:int(1, n) #b:int(1, n)
[a != b]
}*{m - 1}\
#a:int(1, n) #b:int(1, n)
[a != b]
```
Note that [] construction deletes line break before it if placed on newline, \ deletes line break after it
