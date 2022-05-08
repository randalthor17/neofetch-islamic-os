# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Your Name <youremail@domain.com>
pkgname=neofetch-islamic-os
pkgver=7.1.1
pkgrel=1
pkgdesc="A CLI system information tool written in BASH that supports displaying images, patched to add Islamic OS logo."
arch=('any')
url="https://github.com/randalthor17/neofetch-islamic-os"
license=('MIT')
depends=('bash')
makedepends=('git')
optdepends=(
  'catimg: Display Images'
  'chafa: Image to text support'
  'feh: Wallpaper Display'
  'imagemagick: Image cropping / Thumbnail creation / Take a screenshot'
  'jp2a: Display Images'
  'libcaca: Display Images'
  'nitrogen: Wallpaper Display'
  'w3m: Display Images'
  'xdotool: See https://github.com/dylanaraps/neofetch/wiki/Images-in-the-terminal'
  'xorg-xdpyinfo: Resolution detection (Single Monitor)'
  'xorg-xprop: Desktop Environment and Window Manager'
  'xorg-xrandr: Resolution detection (Multi Monitor + Refresh rates)'
  'xorg-xwininfo: See https://github.com/dylanaraps/neofetch/wiki/Images-in-the-terminal'
)
provides=('neofetch')
conflicts=('neofetch')
backup=('etc/neofetch/config.conf')
source=("$pkgname-$pkgver.tar.gz::https://github.com/randalthor17/neofetch-islamic-os/releases/download/$pkgver-IslamicOS/release.tar.gz")
noextract=()
sha256sums=('6bff084471356a5d17c51a53ba5c4a714f28f9cf82327cc2262ca8c6e1e585b3')

package() {
	install -Dm644 neofetch.1 "${pkgdir}/usr/share/man/man1/neofetch.1"
	install -Dm755 neofetch "${pkgdir}/usr/bin/neofetch"
	install -Dm644 LICENSE.md "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE.md"
}
