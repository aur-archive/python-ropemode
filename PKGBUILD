# Maintainer: Allen Li <darkfeline at abagofapples.com>
# Submitter: Moikz
pkgname=python-ropemode
pkgver=0.2
pkgrel=2
pkgdesc="a helper for using rope refactoring library in IDEs"
arch=('any')
url="http://rope.sourceforge.net/ropevim.html"
license=('GPL')
depends=('python-rope')
conflicts=('ropemode')
replaces=('ropemode')
source=(http://pypi.python.org/packages/source/r/ropemode/ropemode-$pkgver.tar.gz)
md5sums=('9aec4e6f777bf1b245467642fa36d180')

build() {
  cd "$srcdir/ropemode-$pkgver"
  2to3 -wn ropemode/decorators.py
  python setup.py install --root=$pkgdir --prefix=/usr --optimize=1
}
