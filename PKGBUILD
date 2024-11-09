pkgname=netlogin
pkgver=1.0.2
pkgrel=1
pkgdesc="Netlogin"
arch=("x86_64")
url="https://github.com/xingjianxu/archpkg-netlgin"
license=('Apache License 2.0')
source=("${pkgname}" 
				"${pkgname}.service"
				"${pkgname}.timer")
depends=("curl")
sha256sums=('a96cfd5c5940010c7eb1333e629ddebf8ac424a5291a39cee4a450a37d93e36b'
            '6ccfa6cc31590a26853fca2365cff2512447c6a98985c6a821bea0c952afd642'
            '44b8c428c57b105ce30bb1b59b5eeaaa9771d7771143778b69caea13c9b70aa1')
package() {
  install -Dm755 "${pkgname}" "${pkgdir}/usr/bin/${pkgname}"
	install -Dm644 "${pkgname}.service" "${pkgdir}/usr/lib/systemd/system/${pkgname}.service"
	install -Dm644 "${pkgname}.timer" "${pkgdir}/usr/lib/systemd/system/${pkgname}.timer"
}
