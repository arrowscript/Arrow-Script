#INITIAL TODO LIST
#
Here is the progress of the project.
#
#ESSENTIALS
![done] (http://s8.postimg.org/vzpt8pj3l/Check_32.png)  Build ArchLinux core as custom [`kernel -ck`] [kernel], enabling the [BFQ I/O Scheduler] [bfq] and Update system;
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Test Network conection (script only will work with internet);
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Set [`Clang LLVM`] [clang] to default compiler;
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
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png)  Provide a 'Help Guide' to Wipe disk ([SSD Memory Cell Clearing] [cellclean]), create GPT, partitioning and formating;
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
`noatime nobarrier nodatacow nodatasum ssd ssd_spread`
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
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Reduce latancy using [`Ulatencyd`] [ulatencyd], [Prelink] [prelink] and [Preload] [preload];
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Install [`Powerpill`] [powerpill];
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Install Network Manager [`ConnMan`] [connman];
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Install [`HTOP`] [htop];
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Install [`MOC` player] [moc];
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Install [`P7ZIP`] [p7zip] (make LZMA2 was default);
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Install [`OpenRC`] [openrc]:;
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Install [`wlterm`] [wlterm] (terminal for Wayland):
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Install [`zpaq`] [zpaq] or the firt usable on the [benchmarks] [compressbench] of compression team. Use it just for backups and save some space !Caution! - really experimental and not garanted.
#
#Configurations
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Use [`LZ4`] [lz4] has default compress algorithm;
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Cache and swappiness [configure] [swap];
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Disable `CPUfreq` (optional);
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Disable [IPV6] [ipv6];
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
#Compile Firefox and addons
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Compile Firefox Nightly from [Mercurial] [mercurial];
#
![notdone] (http://s29.postimg.org/unjjnhs1v/Document_Error_01_32.png) Install some Plugins by default: [UI Enhancer] [addonuienhancer], [Nightly Tester Tools] [nightlytool] (this will eliminate incompatibility with some addon's), [Youtube HTML5] [ythtml5] (Wayland have some troubles with Flash player), [Adblock Plus] [adblock] (with adition [filter lists] [adlist]) and [VIM FX] [vimfx] (optional).
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
#
#
[cellclean]:https://wiki.archlinux.org/index.php/SSD_Memory_Cell_Clearing
[kernel]:https://wiki.archlinux.org/index.php/Linux-ck
[clang]: https://github.com/llvm-mirror/clang
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
