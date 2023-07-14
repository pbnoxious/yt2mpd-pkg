pkgname=yt2mpd
pkgver=v0.1.3
pkgrel=1
pkgdesc="A cli program that fetches audio tracks from youtube-videos for usage in MPD"
arch=('any')
url="github.com/pbnoxious/${pkgname}.git"
license=('GPL3')
depends=('python' 'youtube-dl' 'mpc')
_tag=f8b57d15c7066cf59aaca0014b140b6dbd68cade
source=(git+https://${url}#tag=${_tag}?signed)
md5sums=('SKIP')

pkgver() {
    cd "$pkgname"
    git describe
}

package() {
  cd ${pkgname}
  python setup.py install --root="${pkgdir}/" --optimize=1
}
