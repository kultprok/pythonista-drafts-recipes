pythonista-drafts-recipes
=========================

# The Short Description

A collection of short Python scripts for use in Pythonista on iOS. Triggered by using custom actions for Drafts.

=========================

# The Longer Description

## What's Pythonista?

Pythonista is a great IDE for Python on iOS devices. It actually is one of the finest IDEs for Python I know. It's well thought out and easy on the eyes, too. Pythonista vastly expands your options and possibilities to automate workflows under iOS.

[Give Pythonista a try](http://omz-software.com/pythonista/)

## And this Drafts thingy?

Don't judge Drafts only by its shining surface. It's not yet another, although beautiful, text editor or note-taking app. It supports URL schemes and allows to create your own actions. These actions are URL scheme calls to other apps, which makes Draft some sort of shell for all apps on your device, that support URL schemes.

[Drafts is here](http://agiletortoise.com/drafts/)

## So, now what?

You see, Pythonista gives you the power of Python on your iOS device, and it supports calling your own scripts via URL schemes. Get it? Pythonista + Drafts = Automation liberation. As easy as that.

## And those recipes?

The recipes are a collection of Drafts actions and Python scripts for Pythonista. They are intended to be called from within Drafts.

=========================

# The Recipes

All recipes are stored in their own subfolders. Each subfolder should at least contain:

- The python script file, e.g. *link_shortener_isgd.py*.
- A markdown file with an example Drafts action to trigger, e.g. *link_shortener_isgd_action.md*.
- A manual on how to call and use the script, e.g. *manual.md*.

=========================

# Automation helpers

## draftsaction

There's *draftsaction.py* which is intended to provide a class to easily create draft action links and import links for Drafts for any given script. Also, it should provide templates for manual and action markdown files. This is in an early stage right now.

### Attributes of DraftsAction class:

- name: The script's name to be referenced in documentation.
- action: The pythonista action that should be called from within Drafts.
- actiontitle: How the action should be called in Drafts.
- absolutepath: The absolute path to the Python script.
- importlink: A link to automatically import the action into Drafts.
- data: A dictionary containing all above data.

### Methods of DraftsAction class:

- data_update(): Update all data in data dictionary.
- drafts_action(*args): Create the Pythonista link to be called by Drafts action. args will be arguments of the Pythonista script.
- drafts\_import\_link(): Create the import link.
