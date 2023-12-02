---
layout: post
title: "VMware Tools installation fails on Windows 2000"
date: 2023-12-02 14:25:00 +0200
categories: fix
---

Installing VMware Tools on [Windows 2000](https://winworldpc.com/product/windows-nt-2000/final) isn't very straightforward.

First and foremost, you need to be on Service Pack 4. [You can find it here.](https://winworldpc.com/product/windows-nt-2000/patches)

You might still run into errors despite having installed the Service Pack, though. One such error is `Microsoft Runtime DLLs cannot be installed on this operating system. Please see Microsoft KB835732 for details.`

![Microsoft Runtime DLLs cannot be installed on this operating system. Please see Microsoft KB835732 for details.](/assets/img/win2k_vmware-tools_fail_error.png)

# Solution

In order to fix this, you'll need to download the update mentioned in the error message.

You can find KB835732 here:

- [Microsoft Update Catalog](https://www.catalog.update.microsoft.com/Search.aspx?q=KB835732).
- [(Archived) Microsoft Update Catalog](https://catalog.s.download.windowsupdate.com/msdownload/update/v3-19990518/cabpool/windows2000-kb835732-x86-enu_7b7d1dffd9347af2c166bfcecc4782c.exe)
- [Internet Archive](https://archive.org/details/20231202_20231202_1258)

Use a program like [ImgBurn](https://www.imgburn.com/) to make an ISO out of the update file in order to mount it to the VM.
