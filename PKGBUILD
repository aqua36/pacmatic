# $Id: PKGBUILD 64963 2012-02-19 00:42:02Z kkeen $
# Maintainer: Kyle Keen <keenerd@gmail.com>
pkgname=pacmatic
pkgver=20120218
pkgrel=1
pkgdesc="A pacman wrapper to avoid bricking your system and such other surprises."
arch=('any')
url="http://kmkeen.com/pacmatic/"
license=('GPL')
depends=('pacman' 'bash' 'wget' 'pacman-contrib' 'expac')
makedepends=()
optdepends=('vim: for vimdiff')
source=(http://kmkeen.com/pacmatic/$pkgname-$pkgver.tar.gz)
md5sums=('4b67febe76e3bed7b88c4d4a4c460256')

package() {
  cd "$srcdir/$pkgname"
  install -D -m 0755 $pkgname      "$pkgdir/usr/bin/$pkgname"
  install -D -m 0755 cron-$pkgname "$pkgdir/usr/bin/cron-$pkgname"
  install -D -m 0644 $pkgname.1    "$pkgdir/usr/share/man/man1/$pkgname.1"
}

