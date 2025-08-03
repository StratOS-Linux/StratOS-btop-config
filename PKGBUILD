# Maintainer: @zstg <zestig@duck.com>
pkgname=stratos-mako-config
pkgver=1.0
pkgrel=1
pkgdesc="Btop configuration for StratOS"
arch=('any')
license=('GPL3')
depends=(
    'btop'
)
source=()
md5sums=('SKIP')
install=stratos-btop-config.install
prepare() {
    cp -r "$startdir/.config/" "$srcdir/"
}
package() {
    install -d "$pkgdir/etc/skel/.config"
    cp -r "$srcdir/.config/btop/" "$pkgdir/etc/skel/.config/"
}
