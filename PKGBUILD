#
# Contribuidor: Wkve Telecom
#

pkgname=adns
pkgver=1.6.0
pkgrel=1
pkgdesc="Uma biblioteca de resolução de substituição assíncrona"
arch=('x86_64')
url="https://localhost/adns/"
license=('cIO')
depends=('glibc')
source=(adns.tar.gz)
sha512sums=('SKIP')

build()
{
    cd "$srcdir"/$pkgname
    ./configure --prefix=/usr
    make
}

package()
{
    cd "$srcdir"/$pkgname
    mkdir -p "$pkgdir"/usr/{lib,include,bin}
    make prefix="$pkgdir"/usr install
}
