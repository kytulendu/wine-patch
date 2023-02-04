# wine-patch

A collection of wine patch for my self compile version of wine.

For wine-staging-tkg 7.20

https://github.com/Frogging-Family/wine-tkg-git

Put *.mypatch into `wine-tkg-git/wine-tkg-userpatches` directory

# Patch Lists

    - wine-tkg.cfg
    Customization file for wine-staging-tkg used by myself, put into ~/.config/frogminer/wine-tkg.cfg
    Addition patches in customization file is from https://github.com/Frogging-Family/community-patches

    - 0001-patches/0001-Added-support-for-Win-1-and-2-applications.mypatch
    Add support for Windows 1.x and 2.x applications.
    This is a patch file version of https://github.com/TransmissionZero/Wine

    - 0002-winevdm/*.mypatch
    Patches partially ported from the winevdm project (wine on Windows) version 0.8.1, https://github.com/otya128/winevdm
    Note: OLE stuff might not get ported, as wine's OLE support is limited.
    Remaining component to port:
        gdi.exe16
        user.exe16
        krnl386.exe16
        dispdib.dll16
        msacm.dll16
        shell.dll16
        system.drv16
        toolhelp.dll16
        win87em.dll16
        winnls.dll16
        winoldap
        winspool.drv
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
        haxmvm
        vm86

    - 0003-wine-thaiapi/*.patch
    Patch set to add Thai language API from Windows 3.1/9x Thai Edition support to wine.
    From https://github.com/kytulendu/wine-thaiapi
