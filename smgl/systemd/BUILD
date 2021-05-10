if [[ "$SYSTEMD_GIT" == "y" ]]
then
  ./autogen.sh    --prefix=${INSTALL_ROOT}/ \
              --sysconfdir=${INSTALL_ROOT}/etc \
           --localstatedir=${INSTALL_ROOT}/var \
                  --mandir=${INSTALL_ROOT}/usr/share/man \
                 --infodir=${INSTALL_ROOT}/usr/share/info \
              --includedir=${INSTALL_ROOT}/usr/include \
               --localedir=${INSTALL_ROOT}/usr/share/locale \
            --with-rootdir=${INSTALL_ROOT}/ \
             --with-distro=other \
                           $OPTS
else
mkdir -p build &&
cd build &&
LANG=en_US.UTF-8                    \
meson --prefix=/usr                 \
      --sysconfdir=/etc             \
      --localstatedir=/var          \
      -Dblkid=true                  \
      -Dbuildtype=release           \
      -Ddefault-dnssec=no           \
      -Dinstall-tests=false         \
      -Dkmod-path=/bin/kmod         \
      -Dldconfig=false              \
      -Dmount-path=/bin/mount       \
      -Drootprefix=                 \
      -Drootlibdir=/lib             \
      -Dsplit-usr=true              \
      -Dsulogin-path=/sbin/sulogin  \
      -Dsysusers=false              \
      -Dumount-path=/bin/umount     \
      -Db_lto=false                 \
      -Drpmmacrosdir=no             \
      -Dman=true                    \
      -Dmode=release                \
#      -Ddocdir=/usr/share/doc/systemd-247 \
                           $OPTS
fi
ninja
