pkgname=parallel
pkgver=20180822
pkgrel=1
pkgdesc='A shell tool for executing jobs in parallel'
arch=('x86_64')
url='http://www.gnu.org/software/parallel/'
license=('GPL3')
depends=('perl')
source=(https://ftp.gnu.org/gnu/$pkgname/$pkgname-$pkgver.tar.bz2)
md5sums=('268930f1ef472bdd25e9325ee0c46849')

build() {
  cd parallel-$pkgver
  ./configure --prefix=/usr
  make
}

package() {
  cd parallel-$pkgver
  make DESTDIR="$pkgdir/" install
}
