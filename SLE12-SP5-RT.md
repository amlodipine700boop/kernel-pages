---
title: SLE12-SP5-RT branch
redirect_from: /branches/SLE12-SP5-RT/
---
# SLE12-SP5-RT
This is the SLE 12 SP5 RT kernel branch.

The persons in charge of this branch are:
Mel Gorman <[mgorman@suse.de](mailto:mgorman@suse.de?subject=SLE12-SP5-RT%20branch)>
Frederic Weisbecker <[fweisbecker@suse.de](mailto:fweisbecker@suse.de?subject=SLE12-SP5-RT%20branch)>
Jeffrey Cheung <[jcheung@suse.com](mailto:jcheung@suse.com?subject=SLE12-SP5-RT%20branch)>

It is the above person's responsiblity for checking in this kernel to
the build system, anyone else who wishes to do so, needs to get
permission from them first.

If there are any questions about this branch, please contact the above
mentioned maintainer.


## [packages](https://download.opensuse.org/repositories/Kernel:/SLE12-SP5-RT)
To install
[prebuilt kernel](https://download.opensuse.org/repositories/Kernel:/SLE12-SP5-RT)
from this branch run

```
zypper ar -f https://download.opensuse.org/repositories/Kernel:/SLE12-SP5-RT/default \
    Kernel:SLE12-SP5-RT
zypper in --from Kernel:SLE12-SP5-RT kernel-default
```

Please note: The packages are built for the distribution they are
targetting. In case of the vanilla and linux-next branches, this is the
latest released openSUSE version. While the packages should work fine on
fine on a distribution that is slightly newer or slightly older,
installing ancient kernels on the latest distributions is asking for
trouble. Same goes for the opposite case, e.g. installing the Factory
kernel on SLES 9.

## [kernel-source.git](https://github.com/openSUSE/kernel-source/tree/SLE12-SP5-RT)
There are two SUSE Kernel repositories. Development happens in the
[kernel-source](https://github.com/openSUSE/kernel-source/tree/SLE12-SP5-RT)
git repository. This tree is a quile-like series of patches against the
upstream kernel, plus spec files and various scripts. You can clone it
with

```
git clone https://github.com/openSUSE/kernel-source -b SLE12-SP5-RT
```

## [kernel.git](https://github.com/openSUSE/kernel/tree/SLE12-SP5-RT)
If you just want to hack on the sources and do not need to package the
kernel, use the [kernel](https://github.com/openSUSE/kernel/tree/SLE12-SP5-RT)
git repository. This one has the same layout as the upstream kernel. Clone
command:

```
git clone https://github.com/openSUSE/kernel -b SLE12-SP5-RT
```


