# Maintainer: Jon Gjengset <jon@thesquareplanet.com>
pkgname=cryptsetup-gui
pkgver=0.6.1
pkgrel=1
epoch=
pkgdesc="Simple GUI for unlocking LUKS encrypted devices"
arch=('any')
url="http://csg.thesquareplanet.com"
license=('MIT')
groups=()
depends=('glib2' 'cryptsetup')
makedepends=('gcc' 'glib2')
conflicts=()
replaces=()
install=$pkgname.install
changelog=
source=("http://csg.thesquareplanet.com/release/$pkgname-$pkgver.tar.gz")
noextract=()
md5sums=('a3b0058d6c0439b99b6e435ef61977f0')

build() {
  cd "$srcdir/$pkgname-$pkgver"
  make
}

package() {
  cd "$srcdir/$pkgname-$pkgver"
  make DESTDIR="$pkgdir/" install
}

# vim:set ts=2 sw=2 et:
