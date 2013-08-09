# Discusses future plans for the project.

Below are some broad plans for the project. **Comments & feedback are greatly appreciated! Please leave your suggestions/feedback below!**

# v2.0

Will be a release collecting a series of commonly requested feedback from customers including [support for MSI Patch Files (.msp)](http://code.google.com/p/lessmsi/issues/detail?id=2), [support for external CAB files](http://code.google.com/p/lessmsi/issues/detail?id=7), [a new explorer verb](http://code.google.com/p/lessmsi/issues/detail?id=6), and more...


# Misc

## Add support for Mac / Linux

### Cons

- Requires pretty significant effort:
- ~~Remove dependency on CAB Win32 libs~~ - done using libmspack.
- Remove dependency on Win32 libraries for MSI
Notes:
- WINE has some MSI features, so apparently the format is known to some extent.
- CAB file format is well documented now by MS.

### Pros

- Infinitely more useful on these platforms since MSI is not supported at all.
- Interesting to work on.

## Add MSI Editing Features

Some ideas on this area:
- Add ability to detect and fix the NoImpersonate flag on custom actions (this was requested by a user and recorded at http://code.google.com/p/lessmsi/issues/detail?id=3 )
- Add features to change values in tables (and summary) & "repackage" the MSI. Was mentioned at http://serverfault.com/questions/54386/i-want-to-install-an-msi-twice/54401#54401
- Add features to allow changing files that are in an MSI.
- *Is this useful to people?*