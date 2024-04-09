<<<<<<< HEAD
# Maintainer: Joar Heimonen <joarheimonen@live.no>
# Note: This is only an install script for Yuma123, not the actual project itself.

pkgname=yuma123-git
pkgver=latest
pkgrel=1
pkgdesc="Open-source YANG API in C and CLI (yangcli) and server (netconfd)"
arch=('x86_64')
url="https://github.com/vlvassilev/yuma123"
license=('BSD')
depends=('git' 'autoconf' 'automake' 'make' 'gcc')
makedepends=('libtool') # Add libtool as a build dependency
provides=("${pkgname%-git}")
conflicts=("${pkgname%-git}")
pkgbase=yuma123-git

source=("git+https://github.com/vlvassilev/yuma123")

prepare() {
  cd "$srcdir/yuma123"
  libtoolize
  autoreconf -i -f
}

build() {
  cd "$srcdir/yuma123"
  ./configure CFLAGS='-g -O0' CXXFLAGS='-g -O0' --prefix=/usr
=======
# Maintainer: Frédéric Bogaerts <fred@netpack.pt>

pkgname=xfb
pkgver=1.23
pkgrel=1
pkgdesc="Open-source Radio Automation"
arch=('x86_64')
url="https://github.com/netpack/XFB"
license=('GPL2')

depends=('qt5-base' 'qt5-tools' 'qt5-webkit' 'qt5-multimedia' 'perl-image-exiftool' 'ffmpeg' 'soundconverter' 'lame' 'sox' 'mplayer' 'audacity' 'mediainfo')
makedepends=('qt5-tools')


source=("https://github.com/netpack/XFB/releases/download/v1.23/xfb-1.23.tar.gz")

sha512sums=("b92a5a48a64a26b5c43c0d696736328fd17cb7a65aa85c9bda9b4bc45a8bd0ff05644767e10547dac0c2a57f81f4d1356c5c34db860f3731f49b2e4c2e01a656")


build() {
  cd "$srcdir/usr/share/xfb/bin"
  qmake-qt5 PREFIX=/usr/share/xfb/bin ../src/XFB.pro
>>>>>>> 5d48ff1 (XFB initial commit to AUR)
  make
}

package() {
<<<<<<< HEAD
  cd "$srcdir/yuma123"
  make DESTDIR="${pkgdir}" install
  mv "${pkgdir}/usr/sbin" "${pkgdir}/usr/bin"
}


sha256sums=('SKIP') 
=======
  # Create necessary directories
  install -d "$pkgdir/usr/bin"
  install -d "$pkgdir/etc/xfb"
  install -d "$pkgdir/usr/share/xfb"
  install -d "$pkgdir/usr/share/xfb/bin"
  install -d "$pkgdir/usr/share/xfb/config"
  install -d "$pkgdir/usr/share/xfb/scripts"
  install -d "$pkgdir/usr/share/xfb/jingles"
  install -d "$pkgdir/usr/share/xfb/music"
  install -d "$pkgdir/usr/share/xfb/playlists"
  install -d "$pkgdir/usr/share/xfb/recordings"
  install -d "$pkgdir/usr/share/xfb/tmp"
  install -d "$pkgdir/usr/share/xfb/ftp"
  install -d "$pkgdir/usr/share/applications"
  install -d "$pkgdir/usr/share/pixmaps"

  # Install additional files
  install -m644 usr/share/xfb/config/* "$pkgdir/usr/share/xfb/config"
  install -m644 usr/share/xfb/scripts/* "$pkgdir/usr/share/xfb/scripts"
  install -m755 usr/share/xfb/bin/* "$pkgdir/usr/share/xfb/bin"
  install -m644 etc/xfb/* "$pkgdir/etc/xfb"

  cp -r usr/share/xfb/ftp usr/share/xfb/jingles usr/share/xfb/music usr/share/xfb/playlists "$pkgdir/usr/share/xfb/"

    # Install .desktop file
  install -m644 usr/share/xfb/XFB.desktop "$pkgdir/usr/share/applications/"

  # Install icon file
  install -m644 usr/share/xfb/xfb_icon.png "$pkgdir/usr/share/pixmaps/"


  chmod +x "$pkgdir/usr/share/xfb/config/adb.db"

  # Create symbolic link in /usr/bin
  ln -s "/usr/share/xfb/bin/XFB" "$pkgdir/usr/bin/XFB"

  # Change ownerships
  #chown "$USER:$USER" "$pkgdir/etc/xfb/xfb.conf"
  #chown "$USER:$USER" "$pkgdir/usr/share/applications/XFB.desktop"
  #chown "$USER:$USER" "$pkgdir/usr/share/pixmaps/xfb_icon.png"
  chown -R "$USER:$USER" "$pkgdir/usr/share/xfb"

  echo "Installation of XFB completed successfully!"
  echo "The configuration file is: /etc/xfb/xfb.conf"
  echo "The shared folders are under: /usr/share/xfb"
  echo "You may want to install youtube-dl"
  echo "Can you share some ETH? 0x9700225FcD115230C9166BD68CEdc23e329D3CdF"
  echo "Thank you for installing XFB! I hope you enjoy it! Made with love & linux!"
}



>>>>>>> 5d48ff1 (XFB initial commit to AUR)
