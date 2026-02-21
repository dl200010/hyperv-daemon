# app-emulation/hyperv-daemon
This is an init.d script for Hyper-V daemon that is in tools/hv in the Linux Kernel.

# Why
I wrote this because there was no init script for the Hyper-V daemon

# Dependencies

* sys-kernel/gentoo-sources, or any other source based kernel that has the files in question

# How to Use

* Emerge the dependencies above.
* Follow: https://wiki.gentoo.org/wiki/Hyper-V
* cd /usr/src/linux
* make
* cd tools/hv
* make install
* Install the files in the gentoo folder by
  * Coping the files, or
  * Use the https://github.com/dl200010/dl-overlay portage overlay and "emerge app-emulation/hyperv-daemon".
    * This will install the dependencies above.
* rc-update add hv_kvp_daemon default
* /etc/init.d/hv_kvp_daemon start

# Forks, Patches, Testers, Comments, etc.

Welcome.

# Author

* Chris Dangerfield
* e-mail: dl200010@gmail.com

# License

Copyright 2019 Christopher Dangerfield <DL200010@gmail.com>

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
