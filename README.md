# wine-patch

A collection of wine patch for my self compile version of wine.

Support wine-staging 4.4.

To apply patches use `git apply *.patch` or `git am *.patch`.

# Patch Lists

    - 0001-patches/0001_wine-esync.patch
    Merged and rebased wine esync patch rev. ce79346 from https://github.com/zfigura/wine/releases

    - 0001-patches/0002_staging-config.patch
    Toggle upstream CSMT implementation patch from https://github.com/wine-staging/wine-staging/pull/60

    - 0001-patches/0003_avoid_closing_server_thread_handle_while_wait_on.patch
    rpcrt4: Avoid closing the server thread handle while it is being waited on.

    - 0001-patches/0004_remove_hook_that_timeout.patch
    user32: Remove hooks that time out.

    - 0001-patches/0005_enable_stg_shared_mem_def.patch
    ntdll: Enable STAGING_SHARED_MEMORY by default.

    - 0001-patches/0006_use_clock_monotonic.patch
    ntdll, server: Never use CLOCK_MONOTONIC_RAW
    Using CLOCK_MONOTONIC avoids a kernel call.

    - 0001-patches/0007_large_address_aware-staging.patch
    ntdll/loader: add support for overriding IMAGE_FILE_LARGE_ADDRESS_AWARE Staging version.

    - 0001-patches/0008_FS_bypass_compositor.patch
    Proton's Bypass compositor patch.

    - 0001-patches/0010-Added-support-for-Win-1-and-2-applications.patch
    Add support for Windows 1.x and 2.x applications.
    This is a patch file version of https://github.com/TransmissionZero/Wine

    - 0001-patches/0011-Add-OleIsCurrentClipboard-stub.patch
    Add OleIsCurrentClipboard stub.
    This make application like Microsoft Word 6.0 Thai Edition not crash when accessing clipboard.

    - 0002-winevdm/*.patch
    Patches ported from the winevdm project (wine on Windows) version 0.7.0, https://github.com/otya128/winevdm

    - 0003-wine-thaiapi/*.patch
    Patch set to add Thai language API from Windows 3.1/9x Thai Edition support to wine.
    From https://github.com/kytulendu/wine-thaiapi
    Note: Add OleIsCurrentClipboard stub patch is already included in 0001-patches directory.
