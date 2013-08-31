# Manual

Sometimes, Bitbucket servers are down. Bitbucket provides a feed to check the status of its servers.

Using the script via Drafts is easy. Just make a new note in Drafts, enter whatever you want - some whitespace for instance - and trigger the action. The script will then call the status API and then create a new note in Drafts with the latest status info.

# Remarks

- Drafts won't trigger, when a note is empty, so at least one character has to be provided.
- The feed only contains warnings and alerts. If there is no such warning for the current day, it means, the servers are probably fine.
