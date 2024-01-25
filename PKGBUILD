# Maintainer: Deividas Gedgaudas <sidicer at gmail dot com>

pkgname=nordlayer
pkgver=3.1.0
pkgrel=0
pkgdesc="Proprietary VPN client for linux"
arch=('i686' 'x86_64')
url="https://nordlayer.com"
license=('custom')
replaces=('nordvpnteams-bin')
conflicts=('nordvpnteams-bin')
depends=('bash')
#backup=('etc/default/nordlayer' 'etc/nordlayer/config.hcl' 'etc/nordlayer/ipsec.secrets')
options=('!strip' '!emptydirs')
install=${pkgname}.install
source_x86_64=("https://downloads.nordlayer.com/linux/latest/debian/pool/main/${pkgname}_${pkgver}_amd64.deb")
sha512sums_x86_64=('8e8f369db2bd6ada11564ab8be06f9faa6efa1a11f324956698c3b8b2da8a489ca685ed68e4e775e05e17e363a661f0af6e5c05d6d3cff76ed83e032ef815cdb')

package(){
	# Extract package data
	#tar xzf data.tar.gz -C "${pkgdir}"
	bsdtar -O -xf *.deb data.tar.gz | bsdtar -C "${pkgdir}" -xJf -
    cp -r "${pkgdir}/usr/sbin/." "${pkgdir}/usr/bin"
    sed -i 's+sbin+bin+g' "${pkgdir}/usr/lib/systemd/system/nordlayer.service"
    rm -r "${pkgdir}/usr/sbin"
}
