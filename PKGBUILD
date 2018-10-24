pkgname=pce
pkgver=20180722
pkgrel=1
pkgdesc='Micro Computer Emulator PCE'
url='http://www.hampa.ch/pce/'
arch=('x86_64')
license=('GPLv2')
source=()

prepare() {
	ln -snf "$startdir" "$srcdir/$pkgname"
}

build() {
	cd "$pkgname"
	./configure
	make
}

package() {
	cd "$pkgname"
	make DESTDIR="$pkgdir" install
}
