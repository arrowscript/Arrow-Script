#INITIAL TODO LIST
#
Here is the progress of the project.
#
#ESSENTIALS
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Try [Libreboot] [libreboot] or [Coreboot] [coreboot].
#
![done] (http://s8.postimg.org/vzpt8pj3l/Check_32.png)  Build ArchLinux core with [GNU/Linux-Libre kernel] [gnukernel], compiled with flags for specific archtecture (-o3 -match=*arch-here*) and then apply [Real Time patch] [rtpatch] and [`patch BFS Kolivas`] [kernel] or try [Repo-ck] [repock], enabling the [BFQ I/O Scheduler] [bfq] and Update system. [re]Check system with these [scripts] [deblob] ;
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Test Network conection (script only will work with internet);
#
![inprogress] (http://s22.postimg.org/w7fyxlg2l/Media_Play_32.png)  Implement Hardware Detection (specify here);
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Telemetry using IP address to configure automatic Time Zone and Language;
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png)  Basic's configurations;
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png)  Bootloader (EFI using [Gummiboot] [gummi] and BIOS using [GRUB2] [grub]);
#
#Hard Drive Manager
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png)  Provide a 'Help Guide' to Wipe disk ([SSD Memory Cell Clearing] [cellclean]), create GPT, partitioning, verify 4kb sector disk alignment and formating;
#
  [BRTFS] [btrfs] to SSD/Hibrid and [XFS] [xfs] to HDD.
#
#
XFS custom:
#
`inode64 nobarrier unmask_irq unwritten=0 agcount -l size=128m logbsize=256k lazy-count=1 noatime nodiratime relatime noquota delaylog -b size=64KB`
#
BRTFS custom: 
#
`noatime nobarrier nodatacow nodatasum ssd ssd_spread space_cache compress=lz4`
#
Note: for LZ4 compression use patch.
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png)  Make [`FITRIM`] [fitrim].
#
#Graphics libs and Drivers
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Install `current` proprietary drivers;
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) If nVidia, install too core integration [`CUDA`] [cuda]. Else, install [Catalyst™/Mantle] [catalyst] (AMD);
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Check [`MESA`] [mesa] and [`OpenGL`] [opengl] instalations;
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Install ALSA.
#AUR packages
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Install a [AUR Helper] [aurhelper]. We will use [`Pacaur`] [pacaur], because it is fast and don't need root acess, and don't make many questions like `Yaourt`;
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Reduce latency using [Ulatencyd] [ulatencyd] (seems to not work. Try to build from [Git] [gitulatency] and install libcgroup from [AUR] [libcgroup] - some tips of compiling [here] [tipulatency]), [Prelink] [prelink], [Preload] [preload] and [VeryNice] [verynice];
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Install [`Powerpill`] [powerpill];
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Install Network Manager [`ConnMan`] [connman];
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Install and config. [dnsmasq] [dnscache];
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Install [`HTOP`] [htop];
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Install [`MOC` player] [moc];
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Install [`P7ZIP`] [p7zip] (make LZMA2 was default);
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Install [`wlterm`] [wlterm] (terminal for Wayland):
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Automatize Scripts to make backup's. Use compiled versions from the [Benchmarks] [compressbench] or [Silesia Benckmark] [silesia].
#
#Configurations
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Disable [SELinux] [selinux] (impact system around 7%);
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Systemd profiling;
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Use [`LZ4`] [lz4] has default compress algorithm;
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Cache and swappiness [configure] [swap];
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Disable `CPUfreq` (optional);
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Disable kernel modules [IPV6] [ipv6], `nls_utf8`, `nf_conntrack_netbios_ns` and `floppy`;
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Config. [`mkinitcpio`] [mkinitcpio].
#
#Composer and Desktop Environment
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png)  Compile [Wayland/Weston] [wayland] and configure;
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png)  Compile adn Configure [`QTwayland`] [qtwayland];
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png)  Install [`LXQT` DE] [lxqt];
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Install [`Infinality`] [infinality]:
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png)  Aditional config's.
#
#Network
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Compile Firefox Nightly from [Mercurial] [mercurial] with [Profile-Guided Optimization] [pgo] (disable features unusable);
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Install some Plugins by default: [UI Enhancer] [addonuienhancer], [Nightly Tester Tools] [nightlytool] (this will eliminate incompatibility with some addon's), [Youtube HTML5] [ythtml5] (Wayland have some troubles with Flash player), [Adblock Plus] [adblock] (with adition [filter lists] [adlist]), [Element Hide] [elementhide] and [VIM FX] [vimfx] (optional).
#
#Visual
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Make a custom default Wallpaper and some Design;
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Apply [Simple White] [designff] to Firefox.
#
#PLUS [forward]
#
![plus] (http://s30.postimg.org/3jwa5oc65/Add_New_32.png) Implement CLI (Command Line Interface);
#
![plus] (http://s30.postimg.org/3jwa5oc65/Add_New_32.png) Verify firmware of SSD and provide automatic updates;
#
![plus] (http://s30.postimg.org/3jwa5oc65/Add_New_32.png) RAID 0 'Help Guide'. [See] [noop].
#
#Cleanup finishing
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png)  Clean orphans;
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png)  Reboot.
#
#Research
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) See more about about [IRQ] [irq] settings;
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png)

Disable `zone_reclaim`.
Set (sysctl):

`vm.zone_reclaim_mode = 0` 

on /etc/sysctl.conf

(execute sysctl -p to load on kernel);
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) 
View more [about] [hugepage]: `/sys/kernel/mm/transparent_hugepage/enabled`;
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Enable NUMA interleaving for your application: run with numactl --interleave=all COMMAND ;
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) view more [NTK] [ntk]; 
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) View about [Kdbus] [kdbus];
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Patch BTRFS with LZ4 patch for compression. See [here] [lz4btrfs] and [here] [lz4btrfs1];
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png)
Configs:

`PREEMPT=y`
`CONFIG_1000_HZ=y`
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Try LLVM Linux [Clang to compile kernel] [kernelclang];
#
#
#
[cellclean]:https://wiki.archlinux.org/index.php/SSD_Memory_Cell_Clearing
[repock]: http://repo-ck.com
[kernel]:https://aur.archlinux.org/packages/linux-ck/
[gummi]: https://wiki.archlinux.org/index.php/Gummiboot
[grub]: https://wiki.archlinux.org/index.php/GRUB
[btrfs]: https://btrfs.wiki.kernel.org/
[xfs]: http://xfs.org/
[fitrim]: http://xfs.org/index.php/FITRIM/discard
[noop]: http://en.wikipedia.org/wiki/Noop_scheduler
[lz4]: https://github.com/Cyan4973/lz4/
[swap]: http://rudd-o.com/linux-and-free-software/tales-from-responsivenessland-why-linux-feels-slow-and-how-to-fix-that
[connman]: https://wiki.archlinux.org/index.php/Connman
[cuda]: https://developer.nvidia.com/cuda-downloads
[catalyst]: http://www.amd.com/en-gb/innovations/software-technologies/catalyst
[mesa]: http://www.mesa3d.org/
[opengl]: http://www.opengl.org/
[ipv6]: https://wiki.archlinux.org/index.php/IPv6_-_Disabling_the_Module#Disable_IPv6
[dns]: https://developers.google.com/speed/public-dns/?hl=pt-br
[mercurial]: https://developer.mozilla.org/en-US/docs/Mozilla/Developer_guide/Source_Code/Mercurial
[addonuienhancer]: https://addons.mozilla.org/en-US/firefox/addon/ui-enhancer/
[nightlytool]: https://wiki.mozilla.org/Auto-tools/Automation_Development/Projects/Addons/NightlyTesterTools
[ythtml5]: https://addons.mozilla.org/en-US/firefox/addon/youtube-all-html5/?src=api
[adblock]: https://adblockplus.org/en/firefox
[adlist]: https://adblockplus.org/en/subscriptions
[vimfx]: https://addons.mozilla.org/en-US/firefox/addon/vimfx/
[designff]: https://addons.mozilla.org/en-US/firefox/addon/simplewhite/?src=cb-dl-users
[mkinitcpio]: https://projects.archlinux.org/mkinitcpio.git
[aurhelper]: https://wiki.archlinux.org/index.php/AUR_Helpers
[pacaur]: https://wiki.archlinux.org/index.php/Pacaur
[powerpill]: https://wiki.archlinux.org/index.php/Powerpill
[htop]: http://hisham.hm/htop/
[moc]: http://moc.daper.net/
[p7zip]: http://p7zip.sourceforge.net/
[openrc]: https://wiki.manjaro.org/index.php?title=OpenRC,_an_alternative_to_systemd
[infinality]: http://www.infinality.net/blog/infinality-freetype-patches/
[lxqt]: lxqt.org
[wayland]: http://wayland.freedesktop.org/
[qtwayland]: http://qt-project.org/wiki/QtWayland
[wlterm]:  http://lists.freedesktop.org/archives/wayland-devel/2012-September/005529.html
[zpaq]: https://github.com/zpaq/zpaq
[compressbench]: http://mattmahoney.net/dc/text.html
[ulatencyd]: https://aur.archlinux.org/packages/ulatencyd-git/
[bfq]: https://wiki.archlinux.org/index.php/linux-ck#How%20to%20enable%20the%20BFQ%20I/O%20Scheduler
[prelink]: https://www.archlinux.org/packages/community/x86_64/prelink/
[preload]: https://aur.archlinux.org/packages/preload/
[verynice]: https://aur.archlinux.org/packages/verynice/
[dnscache]: https://www.archlinux.org/packages/extra/x86_64/dnsmasq/
[gitulatency]: https://github.com/poelzi/ulatencyd
[libcgroup]: https://aur.archlinux.org/packages/libcgroup/
[tipulatency]: https://aur.archlinux.org/packages/ulatencyd-git/?comments=all
[selinux]: http://selinuxproject.org/page/Main_Page
[pgo]: https://developer.mozilla.org/en-US/docs/Building_with_Profile-Guided_Optimization
[elementhide]: https://addons.mozilla.org/en-us/firefox/addon/elemhidehelper/?src=cb-dl-users
[silesia]: http://mattmahoney.net/dc/silesia.html
[gnukernel]: http://www.fsfla.org/ikiwiki/selibre/linux-libre/
[rtpatch]: https://rt.wiki.kernel.org/index.php/Main_Page
[libreboot]: http://libreboot.org/
[coreboot]: http://coreboot.org/
[deblob]: http://www.fsfla.org/svn/fsfla/software/linux-libre/scripts/
[irq]: http://wiki.linuxaudio.org/wiki/lowlatency_deprecated
[hugepage]: https://access.redhat.com/documentation/en-US/Red_Hat_Enterprise_Linux/6/html/Performance_Tuning_Guide/s-memory-transhuge.html
[ntk]: http://non.tuxfamily.org/wiki/NTK
[kdbus]: https://github.com/gregkh/kdbus
[lz4btrfs]: https://github.com/miaoxie/linux-btrfs
[lz4btrfs1]: http://www.spinics.net/lists/linux-btrfs/msg17407.html
[kernelclang]: http://git.linuxfoundation.org/llvmlinux.git/
