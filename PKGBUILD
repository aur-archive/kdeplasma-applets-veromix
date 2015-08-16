# Maintainer: Tom Debruyne <tomdebruyne at gmail dot com>

pkgname=kdeplasma-applets-veromix
pkgver=0.18.3
pkgrel=7
pkgdesc="A plasmoid mixer for the Pulseaudio sound server"
url="http://code.google.com/p/veromix-plasmoid/"
license=('GPL3')
arch=('any')
depends=('kdebindings-python2' 'kdebase-workspace' 'python-pyqt4' 'pulseaudio' 'python-xdg')
optdepends=('swh-plugins: equalizer and other effects support')
conflicts=('kdeplasma-addons-applets-veromix')
replaces=('kdeplasma-addons-applets-veromix')
makedepends=()

source=(http://veromix-plasmoid.googlecode.com/files/2012-06-14_${pkgver}_veromix.plasmoid)
sha1sums=('b923d3f1e16def498050c15a33c410d809d91195')
package() {
  cd $srcdir

  install -dm755 ${pkgdir}/usr/share/apps/plasma/plasmoids/veromix-plasmoid 
  cp -R {contents,dbus-service,metadata.desktop} ${pkgdir}/usr/share/apps/plasma/plasmoids/veromix-plasmoid 
  install -Dm644 metadata.desktop ${pkgdir}/usr/share/kde4/services/plasma-applet-veromix-plasmoid.desktop 
  cd ${pkgdir}/usr/share/apps/plasma/plasmoids/veromix-plasmoid
}
