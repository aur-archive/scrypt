# Contributor: Oliver Herold <oliver - at - akephalos - dot - de>

pkgname=scrypt
pkgver=1.1.6
pkgrel=2
pkgdesc="scrypt key derivation function and encryption utility"
arch=('i686' 'x86_64')
source=(http://www.tarsnap.com/scrypt/scrypt-1.1.6.tgz)
optdepends=(tarsnap)
url="http://www.tarsnap.com/scrypt/"
license=('BSD')
md5sums=('a35523cd497f7283635ce881db39c2e2')

build() {
  cd $srcdir/$pkgname-$pkgver
  ./configure --prefix=/usr
  make || return 1
  make DESTDIR=$pkgdir install || return 1
}

