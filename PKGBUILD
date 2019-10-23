pkgname=yt2mpd
pkgver=0.1
pkgrel=1
pkgdesc="A cli program that fetches audio tracks from youtube-videos for usage in MPD"
arch=('any')
url="https://github.com/pbnoxious/${pkgname}"
license=('GPL3')
depends=('python' 'youtube-dl')
source=(${url}/archive/${pkgver}.tar.gz)

package() {
  cd ${pkgname}
  python setup.py install --root="${pkgdir}/" --optimize=1
}
