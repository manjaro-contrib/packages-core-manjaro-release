# Maintainer: Guinux <nuxgui@gmail.com>

pkgname=manjaro-release
pkgver=25.0.0
pkgrel=1
pkgdesc="Manjaro's release definition"
arch=("any")
url="https://manjaro.org/"
license=('GPL2')
depends=('lsb-release')
source=('lsb-release')
install="manjaro-release.install"
sha256sums=('1e930c9c30c82fbc697aaa9a88adbb4e3333a032f81a15a7512d797abc62ec31')

#pkgver() {
    #parse lsb-release
#    grep 'DISTRIB_RELEASE='  lsb-release | cut -d '=' -f2
#}

package() {
    # Copy files
    mkdir -p ${pkgdir}/etc
    install -m644 ${srcdir}/lsb-release ${pkgdir}/etc/
}
