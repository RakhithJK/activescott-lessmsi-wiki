# Reference information on the MSI & CAB file formats.

# References on MSI & CAB File Format

## MSI Files/Databases

### Tables

MSI files are essentially a relational database. So the Tables are the key to MSI databases. The key reference page from Microsoft that documents what all the tables are is at http://msdn.microsoft.com/en-us/library/aa368259(v=vs.85).aspx

### Important Tables

- [File Table](http://msdn.microsoft.com/en-us/library/aa368596(v=vs.85).aspx)
- [Component Table](http://msdn.microsoft.com/en-us/library/aa368007(v=vs.85).aspx)
- [Directory Table](http://msdn.microsoft.com/en-us/library/aa368295(v=vs.85).aspx)
- [Media Table](http://msdn.microsoft.com/en-us/library/aa369801(v=vs.85).aspx)
- [_Streams Table](https://msdn.microsoft.com/en-us/library/windows/desktop/aa372919(v=vs.85).aspx)
- [_Storages Table](https://msdn.microsoft.com/en-us/library/windows/desktop/aa372916(v=vs.85).aspx)

### Notes on `_Streams` and `_Storages` Tables
...and how they related to embedded OLE Streams:
* [Extract Files from Patches - Setup & Install by Heath Stewart](https://blogs.msdn.microsoft.com/heaths/2006/02/14/extract-files-from-patches/)


## CAB File Format Notes

~~Just in case I ever stop procrastinating about implementing a CAB reader that is not dependent upon the Windows API below are some references that I have compiled on the CAB file format~~ - **Been there done that:** https://github.com/activescott/libmspack4n
- [Microsoft's Windows Cabinet API Reference](http://msdn.microsoft.com/en-us/library/gg547636(v=vs.85).aspx)
- CAB File Format info from MS: http://msdn.microsoft.com/en-us/library/bb417343.aspx
- [libmspack](http://www.cabextract.org.uk/libmspack/) Is an open C library that deals with CAB format on `*`nix. No dependencies.
- In lessmsi we created a .NET wrapper around a minor fork of libmspack and use it to decompress cabs. It brings lessmsi one step closer to working on mac/linux and was more interesting (and probably easier) than using the windows cabinet API. The code for that is at http://code.google.com/p/lessmsi/source/browse/?repo=libmspack4n
- http://www.cabextract.org.uk/wince_cab_format/
- http://msdn.microsoft.com/en-us/library/bb267310(VS.85).aspx
- http://www.ddj.com/184410186;jsessionid=30Q2P0IQ3EA4XQE1GHPSKH4ATMY32JVN?*requestid=420442
- http://msdn.microsoft.com/en-us/library/aa367841%28VS.85%29.aspx
- http://en.wikipedia.org/wiki/Cabinet*%28file_format%29