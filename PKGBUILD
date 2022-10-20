# Maintainer: Sergej Pupykin <pupykin.s+arch@gmail.com>
# Contributor: Morgan LEFIEUX <comete_AT_archlinuxfr.org>
# Contributor: Colin Wee <2gbleh@gmail.com>

pkgname=python-lzo
pkgver=1.14
pkgrel=1
pkgdesc="Python bindings for the LZO data compression library"
arch=('x86_64')
url="https://pypi.python.org/pypi/python-lzo"
license=('GPL2')
makedepends=()
source=("https://pypi.org/packages/source/p/python-lzo/python-lzo-$pkgver.tar.gz")
sha256sums=('83cbd8ecaae284735250e31d6c0ecc18ac08763fab2a8c910dc5a6910db6250c')

build() {
  cd "$srcdir/python-lzo-$pkgver"
  python setup.py build
}

package() {
  cd "$srcdir/python-lzo-$pkgver"
  python setup.py install --skip-build --optimize=1 --root "$pkgdir"
}
