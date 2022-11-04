# Maintainer: Your Name <foobar@example.com>
pkgname=NAME
pkgver=VERSION
pkgrel=1
pkgdesc=''
arch=()
depends=()
focal_depends=()
makedepends=()
makedepends_x86_64=()
checkdepends=()
optdepends=()
focal_optdepends_x86_64=()
provides=()
conflicts=()
replaces=()
preinst=''
postinst=''
prerm=''
postrm=''
backup=()
options=()
license=()
url=''

source=()
sha256sums=()
noextract=()

prepare() {
    cd "${pkgname}-${pkgver}/"
    git submodule init
}

build() {
    cd "${pkgname}-${pkgver}/"
    make
}

package() {
    cd "${pkgname}-${pkgver}/"
    make DESTDIR="${pkgdir}/" install
}

# vim: set sw=4 expandtab:
