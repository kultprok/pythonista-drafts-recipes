# Manual

This script will work like a command-line tool to replace the string in a given text. The output of the help-command looks like this:

    usage: search-and-replace.py [-h] [-old STRING|REGEXP] [-new STRING] [-c INT]
                               [-f INT|re.FLAG]
                               [STRING [STRING ...]]
    
    Search and Replace for Drafts.
    
    positional arguments:
      STRING                the string to search in
    
    optional arguments:
      -h, --help            show this help message and exit
      -old STRING|REGEXP, --old STRING|REGEXP
                            the old string. regular expression allowed.
      -new STRING, --new STRING
                            the new string to replace with.
      -c INT, --c INT, -count INT, --count INT
                            the number of times to replace.
      -f INT|re.FLAG, --f INT|re.FLAG, -flags INT|re.FLAG, --flags INT|re.FLAG
                            the flags for regeular expression substitution.

# Remarks

Possible inputs for flags:

    2 = IGNORECASE
    4 = LOCALE
    8 = MULTILINE
    16 = DOTALL
    64 = VERBOSE