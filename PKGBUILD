# Maintainer: Sebastien Luttringer <seblu+arch@seblu.net>
pkgname=ext4magic
pkgver=0.2.3
pkgrel=1
pkgdesc='Linux admin tool, can help to recover deleted or overwritten files on ext3 and ext4 filesystems'
arch=('i686' 'x86_64')
url='http://developer.berlios.de/projects/ext4magic/'
license=('GPL2')
depends=('util-linux' 'e2fsprogs')
source=("http://download.berlios.de/$pkgname/$pkgname-$pkgver.tar.gz") 
md5sums=('b23ecf9dccc8b597fbbe2d149d0c08ac')

build() {
  cd $pkgname-$pkgver
  ./configure --prefix=/usr
  make
}

package() {
  cd $pkgname-$pkgver
  make DESTDIR="$pkgdir" install
}

# vim:set ts=2 sw=2 ft=sh et:
