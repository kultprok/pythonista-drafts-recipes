# Manual

This script is designed to work like a command-line interface. The help option will produce the following output:

    usage: hasher.py [-h] [-hs HASH-NAME] [-u URL] [STRING [STRING ...]]
    input a string to hash.
    
    positional arguments:
    STRING                the string to hash
    
    optional arguments:
		-h, --help            show this help message and exit
		-hs HASH-NAME, --hs HASH-NAME, -hash HASH-NAME, --hash HASH-NAME the hash function of hashlib to use. defaults to sha1
		-u URL, --u URL, -url URL, --url URL url scheme to call after hashing. use to call an app.
		
Note that the default hash algorithm is SHA1. The result will be send to the clipboard. Then Drafts is opened, or another app that supports URL schemes.
	 
# Examples

The simplest input would be without any optional argument. It will send *505b32a013ac5e803f24579b99acb19b679e0a82* to clipboard. It's SHA1:

    this_is_a_test
   
Get the MD5 of the same string. It will send *05e4ad8f026394d064eb94b88ce4a0d4* to clipboard:

    this_is_a_test -hs md5
   
Get the SHA512 of that string, and open Chrome browser after calculating the hash. Will send *0d6ef2f011a4f8f02afb68fa0d39a98d4901c3c329c066fff3288c99181cd9bf47c92a3d2ceb38fbf07237f108fce3effcbe3fc2b84e4dac2394c2a8dd3bd5c9* to clipboard, and open Chrome:
    
	this_is_a_test -hs sha512 -u chrome://

# Remarks

You may enter all hash algorithms that are supported by Python's hashlib module. At the moment these are:

- MD5
- SHA1
- SHA224
- SHA256
- SHA384
- SHA512

For further information see: [hashlib Python Documentation](http://docs.python.org/2/library/hashlib.html)