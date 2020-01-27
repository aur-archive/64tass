# Contributor: lobotomius at gmail dot com
# Maintainer: lobotomius at gmail dot com

pkgname=64tass
pkgver=1.54.1900
pkgrel=1
pkgdesc="6502/65C02/R65C02/W65C02/65CE02/65816/DTV/65EL02 Turbo Assembler"
arch=('i686' 'x86_64')
url='http://tass64.sourceforge.net'
license=('GPL')
source=("http://downloads.sourceforge.net/project/tass64/source/64tass-$pkgver-src.zip")
md5sums=('a06434a6c8b82baafaa72126a2f7ef0e')
conflicts=("64tass-svn")

build() {
	cd "$srcdir/64tass-$pkgver-src"
	make
}

package() {
	cd "$srcdir/64tass-$pkgver-src"
	mkdir -p "$pkgdir/usr/bin"
	install -m 755 64tass "$pkgdir/usr/bin"
}
