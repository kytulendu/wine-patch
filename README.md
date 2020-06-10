# wine-patch

A collection of wine patch for my self compile version of wine.

Support wine-staging 5.9

To apply patches use `git apply *.patch` or `git am *.patch`.

# Patch Lists

    - 0001-patches/0001_staging-config.patch
    Toggle upstream CSMT implementation patch from https://github.com/wine-staging/wine-staging/pull/60

    - 0001-patches/0002_use_clock_monotonic.patch
    ntdll, server: Never use CLOCK_MONOTONIC_RAW
    Using CLOCK_MONOTONIC avoids a kernel call.

    - 0001-patches/0004_enable_stg_shared_mem_def.patch
    ntdll: Enable STAGING_SHARED_MEMORY by default.

    - 0001-patches/0005_plasma_systray_fix.patch
    winex11.drv: Fix system tray on KDE Plasma.
    From https://github.com/Tk-Glitch/PKGBUILDS/blob/master/wine-tkg-git/wine-tkg-patches/misc/plasma_systray_fix.patch

    - 0001-patches/0006_LAA-staging.patch
    ntdll/loader: add support for overriding IMAGE_FILE_LARGE_ADDRESS_AWARE

    - 0001-patches/0007_path_of_exile.patch
    ole32: Fix WIC error in Path of Exile.
    From https://bugs.winehq.org/show_bug.cgi?id=42695

    - 0001-patches/0008_FS_bypass_compositor.patch
    Proton's Bypass compositor patch.

    - 0001-patches/0009_Support-child-window-rendering-for-vulkan.patch
    winex11.drv: Support child window rendering for Vulkan via XComposite
    From https://bugs.winehq.org/show_bug.cgi?id=45277

    - 0001-patches/0010-Added-support-for-Win-1-and-2-applications.patch
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
