# Maintainer: Michael Wendland <dev@michiwend.com>

pkgname=gnome-shell-extension-arch-update
pkgver=14
pkgrel=1
pkgdesc="Update indicator for ArchLinux and Gnome-Shell"
arch=('any')
url="https://github.com/RaphaelRochet/arch-update"
license=('GPL3')
depends=('gnome-shell>=3.18')
provides=('gnome-shell-extension-arch-update')
conflicts=('gnome-shell-extension-arch-update')
source=("${pkgname}-${pkgver}.tar.gz::https://github.com/RaphaelRochet/arch-update/archive/v${pkgver}.tar.gz")
sha256sums=('56a405371577fd9ec49f2c3177f77f1b3f50dec949729dcdc1c54c0b6410862d')


package() {
  local _uuid='arch-update@RaphaelRochet'
  local _install_dir="${pkgdir}/usr/share/gnome-shell/extensions/${_uuid}"

  install -dm655 $_install_dir
  cd "arch-update-${pkgver}"
  cp -R * $_install_dir
}

# vim: ts=2 sw=2 et:
