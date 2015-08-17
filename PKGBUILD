# Maintainer : Martin Wimpress <code@flexion.org>

pkgname=pocket
pkgver=1.5
pkgrel=3
pkgdesc="Desktop companion to the Android app of the same name. Securely stores all your sensitive data."
arch=('i686' 'x86_64')
url="http://timothyjc.blogspot.co.uk/2010/12/wallet-for-android.html"
license=('custom')
depends=('java-runtime')
options=('!strip')
source=("http://dl.dropbox.com/u/2309173/${pkgname}_${pkgver}.jar"
        "${pkgname}.sh"
        "${pkgname}.desktop"
        "${pkgname}.png")
md5sums=('413cb9ea15bb58cefe51f384487a9e6d'
         '4a4c6e53d4bd1265677551b361210f16'
         '15242cb095e0c84b46fa83d8c371d0d6'
         'e3c74060be4883b6955eb3daf37d3c46')

package() {
    cd ${srcdir}
    install -D -m 644 ${pkgname}_${pkgver}.jar "${pkgdir}/usr/share/java/${pkgname}/${pkgname}.jar"
    install -D -m 755 ${pkgname}.sh "${pkgdir}/usr/bin/${pkgname}.sh"
    install -D -m 644 ${pkgname}.desktop "${pkgdir}/usr/share/applications/${pkgname}.desktop"
    install -D -m 644 ${pkgname}.png "${pkgdir}/usr/share/pixmaps/${pkgname}.png"
}
