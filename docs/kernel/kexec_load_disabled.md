---
layout: sysctl
title: kexec_load_disabled
sysctl-category: kernel
sysctl-file: /proc/sys/kernel/kexec_load_disabled
sysctl-variable: kernel.kexec_load_disabled
source: https://www.kernel.org/doc/Documentation/sysctl/kernel.txt
---

A toggle indicating if the kexec_load syscall has been disabled. This
value defaults to 0 (false: kexec_load enabled), but can be set to 1
(true: kexec_load disabled). Once true, kexec can no longer be used, and
the toggle cannot be set back to false. This allows a kexec image to be
loaded before disabling the syscall, allowing a system to set up (and
later use) an image without it being altered. Generally used together
with the "modules_disabled" sysctl.

