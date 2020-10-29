# wine-patch

A collection of wine patch for my self compile version of wine.

For wine-staging-tkg 5.20

https://github.com/Frogging-Family/wine-tkg-git

# Patch Lists

    - 0001-patches/0001-Added-support-for-Win-1-and-2-applications.mypatch
    Add support for Windows 1.x and 2.x applications.
    This is a patch file version of https://github.com/TransmissionZero/Wine

    - 0002-winevdm/*.patch
    Patches ported from the winevdm project (wine on Windows) version 0.7.0, https://github.com/otya128/winevdm
    Note: OLE stuff might not get ported, as wine's OLE support is limited.
    Remaining component to port:
        dispdib.dll16
        haxmvm
        gdi.exe16
        krnl386.exe16
        shell.dll16
        system.drv16
        toolhelp.dll16
        user.exe16
        vm86
        win87em.dll16
        winnls.dll16
        winoldap
        winspool (winspool.drv)
        wow32
        widl
        compobj.dll16
        ole2.dll16
        ole2disp.dll16
        ole2nls.dll16
        olecli.dll16
        olesvr.dll16
        storage.dll16
        typelib.dll16

    - 0003-wine-thaiapi/*.patch
    Patch set to add Thai language API from Windows 3.1/9x Thai Edition support to wine.
    From https://github.com/kytulendu/wine-thaiapi
