# Maintainer: DarkXero <info@techxero.com>
pkgname=calamares-xfce-cfg
_destname1="/etc"
pkgver=23.08
pkgrel=5
pkgdesc="calamares 3.3 Config for XeroCE"
arch=('any')
url="https://github.com/XeroLinux"
license=('GPL3')
makedepends=('git')
depends=()
conflicts=('calamares-config-dev')
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}/${pkgname}")
sha256sums=('SKIP')
package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
	rm ${srcdir}/${pkgname}/creds.sh
	rm ${srcdir}/${pkgname}/push.sh
	rm ${srcdir}/${pkgname}/README.md
	rm ${srcdir}/${pkgname}/PKGBUILD
}
