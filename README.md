# dotfiles

## tmux

### Dependências

- [tmux](https://github.com/tmux/tmux) >= 3.6
- [catppuccin/tmux](https://github.com/catppuccin/tmux) v2.3.0
- [tmux-plugins/tmux-cpu](https://github.com/tmux-plugins/tmux-cpu)
- [tmux-plugins/tmux-battery](https://github.com/tmux-plugins/tmux-battery)
- Fonte com suporte a [Nerd Fonts](https://www.nerdfonts.com/)

### Instalação

1. Instalar o tmux:
   ```bash
   brew install tmux        # macOS
   sudo apt install tmux    # Ubuntu/Debian
   ```

2. Clonar os plugins:
   ```bash
   mkdir -p ~/.config/tmux/plugins

   git clone --depth 1 --branch v2.3.0 https://github.com/catppuccin/tmux.git \
     ~/.config/tmux/plugins/catppuccin/tmux

   git clone --depth 1 https://github.com/tmux-plugins/tmux-cpu.git \
     ~/.config/tmux/plugins/tmux-cpu

   git clone --depth 1 https://github.com/tmux-plugins/tmux-battery.git \
     ~/.config/tmux/plugins/tmux-battery
   ```

3. Copiar a configuração:
   ```bash
   cp tmux/tmux.conf ~/.config/tmux/tmux.conf
   ```

4. Abrir o tmux:
   ```bash
   tmux
   ```

### Recarregar configuração

```
Ctrl+b r
```
