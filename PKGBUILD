# Author: half-left <http://half-left.deviantart.com/>
# Maintainer: foalsrock <foalsrock at gmail dot com>

pkgname=gnome-shell-theme-slave
pkgver=20120529
pkgrel=4
pkgdesc="This is a GNOME Shell theme based on SLAVE - a Windows 7 theme."
url="http://half-left.deviantart.com/art/GNOME-Shell-SLAVE-254075556"
license=('GPL')
arch=('any')
depends=('gnome-shell')
optdepends=('gnome-shell-extension-user-theme: User Theme extension for GNOME Shell'
            'gnome-tweak-tool: A tool to customize advanced GNOME 3 options.')
source=("http://www.deviantart.com/download/254075556/gnome_shell___slave_by_half_left-d479pyc.zip")
DLAGENTS=('http::/usr/bin/wget -c -t 3 --waitretry=3 -H -U Mozilla -O %o %u')
md5sums=('2c154fd1a24f71982596637327af4c48')

package() {
    mkdir -p "${pkgdir}/usr/share/themes"
    cp -r "${srcdir}/SLAVE" "${pkgdir}/usr/share/themes/"

    install -Dm644 "${srcdir}/SLAVE/gnome-shell/LICENSE" "${pkgdir}/usr/share/licenses/gnome-shell-theme-slave/LICENSE"
    
}

