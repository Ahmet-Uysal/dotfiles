# dotfiles
arch linux için kurulması gereken paketler
base base-devel linux linux-firmware iwd networkmanager net-tools gnome-terminal chromium xorg xorg-xinit nitrogen picom i3 dhcp dhcpcd 
# ubuntu i3 vm
Gerekli olan dosyaları bulabilirsin.


## Kurulması Gerekenler

`i3-gaps` için https://blog.elreydetoda.site/minimal-i3-gaps-install-ubuntu/ bu siteden yararlanılabilir
```
sudo apt-get install i3
sudo apt install feh
sudo apt install picom
sudo apt install rofi
sudo apt install polybar




```
terminal üzerinde git branch göstermek için `bashrc` dosyasına asagıdaki kodu ekleyebilirsiniz
```
git_branch() {
  git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/(\1)/'
}
export PS1="\[\e]0;\u@\h: \w\a\]${debian_chroot:+($debian_chroot)}\[\033[01;32m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\w\[\033[00m\] \$(git_branch)\$ "

```
`https://github.com/adi1090x/polybar-themes` polybarı buradan yükleyebiliriz
`https://github.com/Ahmet-Uysal/oh-my-bash` adresinden terminal promtunu özelleştirebiliriz
