# brew-search

CLI tool allowing search Homebrew packages with sorting by popularity.

## Install

```sh
pip install brew-search
```

## Example

```sh
❯ brew-search git -n 10
342760 git - Distributed revision control system
164064 gh - GitHub command-line tool
 68467 git-lfs - Git extension for versioning large files
 30214 argocd - GitOps Continuous Delivery for Kubernetes
 26539 hub - Add GitHub support to git on the command-line
 17324 act - Run your GitHub Actions locally
 16758 git-gui - Tcl/Tk UI for the git revision control system
 15484 lazygit - Simple terminal UI for git commands
 12205 bat - Clone of cat(1) with syntax highlighting and Git integration
 11678 gitleaks - Audit git repos for secrets

❯ brew-search game -n 10 -c
7395 steam - Video game digital distribution service
1140 godot - Game development engine
1007 minecraft - Sandbox construction video game
 920 epic-games - Launcher for *Epic Games* games
 913 heroic - Game launcher
 798 openemu - Retro video game emulation
 672 openra - Real-time strategy game engine for Westwood games
 531 playcover-community - Sideload iOS apps and games
 513 0-ad - Real-time strategy game
 478 moonlight - GameStream client
```

## Usage

```
usage: brew-search [-h] [--number NUMBER] [--cask] [--formula] [--update] term

CLI tool for search packages on Homebrew repository by provided keyword.

positional arguments:
  term                  search term

options:
  -h, --help            show this help message and exit
  --number NUMBER, -n NUMBER
                        number of results
  --cask, -c            search casks only
  --formula, -f         search formulas only
  --update              force update statistics
```
