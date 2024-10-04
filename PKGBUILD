# Maintainer: haxibami <contact at haxibami dot net>

pkgname=ttf-rubik-vf
pkgver=2.3.0
pkgrel=1
_commit=e337a5f69a9bea30e58d05bd40184d79cc099628
pkgdesc="A sans serif font family with slightly rounded corners: variable font version"
arch=("any")
url="https://github.com/googlefonts/rubik"
license=("OFL")
source=(
      "${url}/blob/${_commit}/fonts/variable/Rubik%5Bwght%5D.ttf"
      "${url}/blob/${_commit}/fonts/variable/Rubik-Italic%5Bwght%5D.ttf"
      "${url}/blob/${_commit}/OFL.txt"
      "${url}/blob/${_commit}/AUTHORS.txt"
      "${url}/blob/${_commit}/CONTRIBUTORS.txt"
)

sha256sums=('93d17f662fdb0291ce55a9e9af408f2ad0d2bbf2efe6664bef97d8933d8b07f3'
            '0c1864e40441a6c98755298313124add944ddcb8a99530f7af35384b77dd6491'
            '3e9cc4fa69cfae610fe214ecc88b8da954f945111d46fd16d4a003821f6ed9ac'
            'd78c5842da21134acc69e64d5098fb8c51192d974ea3ddd2fb279ea695e195ef'
            'b896820ec04e66252c409730b4091ac2986c645f0027fe6d76dceba46adb8f0f')

package() {
      install -d ${pkgdir}/usr/share/fonts/TTF
      install -m644 ${srcdir}/*.ttf ${pkgdir}/usr/share/fonts/TTF/
      cd ${srcdir}
      install -D -m644 -t ${pkgdir}/usr/share/licenses/${pkgname}/ OFL.txt AUTHORS.txt CONTRIBUTORS.txt
}