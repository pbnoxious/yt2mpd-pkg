pkgname=yt2mpd
pkgver=0.1
pkgrel=1
pkgdesc="A cli program that fetches audio tracks from youtube-videos for usage in MPD"
arch=('any')
url="https://github.com/pbnoxious/${pkgname}"
license=('GPL3')
depends=('python' 'youtube-dl' 'mpc')
source=(${url}/archive/v${pkgver}.tar.gz)
md5sums=('2ca66054bf1fc7e5f04be6f052ddb19c')

package() {
  cd ${pkgname}-${pkgver}
  python setup.py install --root="${pkgdir}/" --optimize=1
}
