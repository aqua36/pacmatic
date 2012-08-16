# $Id: PKGBUILD 75208 2012-08-16 04:54:54Z kkeen $
# Maintainer: Kyle Keen <keenerd@gmail.com>
pkgname=pacmatic
pkgver=20120816
pkgrel=1
pkgdesc="A pacman wrapper to avoid bricking your system and such other surprises."
arch=('any')
url="http://kmkeen.com/pacmatic/"
license=('GPL')
depends=('pacman' 'bash' 'wget' 'pacman-contrib' 'expac')
makedepends=()
optdepends=('vim: for vimdiff'
            'html2text: for prettier news')
source=(http://kmkeen.com/pacmatic/$pkgname-$pkgver.tar.gz)
md5sums=('e6c4177c18befdcafc81d1dffb75d6a2')

package() {
  cd "$srcdir/$pkgname"
  install -D -m 0755 $pkgname      "$pkgdir/usr/bin/$pkgname"
  install -D -m 0755 cron-$pkgname "$pkgdir/usr/bin/cron-$pkgname"
  install -D -m 0644 $pkgname.1    "$pkgdir/usr/share/man/man1/$pkgname.1"
}

