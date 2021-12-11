# stringutilization

basic python script for various string operations, requires angr

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
