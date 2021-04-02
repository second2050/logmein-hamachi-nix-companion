# Maintainer: second2050 (karui [at] waifu [dot] club)

pkgname=logmein-hamachi-nix-companion
_pkgname=logmein-hamachi
pkgver=1
pkgrel=1
pkgdesc='systemd unit file for logmein-hamachi installed via nix'
arch=('any')
license=('unlicense')
depends=('nix')
provides=('logmein-hamachi')
conflicts=('hamachi'
		   'logmein-hamachi')

source=("${_pkgname}.service")
sha1sums=('8842813d1ee57e47302550e13e55dc704b394c5d')

package() {
    cd ${pkgdir}
    mkdir -p "usr/lib/systemd/system"
    cd ../..
	install -m 644 "${_pkgname}.service" "${pkgdir}/usr/lib/systemd/system/${_pkgname}.service"
}
