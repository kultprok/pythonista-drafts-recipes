# Manual

This script is pretty straight-forward. Provide a URL to shorten, send it to [is.gd](http://is.gd/) and copy the short-link to the clipboard.

- Open Drafts and create a new note.
- Type or paste a full URL, that you wish to shorten. Not less, not more.
- Choose the corresponding action and trigger it.
- Pythonista will open and run the script.
- In case of an error, Pythonista will show a dialog informing you about the type of error. Then the script will return to Drafts.
- In the more likely case of success. The script will open Drafts again, the shortened link was copied to the clipboard.

# Remarks

I chose *is.gd* because of its hassle-free API. There's no registration or login required. So there's no need to handle account credentials.