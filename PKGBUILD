pkgname=yt2mpd
pkgver=0.1
pkgrel=1
pkgdesc="A cli program that fetches audio tracks from youtube-videos for usage in MPD"
arch=('any')
url="https://github.com/pbnoxious/${pkgname}"
license=('GPL3')
depends=('python' 'youtube-dl' 'mpc')
source=(${url}/archive/v${pkgver}.tar.gz)
md5sums=('428a3b75976d57c91e96fe1ed6a4a525')

package() {
  cd ${pkgname}-${pkgver}
  python setup.py install --root="${pkgdir}/" --optimize=1
}
