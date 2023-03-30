# Maintainer: DarkXero <info@techxero.com>
pkgname=universal-arch-linux-sys-utility
_destname1="/"
pkgver=1.0.0
pkgrel=1
pkgdesc="a univeral system utility for Arch"
arch=('any')
url="https://github.com/hhk02"
license=('GPL3')
makedepends=('git')
depends=('zenity')
conflicts=()
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}/${pkgname}")
sha256sums=('SKIP')
package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
	rm "${pkgdir}${_destname1}/PKGBUILD"
}
