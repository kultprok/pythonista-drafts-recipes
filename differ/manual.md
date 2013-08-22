# Manual

This script will work like a command-line tool to compare the content of two given texts. The output of the help-command looks like this:

'''
usage: differ.py [-h] [-f STRING [STRING ...]] [-t STRING [STRING ...]]
                     [-wc INT]

diff two texts.

optional arguments:
  -h, --help            show this help message and exit
  -f STRING [STRING ...], --f STRING [STRING ...], -from STRING [STRING ...], --from STRING [STRING ...]
                        the first text to compare
  -t STRING [STRING ...], --t STRING [STRING ...], -to STRING [STRING ...], --to STRING [STRING ...]
                        the second text to compare
  -wc INT, --wc INT, -wrapcolumn INT, --wrapcolumn INT
                        number of characters each column in diff should wrap
                        to
'''

The diff table will be shown in the default browser.

# Remarks

It will create a file called *diff_table.html* in the working directory.