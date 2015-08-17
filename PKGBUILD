# Maintainer: slowpoke <mail+aur@slowpoke.io>>
#
pkgname=uguu
pkgver=1.2.0
pkgrel=1
pkgdesc="generate Flexget config files for downloading series"
arch=(any)
url="https://github.com/proxypoke/uguu"
license=('custom:Anti-License')
depends=('python' 'python-yaml')
optdepends=('flexget: to actually use the generated configs')
makedepends=('unzip')
options=(!emptydirs)
source=("https://github.com/proxypoke/uguu/archive/v${pkgver}.zip")
md5sums=('105cdfb5ae5d9f83b61f28c68cdfa5ae')


package() {
  cd "$srcdir/$pkgname-$pkgver"
  python setup.py install --root="$pkgdir/" --optimize=1
}

# vim:set ts=2 sw=2 et:
