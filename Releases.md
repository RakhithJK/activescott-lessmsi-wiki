This page contains release notes about each release of the product.

# v1.1.3 - Aug 1, 2013

- Issue 43: You can now drag & drop .msi files onto the dialog and it will open them.
- Issue 50: The list of tables in the Table View tab now only lists tables that actually exist in the currently loaded msi.


# v1.1.1 - March 25, 2013

Major improvements to the console/command line interface. See CommandLine for documentation.
## New Features

- Issue 6:  Add another Explorer verb, command-line support for opening an MSI, not just Extract
- Issue 23: Add support for individual file extraction on command line
- Issue 36: Create Chocolatey Package & Ensure Published with Each Release
- Issue 26: Add another command line option to print table contents to a tab separated file
- Issue 45: Open file in GUI from command line
- Issue 47: Add command line - command load file in less msi
- Issue 40: Command line switch to specify the path for extracted files
- Issue 39: Command-line switch to extract MSI info (.MSI version)
## Fixes

- Issue 41 Keep original (archived) attributes and time stamps (date, time, etc.) for the extracted files
- Issue 46 Command prompt/console window briefly visible when strating lessmsi.
- Issue 44 Unhandled Exception when you cancel the Open File window


# v1.0.10 - February 14, 2013

- Fix for error that occured when selecting only some files to extract rather than all files (Issue 37).
- Data grid views are sortable (thanks to [@zippy1981](https://twitter.com/zippy1981)).
- File text input is reverted after loading a non-existant file (thanks to [@zippy1981](https://twitter.com/zippy1981)).
- About box with appropriate credits.
- Preferences dialog centers over main window now.

# v1.0.9 - January 27, 2013

v1.0.9 fixes Issue 28 where some msi files didn't get all files extracted. Also adds some UI improvements thanks to Justin Dearing ([@zippy1981](https://twitter.com/zippy1981)). Thanks Justin! 

**Note:** A new cab extraction library based on [libmspack](http://www.cabextract.org.uk/libmspack) is used to decompress cab files. This is a major change, so please report any problems. 
**Note:** For developers the [libmspack](http://www.cabextract.org.uk/libmspack) library was slightly modified and a wrapper library libmspackn to make it callable from .NET/Mono/CLI/C# applications was made. The code for this is in the  repo at http://code.google.com/p/lessmsi/source/list?repo=libmspack4n .


# v1.0.8 - December 5, 2010

Version 1.0.8 adds the following fixes and new features:
- Issue 10: (and Issue 14): Supports "type ahead" (autocomplete, intellisense) for the file textbox.
- Issue 11: Fixes context menu option when path of msi has spaces in it.
- Issue 15: The data grid columns are sized more intelligently and default size of window is larger.
- Issue 16: An unhandled exception could occur while extracting if you typed the wrong file name in.
- Issue 17: An list of most recently used msi files is now in the file menu.