# Maintainer: jhillix <sandboxlinux@gmail.com>

pkgname=hwifo
pkgver=21.53
pkgrel=1
pkgdesc="Hardware information tool"
arch=('arm')
url="http://www.linuxintro.org/wiki/Hwinfo"
license=('GPL')
groups=('base-devel')
depends=('glibc')

#makedepends=()
#checkdepends=()
#optdepends=()

source=("https://github.com/openSUSE/$pkgname")
md5sums=('SKIP')

prepare() {
	cd "$pkgname"
	git checkout "$pkgver"
}

build() {
	cd "$pkgname"
	make
}

check() {
	cd "$pkgname"
	make -k check
}

package() {
	cd "$pkgname"
	make install
}
