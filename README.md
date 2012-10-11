# Magento Boilerplates #

This repo contains the familiar magento folder structure with
boilerplate code sprinkled within. Nice for when you want to create new
modules, skins or templates.

Have your own Magento boilerplates? Send a pull request!

## Using these boilerplates ##

A tool to automatically generate custom modules, controllers and other
Magento files is in the works. For now, you can manually replace any
template placeholder found within each of the files.

### Placeholder Tags ###

These boilerplates contain different placeholders that allow custom
values to be placed throughout. Placeholders come in two flavors:

 * Variable Placeholders:
   	`{{VariableName}}`
 * Extended Information:
    ```
    {:Example:}
		Some content
	{:/Example:}
	
	{:Details:}
		Some detailed information
	{:/Details:}
    ```

#### Variable Placeholders ####

Throughout the boilerplate templates, different variable placeholders
are used. These variables look like ``{{VariableName}}` and can be
replaced throughout the scripts with the values they represent.

#### Extended Information ####

These boilerplates contain a great amount of instruction for those who
are just starting out using Magento. Information that is above and
beyond normal commentry are encapsulated within different extended
information tags. These tags take the form of `{:TagName:}` and
`{:/TagName:}`. The following tag names are currently defined:

 * Example
	- Defines a section of the boilerplate that is an example.
 * Details
	- Defines a section of the boilerplate that contains in depth
	details.

### File/Folder Name Placeholder Tags ###

Througout the folder structure, you will find files or folders named
with `[VariableNameHere]`. When generating the boilerplates, files or
folders whose names contain `[VariableName]` will have the variable (and
dashes) replaced with the variable's value (the dashes are removed as
well). Note, the case of the variable is important (see the next
section).

### Variable Naming Conventions ###

A couple of conventions are used when using Variable Placeholders
(either in file/folder names or within the actual text documents).
Whever a variable needs to be Title Cased (OneTwoThree), the variable
name MUST start with an uppercase letter (example: `{{VariableName}}`,
or `[VariableName]` if the variable is within a file/folder name).
When a variable needs to be lowercase (onetwothree), the variable name
MUST start with a lowercase letter (example `{{variablename}}` or
`[variablename]`).
