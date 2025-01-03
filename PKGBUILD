# Maintainer: VHSgunzo <vhsgunzo.github.io>

pkgname='runimage-unionfs-fuse'
pkgver='3.5'
pkgrel='1'
pkgdesc='unionfs-fuse for RunImage container'
url='https://github.com/VHSgunzo/unionfs-fuse-static'
arch=('x86_64' 'aarch64')
license=('MIT')
provides=("unionfs-fuse=$pkgver-$pkgrel")
options=(!strip)
depends=('runimage-static')
source=("$url/releases/download/v$pkgver/unionfs-${CARCH}")
sha256sums=('SKIP')

package() {
  install -Dm755 "unionfs-${CARCH}" "${pkgdir}/var/RunDir/static/unionfs"
}
