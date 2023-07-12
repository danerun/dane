# DANE: Dotfiles Are Not Enough

## Dotfiles

Dotfiles always end up failing and breaking because dotifles are designed to configure a specific version of a piece of software.

Nix has "home manager" that is getting close to what DANE is dreaming of delivering.

## Solution

We must handle:

- Program Versions
- Dotfiles Content
  - Adjust Programatically per Operating System
  - Adjust per environment - For example X11 vs Wayland, KDE Plasma vs i3, etc
  - Adjust Programatically per Region (some settings only apply in `VPN Required` countries)
 
## The Goal: One terminal package

- Can run anywhere... On WSL, On mac, On Linux, Inside Docker
- Does not require a full `Nix` install
- Can be bootstrapped in under 1 minute in a normal situation
- Should take less than 1GB of space in the `inside Docker` version of the install
- Should include: Tmux, Zsh, Internet Shared Shell History, Neovim, Clipboard access, SSH access
