# wine-win16-enhancements

A collection of patches to improve Win16 application on wine.

I'll update the patches against lastest version of wine if needed.

Support wine 3.13 or higher.

To apply patches, copy all patches to wine source code directory and `git apply *.patch` or `git am *.patch`.

# Patches Lists

- 0001-Added-support-for-Win-1-and-2-applications.patch

This is a patch file version of https://github.com/TransmissionZero/Wine

This patch add support for Windows 1.x and 2.x applications.

- 0002-Add-OleIsCurrentClipboard-stub.patch

This patch add OleIsCurrentClipboard stub, this make application like Microsoft Word 6.0 Thai Edition not crash when accessing clipboard.
