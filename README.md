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
	-- dropbox runtime done by nautilis dropbox, which require nautilus, which require gnome...
	-- thunar-dropbox plugin => gnome ...
 - thunar-media-tags-plugins DONE : updated to 0.3.0
 - thunar-thumbnailers REMOVED : not needed annymore for thumbnails
 - thunar-vcs-plugin DONE : updated to 0.2.0
 - thunar-volman DONE : updated to 4.16.0
 - verve-plugin DONE : renamed to xfce4-verve-plugin for consistancy, updated to 2.0.1

