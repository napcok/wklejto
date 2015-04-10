# Maintainer: Napcok <napcok [at] gmail [dot] com>
pkgname=wklejto
pkgver=0.1.0
pkgrel=1
pkgdesc="Skrypt do wklejania tekstów na wklejto.org"
arch=('any')
url="https://github.com/napcok/wklejto"
license=('GPL')
groups=()
depends=()
makedepends=('git')
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
source=("$pkgname::git+http://github.com/napcok/wklejto#branch=master")
noextract=()
md5sums=('SKIP') #generate with 'makepkg -g'

_gitroot=https://github.com/napcok/wklejto
_gitname=master


build() {
  cd "$srcdir"
  msg "Connecting to GIT server...."
  cd "$srcdir/$pkgname"

  msg "Starting build..."
  echo "$srcdir/$pkgname"
}

package() {
  cd "$srcdir/$pkgname"
  echo "srcdir: ${srcdir}"
  echo "pkgdir: ${pkgdir}"
  
  install -Dm755 ./usr/bin/${pkgname} ${pkgdir}/usr/bin/${pkgname}
  install -Dm744 ./usr/share/${pkgname}/lang-mappings.sed ${pkgdir}/usr/share/${pkgname}/lang-mappings.sed


  
}

#makepkg -fsC --needed 
#sudo pacman -U wklejto-0.1.0-1-any.pkg.tar.xz
