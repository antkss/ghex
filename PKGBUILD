# Maintainer: FabioLolix
# Maintainer: éclairevoyant
# Contributor: ThatOneCalculator <kainoa at t1c dot dev>

pkgname=mghex
pkgver=1
pkgrel=1
pkgdesc="nothing there"
arch=(x86_64)
license=(BSD)
conflicts=("ghex")


options=(!docs !debug)

prepare() {
    echo lmao
}

build() {
    cd $srcdir/../ghex
    meson setup build --prefix /usr --reconfigure
    ninja -C build
}

package() {
    cd $srcdir/../ghex
    meson install -C build --destdir $pkgdir --strip 
}
