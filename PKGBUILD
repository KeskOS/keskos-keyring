pkgname=keskos-keyring
pkgver=0.1.0
pkgrel=1
pkgdesc="Placeholder package for the future KeskOS pacman signing keyring"
arch=(any)
url="https://github.com/memegeko/keskos"
license=(custom:KeskOS)
source=()
sha256sums=()

package() {
  install -D -m 644 "${startdir}/README.md" "${pkgdir}/usr/share/doc/${pkgname}/README.md"
  install -d "${pkgdir}/usr/share/pacman/keyrings"
  printf '%s\n' "KeskOS keyring placeholder package" >"${pkgdir}/usr/share/pacman/keyrings/keskos-placeholder"
}
