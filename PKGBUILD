# Author: Oleg Slobodskoi <oleg008@gmail.com>
# Contributor: Jonathan Buchanan
# Contributor: Ashar Voultoiz
# Maintainer: kof <oleg008@gmail.com>
_npmname=qunit
pkgname=nodejs-qunit # All lowercase
pkgver=0.5.16
pkgrel=1
pkgdesc="QUnit testing framework for nodejs"
arch=(any)
url="http: //github.com/kof/node-qunit"
license=(MIT)
depends=('nodejs' )
optdepends=()
source=(http://registry.npmjs.org/$_npmname/-/$_npmname-$pkgver.tgz)
noextract=($_npmname-$pkgver.tgz)
sha1sums=(33947c59f51d93cf27399b8408a8b53c73175d15)
build() {
  cd $srcdir
  local _npmdir="$pkgdir/usr/lib/node_modules/"
  mkdir -p $_npmdir
  cd $_npmdir
  npm install -g --prefix "$pkgdir/usr" $_npmname@$pkgver
}
# vim:set ts=2 sw=2 et: