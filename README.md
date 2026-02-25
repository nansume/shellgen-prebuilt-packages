# Prebuilt Packages for Bootstrap

Prebuilt binaries packages from shellgen-ports for bootstrap.

---

## Features

* Prebuilt packages for x32 (amd64-linux-muslx32)
* Some prebuilt packages for amd64 (amd64-linux-musl)
* Some prebuilt packages for x86 (i686-linux-musl)
* Some prebuilt packages for x32 (amd64-linux-dietlibcx32)
* Some prebuilt packages for amd64 (amd64-linux-dietlibc)
* Some prebuilt packages for x86 (i686-linux-dietlibc)
* Some packages build as static
* Toolchain packages build as static

---

## Requirements

- Linux kernel v4.19.* (probably older kernel same working) or later
   .config: CONFIG_X86_X32=y
- For static build packages no required libc
- Musl libc for packages build as shared (optional)

---

## Manual Install

From user:
```
$ cd ${HOME}/download
$ mv busybox_1.37.0_x32.clz busybox_1.37.0_x32.cpio.lzo
$ lzop -dc busybox_1.37.0_x32.cpio.lzo | cpio -u -i -m -p /tmp/busybox_1.37.0_x32
```

From root:
```
% cp -r /tmp/busybox_1.37.0_x32/* /mnt/chroot
```

---

## License

This work is multi-licensed under either GPLv3 or MIT license or UnLicense.

 * GNU GPLv3 [LICENSE.GPLv3](http://www.gnu.org/licenses/gpl-3.0.html)
 * MIT license [LICENSE.MIT](https://github.com/nansume/www-get-ip/raw/master/LICENSE.MIT)
 * UnLicense [UNLICENSE](https://github.com/nansume/www-get-ip/raw/master/UNLICENSE)
 * 
