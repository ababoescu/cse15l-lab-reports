**Researching the Command: grep**

**Grep -r -l:**
1. -r: searches the listed subdirectories recursively
2. -l: outputs the names of the matching files containing the inputed string only (will make the searches potentially less expensive)
```
#searching for the string "Claude"
$ grep -r -l "Claude" written_2/
written_2/non-fiction/OUP/Kauffman/ch5.txt
written_2/travel_guides/berlitz1/WhereToFrance.txt
written_2/travel_guides/berlitz1/WhereToFWI.txt
written_2/travel_guides/berlitz2/Costa-WhereToGo.txt
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt
written_2/travel_guides/berlitz2/Paris-WhereToGo.txt
```
The above example is searching for a file and the path to that file containing the string "Claude" in the written_2 directory. This command is helpful for searching the subdirectories recursively and will output the not only the names of the matching files containing the inputed string, but include their path so that the user can easily find which directories and subdirectories the file is located.
```
#searching for the string "Lucayans"
$ grep -r -l "Lucayans" written_2/
written_2/travel_guides/berlitz2/Bahamas-History.txt

```
Much the the example before, however this example is searching for the file containing the string "Lucayans" in the written_2 directory.



**Grep -v -e:**
1. -v: select lines that are not matching any of the specified patterns
2. -e: specifies a pattern used during the search of the input
```
#searching lines in file ch5.txt not containing the **strings** "is" and "a"
$ grep -v -e "is" -e "a" written_2/non-fiction/OUP/Kauffman/ch5.txt




Know-how
Knowing
Ethics



```
This example is finding all the lines in the file _ch5.txt_ that do not contain the strings "is" and "a" and returning them. This is helpful for locating lines that exclude strings that the user does not want such as "is" and "a", as shown from this example.
```
#searching lines in file ch5.txt not containing the **words** " is " and " a "
$ grep -v -e "is" -e "a" written_2/non-fiction/OUP/Kauffman/ch5.txt


Chapter 5
A Physics of Semantics?
Know-how
Unlike “know that,” “know-how” does not involve propositions about the world. “Know-how” involves procedural knowledge about how to get on in the world. The cheetah streaking after the wildebeest, the athletic genius high jumping, have the know-how to do it.
Semantics
All of which brings us, inevitably, to the brink of semantics.
Knowing
What about “knowing”?
I do not disagree, although I have placed far greater emphasis on the roles of self-organization in evolution. Here, in Investigations, I am trying to point at the mysterious but utterly natural hopefulness in which an increasing diversity of broken symmetries in the universe creates the diversity of structures and processes that can constitute and identify ramified and ramifying sources of energy, detect those sources of energy, create devices and processes that couple to those sources of energy, and generate yet more diversity that propagates macroscopic order even further. I wonder, in short, at the naturalness and self-generaticity of Dennett’s cranes building cranes building cranes in biospheres, perhaps planetary geologies, and beyond.
Ethics


```
This example is almost the same as the previous example, however in this example the command is used to find all the lines in the file _ch5.txt_ that do not contain the **words** "is" and "a" rather than the strings.


**Grep -e:**
-e: specifies a pattern used during the search of the input
```
#
$ grep -e "Claude " written_2/non-fiction/OUP/Kauffman/ch5.txt
The calculus that is Claude Shannon’s elegant information theory has always been about reduction of uncertainty about the statistics of the source of a set of symbols. Nowhere in the core of Shannon’s work concerning the encoding and transmission of information does the meaning, or semantics, of the information enter. This is no criticism, and is widely known and appreciated. There is, however, just a hint of semantics in Shannon’s view that the semantics resides in the “decoder.”
```
