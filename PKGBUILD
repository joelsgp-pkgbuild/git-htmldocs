# Maintainer: Victoria Mitchell <victoria@quietmisdreavus.net>
pkgname=git-htmldocs
pkgver=2.40.1
pkgrel=1
pkgdesc="HTML documentation files for Git"
arch=('any')
url="https://git-scm.com/"
license=('GPL2')
groups=()
depends=('git')
makedepends=()
checkdepends=()
optdepends=()
source=("https://www.kernel.org/pub/software/scm/git/$pkgname-$pkgver.tar."{xz,sign})
sha256sums=('8c08b31087566e719f6a7d16bb102255a8b9b970aefba6e306d6340eefe368ee'
            'SKIP')
validpgpkeys=('96E07AF25771955980DAD10020D04E5A713660A7') # Junio C Hamano

package() {
    install -Dm644 -t "$pkgdir/usr/share/doc/git-doc" *.html
    install -Dm644 -t "$pkgdir/usr/share/doc/git-doc/howto" howto/*.html
    install -Dm644 -t "$pkgdir/usr/share/doc/git-doc/technical" technical/*.html
}
