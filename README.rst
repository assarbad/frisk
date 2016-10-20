====================================
 FRISK Software C++ utility classes
====================================

About
-----
These are a few utility classes originally published - with permission from Friðrik, the company owner at the time - some time before around 2010 on my Subversion server. Publishing it again now, since my Subversion server has been discontinued.

The classes were developed by me for FRISK while working on F-PROT Antivirus for Windows 6.x.

The classes are:

- ``CLoadLibrary`` which wraps loading a DLL (or other PE file), also as a data file, and gives access to certain aspects of the loaded DLL. It also has convenience functions to format messages based on a status code (``FormatMessage`` Win32 API).
- ``CSimpleBuf`` is used by ``CLoadLibrary`` and offers a very simple "string buffer" class which is convenient to use with Win32 APIs expecting a buffer. Thanks to its template class nature, it can be specialized for ``TCHAR``, ``WCHAR`` or ``CHAR``, as needed.
- ``CEnsureVersion`` derives from ``CLoadLibrary`` and allows to easily check against an expected version, based on the version resource of a DLL (or other PE file). It also allows to get a string representation of the version number expected and found.

License
-------
Copyright (C) FRISK Software International (FRISK)

The classes are licensed under the 3-clause BSD license as present in the file
header of the files.
