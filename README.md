# NaturalStringComparer
Compare for string to sort by number in string (as windows explorer do)
This is an easy to use and useful little library for programs that want to sort string naturaly by numbers.
you know 2 is lower than 11 but C# default string comparer not know this or not like this.
so you may lile to use my lib for a human friendly string comparing and sorting.

```
var stringList = new List<string>
            {
                "number1", "number2", "number3", "number4", "number10", "number15", "number22", "number26"
                , "number9", "number33", "number5", "number12"
            };
foreach(var item in stringList)
{
  Console.WriteLine(item)
}
stringList.Sort(NaturalStringComparer.Default);
/*
list will be like this () :
number1
number2
number3
number4
number5
number9
number10
number12
number15
number22
number26
number33
*/
```
