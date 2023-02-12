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

```
#searching for the string "Lucayans"
$ grep -r -l "Lucayans" written_2/
written_2/travel_guides/berlitz2/Bahamas-History.txt

```
