# Maintainer: lilydjwg <lilydjwg@gmail.com>
_name=svgwrite
pkgname=python2-${_name}
pkgver=1.1.3
pkgrel=1
pkgdesc="A Python library to create SVG drawings."
arch=('any')
url="http://bitbucket.org/mozman/svgwrite"
license=('MIT')
depends=('python')
makedepends=('python-setuptools')
md5sums=('01adbeae1d75741f515058120f761120')
source=("http://pypi.python.org/packages/source/s/${_name}/${_name}-${pkgver}.tar.gz")

build() {
  cd "$srcdir/$_name-$pkgver"

  python setup.py build
}

package() {
  cd "$srcdir/$_name-$pkgver"
  python2 setup.py install --root=$pkgdir/ --optimize=1
}
