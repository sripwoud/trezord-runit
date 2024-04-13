# Maintainer: sripwoud <me@sripwoud.xyz>
_pkgname=trezord
pkgname=${_pkgname}-runit
pkgver=1.0
pkgrel=1
pkgdesc="Custom ${_pkgname} runit service"
arch=('any')
url="https://github.com/sripwoud/${_pkgname}-runit"
license=('AGPL-3.0-only')
depends=('runit' 'trezord-git')
source=("run" "run.asc")
validpgpkeys=('D99B40AC0CE81A5FF8B8456F6296216946C1B36A')
sha256sums=('221ef4580ba61621d9da32ea54a7a9b8e7ff7615155f46c68e4c2e1f7d8ccf96' 'SKIP')
install=run.install

package() {
    install -Dm755 "${srcdir}/run" "${pkgdir}/etc/runit/sv/${_pkgname}/run"
}
