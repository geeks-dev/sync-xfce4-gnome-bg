# Maintainer: kaz <kaz@geeks-dev.com>

pkgname=sync-xfce4-gnome-bg
pkgver=1.0
pkgrel=1
pkgdesc="Sync xfce4 desktop background to dconf org.gnome.desktop.background."
arch=('any')
url="https://github.com/geeks-dev/sync-xfce4-gnome-bg"
license=('MIT')
depends=('systemd' 'libxml2' 'glib2' 'xfconf')
install=${pkgname}.install
source=("sync-xfce4-gnome-bg.path"
        "sync-xfce4-gnome-bg.service"
        "sync-xfce4-gnome-bg")
md5sums=('f3284565731e3162697e664620f42011'
         '689420db41e1536a63a62de0925efcd3'
         '41dc876bd91c974a14bd0ee863c7304f')

package() {
    install -Dm755 'sync-xfce4-gnome-bg' "$pkgdir/usr/bin/sync-xfce4-gnome-bg"
    install -Dm644 'sync-xfce4-gnome-bg.path' "$pkgdir/usr/lib/systemd/user/sync-xfce4-gnome-bg.path"
    install -Dm644 'sync-xfce4-gnome-bg.service' "$pkgdir/usr/lib/systemd/user/sync-xfce4-gnome-bg.service"
}
