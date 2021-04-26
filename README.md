## MyOwnGrimoire

Some XFCE updates for the Source Mage "test" grimoire. 

Use at your own risk.

### Some Details : 

- libxfce4menu, libxfcegui4 have been removed, they're deprecated
- notification-daemon-xfce not needed anymore and libsexy won't cast
- xfce-utils, xfce4-iconbox, xfce4-mixer pretty old and useless as far as I know
- thunar-vfs removed as well, deprecated too
- squeeze has a thunar-vfs dependency, I don't know yet if gvfs would do the job

- updated dependency for xfwm4 and ristretto
- updated version for almost everything else
- removed all gpg sig
- added sha hash when it was missing

- xfmedia is discontinued, has been removed
- xfdiff pretty old and not really worth the struggle
- updated thunar to 4.16.6

### Plugins
 - thunar-archive-plugin DONE : updated to 0.4.0
 - thunar-dropbox NOT YET : updated to 0.3.1, new SOURCE_URL + clean dependencies + cmake instead of waf, still requires dropbox 
	- dropbox runtime done by nautilis dropbox, which require nautilus, which require gnome...
	- so basically thunar-dropbox plugin = cast gnome, need to sort this ...
 - thunar-media-tags-plugins DONE : updated to 0.3.0
 - thunar-thumbnailers REMOVED : not needed annymore for thumbnails
 - thunar-vcs-plugin DONE : updated to 0.2.0
 - thunar-volman DONE : updated to 4.16.0
 - verve-plugin DONE : renamed to xfce4-verve-plugin for consistancy, updated to 2.0.1
 - xfce4-battery-plugin DONE : updated tp 1.1.4, can't test it unfortunately
 - xfce4-cddrive-plugin REMOVED 
 - xfce4-cellmodem-plugin REMOVED
 - xfce4-clipman-plugin DONE : updated to 1.6.1
 - xfce4-cpufreq-plugin DONE : updated to 1.2.5
 - xfce4-cpugraph-plugin DONE : updated to 1.2.3
 - xfce4-datetime-plugin DONE : updated to 0.8.1 not better than the default panel clock nowadays ...
 - xfce4-diskperf-plugin DONE : updated to 2.6.3
 - xfce4-eyes-plugin DONE : updated to 4.5.1
 - xfce4-fsguard-plugin DONE : updated to 1.1.2
 - xfce4-genmon-plugin DONE : updated to 4.1.0
 - xfce4-gvfs-mount REMOVED
 - xfce4-mailwatch-plugin DONE : updated to 1.3.0
 - xfce4-mount-plugin DONE : updated 1.1.5
 - xfce4-mpc-plugin DONE : updated to 0.5.2
 - xfce4-netload-plugin DONE : updated to 1.4.0
 - xfce4-notes-plugin DONE : updated to 1.9.0
 - xfce4-palces-plugin DONE : updated to 1.8.1, updated dependencies (thunar-vfs removed)
 - xfce4-quicklauncher-plugin REMOVED
 - xfce4-screenshooter-plugin REMOVED
 - xfce4-sensors-plugin DONE : updated to 1.3.95, I don't have what it takes to test it
 - xfce4-smartbookmark-plugin DONE : updated to 0.5.2
 - xfce4-systemload-plugin DONE : updated to 1.3.1
 - xfce4-wavelan-plugin DONE : updated to 0.6.2
 - xfce4-weather-plugin NOT FINISHED : updated to 0.11.0 but can't update location, don't know why
 - xfce4-xkb-plugin DONE : updated to 0.8.2
	- require liblzma.la to compile, hence the modified xz-utils spell

