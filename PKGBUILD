# Maintainer Eric Vidal <eric@obarun.org>

pkgname=oblibs
pkgver=0.0.0.1
pkgrel=1
pkgdesc='Obarun library'
url='https://github.com/Obarun/oblibs.git'
arch=(x86_64)
license=('ISC')
depends=()
makedepends=('git' 'skalibs')
sha1sums=('SKIP')
source=("${pkgname}::git+${url}#branch=master")
validpgpkeys=('6DD4217456569BA711566AC7F06E8FDE7B45DAAC') # Eric Vidal

build() {
	cd "$pkgname"
	./configure \
		--disable-shared
	make
}
package() {

  cd "$pkgname"
		 
  make DESTDIR="$pkgdir" install
}
