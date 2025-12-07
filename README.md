# termux-proot-stuff

# Converting an `ubuntu-arm.qcow2` Disk Image Into a Root Filesystem Tarball

These are the steps we used to take an **Ubuntu ARM qcow2 image** on a Debian/LMDE host and turn it into a **root filesystem tarball** suitable for use with proot/Termux (or anything else that wants a plain rootfs).

> **Scope:**  
> This document goes only up to the point where we have a `rootfs.tar` file.  
> (No Android / Termux / proot steps included.)

---

## 0. Starting Point

- Host OS: Debian/LMDE (root shell).
- qcow2 file: e.g.

  ```bash
  /var/lib/libvirt/images/ubuntu-arm.qcow2

