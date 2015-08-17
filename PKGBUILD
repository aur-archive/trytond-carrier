# Maintainer: Robin Baumgartner <robin@baumgartners.ch>
pkgname=trytond-carrier
_pkgname=trytond_carrier
pkgver=3.4.1
_pkgdir=3.4
pkgrel=1
pkgdesc="The carrier module of the Tryton application platform"
arch=('any')
url='http://www.tryton.org/'
license=('GPL3')
groups=('trytond-modules')
depends=('trytond>=3.4' 'trytond-party>=3.4' 'trytond-product>=3.4')
makedepends=('python2-distribute')
source=("http://downloads.tryton.org/$_pkgdir/$_pkgname-$pkgver.tar.gz")
md5sums=("92d501845b38af5493ff7333bacc4015")

build() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py build
}

package() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py install --root=$pkgdir
}