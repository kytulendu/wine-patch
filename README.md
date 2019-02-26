# wine-patch

A collection of wine patch for my self compile version of wine.

Support wine lastest version.

To apply patches, copy all patches to wine source code directory and `git apply *.patch` or `git am *.patch`.

# Patch Lists

- 0001_wine-esync.patch

wine esync patch rev. ce79346

- 0002_staging-config.patch

Toggle upstream CSMT implementation patch from https://github.com/wine-staging/wine-staging/pull/60

- 0003_avoid_closing_server_thread_handle_while_wait_on.patch

rpcrt4: Avoid closing the server thread handle while it is being waited on.

- 0004_remove_hook_that_timeout.patch

user32: Remove hooks that time out.

- 0005_enable_stg_shared_mem_def.patch

ntdll: Enable STAGING_SHARED_MEMORY by default.

- 0006_use_clock_monotonic.patch

ntdll, server: Never use CLOCK_MONOTONIC_RAW

Using CLOCK_MONOTONIC avoids a kernel call.

- 0007_large_address_aware-staging.patch

ntdll/loader: add support for overriding IMAGE_FILE_LARGE_ADDRESS_AWARE Staging version.

- 0008_FS_bypass_compositor.patch

Proton's Bypass compositor patch.

- 0009_Update_OpenCL.patch

Update wine OpenCL pass-thought to OpenCL 2.1, from https://github.com/kytulendu/wine-opencl

- 0010-Added-support-for-Win-1-and-2-applications.patch

Add support for Windows 1.x and 2.x applications. This is a patch file version of https://github.com/TransmissionZero/Wine

- 0011-Add-OleIsCurrentClipboard-stub.patch

Add OleIsCurrentClipboard stub, this make application like Microsoft Word 6.0 Thai Edition not crash when accessing clipboard.

- 01xx_winevdm_*.patch

Patch from the winevdm project (wine on Windows) rev. 8dbcdfc2, https://github.com/otya128/winevdm
