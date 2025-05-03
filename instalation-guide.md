## YAY installation

```sh
sudo pacman -S --needed git base-devel && git clone https://aur.archlinux.org/yay.git && cd yay && makepkg -si
```

## ZSH setup

```sh
pacman -S zsh

chsh -s /bin/zsh

sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

git clone --depth=1 https://github.com/romkatv/powerlevel10k.git "${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k"

git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting

yay -S nitch

yay -S python-pywal

wal -i Pictures/wallpapers/fog.jpeg

cp arch-configs/zsh/.p10k.zsh /home/franco

cp arch-configs/zsh/.zshrc /home/franco

mkdir -p ~/.local/share/fonts

cp arch-configs/fonts/* ~/.local/share/fonts
```
