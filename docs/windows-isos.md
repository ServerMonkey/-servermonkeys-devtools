# Note on Microsoft Windows ISO files

Microsoft does not provide legacy releases of Windows. In fact they are
actively removing links to Windows ISO files.

This is a nightmare for security researchers and system administrators. Because
this makes it more or less impossible to create automated download scripts. How
can you research a specific version of an operating system, if it is not
available?

If you want to use Windows in a deterministic way. You have to get the ISO
files elsewhere. As of writing this document you can
search [archive.org](https://archive.org/) for older releases. But it is
probably just a matter of time before the links change or disappear.

The website [files.rg-adguard.net](https://files.rg-adguard.net/) provides a
collection of hashes. In this way you can at least determine if the files you
have are correct.

If you need to build a deterministic environment offline, it is a good idea to
host your own internal archive of Windows ISO's.
