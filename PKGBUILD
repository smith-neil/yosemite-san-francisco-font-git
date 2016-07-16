# Maintainer: Neil Smith smith.neil.h@gmail.com

_pkgname=YosemiteSanFranciscoFont

pkgname=YosemiteSanFranciscoFont-git
pkgver=1.0.r0.g6bdbc49
pkgrel=1
pkgdesc="San Francisco font - the Apple Watch font"
arch=('any')
url="https://github.com/smith-neil/YosemiteSanFranciscoFont"
license=('GPL')
groups=()
depends=()
makedepends=('git')
provides=($_pkgname)
source=('git+https://github.com/smith-neil/YosemiteSanFranciscoFont.git')
md5sums=('SKIP')

pkgver() {
    cd "$srcdir/$_pkgname"
    git describe --tags --long | sed -r -e 's,^[^0-9]*,,;s,([^-]*-g),r\1,;s,[-_],.,g'
}

package() {
    cd -la "$srcdir/$_pkgname"
    cp 'System San Francisco Display Bold.ttf' /usr/share/fonts/TTF
    cp 'System San Francisco Display Regular.ttf' /usr/share/fonts/TTF
    cp 'System San Francisco Display Thin.ttf' /usr/share/fonts/TTF
    cp 'System San Francisco Display Ultralight.ttf' /usr/share/fonts/TTF
}
