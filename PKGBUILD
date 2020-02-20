pkgname=yt2mpd
pkgver=0.1.1
pkgrel=1
pkgdesc="A cli program that fetches audio tracks from youtube-videos for usage in MPD"
arch=('any')
url="https://github.com/pbnoxious/${pkgname}"
license=('GPL3')
depends=('python' 'youtube-dl' 'mpc')
source=(${url}/archive/v${pkgver}.tar.gz)
md5sums=('c6e904411079f47c15a45ce8978edf3b')

package() {
  cd ${pkgname}-${pkgver}
  python setup.py install --root="${pkgdir}/" --optimize=1
}
