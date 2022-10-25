# mac-pre-dev
Mac Pre Development

Dibawah ini adalah instruksi untuk mempersiapkan lingkungan pengembangan MacOS, selain yang berbasis XCode (Swift, Objective-C).
Menggunakan instruksi ini berarti **Anda siap untuk keluar dari zona nyaman**. Artinya Anda harus teliti dan berhati-hati sebelum menginstall aplikasi-aplikasi yang disediakan diluar App Store.

# XCode

Setelah menginstall XCode dari App Store jalankan command berikut di terminal:

```sh
sudo xcode-select -s /Applications/Xcode.app/Contents/Developer
```
```sh
sudo xcodebuild -license
```

# Brew

Install brew untuk menginstall library-library yang tidak disediakan di App Store.
Informasi lebih lanjut bisa dilihat di <a href="https://brew.sh" target="_blank">Situs Brew</a>

Install brew lewat command line:

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Sebelum menginstall aplikasi dan library berbasis `brew`, Anda dapat mencari dan melihat instruksi instalasinya di <a href="https://brew.sh" target="_blank">Situs Brew</a>

# MacPorts

MacPorts adalah kumpulan library dan aplikasi berbasis GNU. Install MacPorts hanya jika Anda ingin menginstall aplikasi berbasis GNU/Linux atau terbentur masalah instalasi yang disediakan `brew`, misalnya ada library yang kurang. Install MacPorts sesuai versi MacOS Anda dari <a href="https://www.macports.org/install.php" target="_blank">Situs MacPorts</a>.

Library dan aplikasi yang disediakan MacPorts dapat Anda lihat di <a href="https://ports.macports.org" target="_blank">Situs MacPort</a>

Setelah menginstall MacPort, Anda harus membuka Terminal baru lalu jalan perintah:

```sh
sudo port -v selfupdate
```

# VIM

Jalankan command berikut untuk konfigurasi dasar vim

```sh
touch ~/.vimrc
echo "set expandtab" >> ~/.vimrc
echo "set backspace=indent,eol,start" >> ~/.vimrc
echo "set smartindent" >> ~/.vimrc
echo "syntax on" >> ~/.vimrc
echo "set nowrap" >> ~/.vimrc
echo "set tabstop=4" >> ~/.vimrc
echo "set shiftwidth=4" >> ~/.vimrc
echo "set nocindent" >> ~/.vimrc
echo "set number" >> ~/.vimrc
```
