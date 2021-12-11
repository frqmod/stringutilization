# stringutilization

a basic python script for various string operations based around string utilization, requires angr

built 99.9% for personal use

```
usage: stringutil.py [-h] [-o OUTFILE] [-f FUNCTION] [-n NUMCHARS] [-s SEARCHSTRING] [-a ADDRESS] [-i] infile

positional arguments:
  infile                Input file

optional arguments:
  -h, --help            show this help message and exit
  -o OUTFILE, --outfile OUTFILE
                        Output file
  -f FUNCTION, --function FUNCTION
                        Function name to check for usage in
  -n NUMCHARS, --numchars NUMCHARS
                        Minimum number of printable characters for a string
  -s SEARCHSTRING, --searchstring SEARCHSTRING
                        Only show strings that contain this substring
  -a ADDRESS, --address ADDRESS
                        Attempts to find a string at a given address
  -i, --ignorenonuser   [EXPERIMENTAL] Attempts to ignore strings only found in library functions
```

---

more info:

this script uses angr to pull functions and their disassembly, and then process addresses/offsets to find potential strings locations, which are then checked for validity

the options are self explanatory, with the only two real notable highlights is the ability to filter based on function/string and the ability to attempt to ignore non-user strings, which is fancy jargon for only displaying strings used in functions that aren't known library functions
