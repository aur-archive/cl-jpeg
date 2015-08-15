# Maintainer:  Taras Shpot <mrshpot at gmail dot com>

pkgname=cl-jpeg
_clname=jpeg
pkgver=1.023
pkgrel=3
pkgdesc="a Common Lisp library for creating PNG files"
arch=('i686' 'x86_64')
url="http://www.cliki.net/cl-jpeg"
license=('BSD')

depends=('common-lisp' 'cl-asdf')

install=cl-jpeg.install
source=('http://www.common-lisp.net/project/mcclim/cl-jpeg.tar.gz')
md5sums=('276ef9ce3c03a1fa5815b27ee037b739')

build() {
  ### TODO: finish this. I've only filled in the versions ans URLs
    install -d ${pkgdir}/usr/share/common-lisp/source/${_clname}
    install -d ${pkgdir}/usr/share/common-lisp/systems

    cd ${srcdir}/${pkgname}

	install -m 644 -t ${pkgdir}/usr/share/common-lisp/source/${_clname} \
	  ${srcdir}/${pkgname}/*.lisp
	install -m 644 -t ${pkgdir}/usr/share/common-lisp/source/${_clname} \
	  ${srcdir}/${pkgname}/${pkgname}.asd


	
    cd ${pkgdir}/usr/share/common-lisp/systems
    ln -s ../source/${pkgname}/${_clname}.asd .
}

# vim:set ts=2 sw=4 et nospell:
