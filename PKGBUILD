# Maintainer: Maurizio D'Addona <mauritiusdadd@libero.it>

pkgname=lnxstack
pkgver=1.0.0
pkgrel=1
pkgdesc="A program usefull to align and stack astronomical images"
arch=(any)
url="http://sourceforge.net/p/lxnstack/wiki/Home/"
license=('GPL3')
groups=()
depends=('python2>=2.7.0' 'python2-numpy>=1.7.0' 'qt>=4.8.0' 'opencv>=2.4.0' 'python2-imaging>=1.1.6' 'python2-pyqt>=4.9.6' 'v4l-utils>=0.8.9')
options=()
source=(http://ignum.dl.sourceforge.net/project/lxnstack/tarballs/$pkgname-$pkgver.tar.gz)
md5sums=('1a409229475c4799ea27ab212003ba99') #generate with 'makepkg -g'

package() {
  cd "$srcdir/$pkgname-$pkgver"
  python2 ./install.py --prefix="$pkgdir" --ignore-prefix
}

