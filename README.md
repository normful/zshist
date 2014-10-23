# zshist

When you use zsh as your shell, you can use `setopt EXTENDED_HISTORY` to save timestamps to you commands in `.zsh_history`.
However, the timestamps are in seconds since the epoch, and therefore not quite well readable.
This simple script will parse `.zsh_history` and convert timestamps to readable format. As a bonus, it will colourise the output.

## Dependencies

- Python

## Installation

- Copy `.zshistrc` to `~/.zshistrc`
- Copy `zshist` somewhere in your path
- Copy manpage to an appropriate place

## Usage

- `zshist` without arguments will display `$HOME/.zsh_history`
- If there is an argument, and it is file, it will be displayed.
- If it is a directory, zshist will append `.zsh_history` to the argument and try to display this.

## Changes

- 0.2   - Mon Jan 31 14:47:00 CET 2000: if an argument is a directory, append .zsh_history to it.
- 0.3   - Tue Feb  8 13:34:07 CET 2000: fix stupid bug mangling lines with : in them 
- 0.3.1 - Wed Oct 22 21:50:00 PDT 2014: use time.ctime instead

## Contributors

- Written by Radovan Garabik <garabik@melkor.dnp.fmph.uniba.sk>.
- For new versions, look at http://melkor.dnp.fmph.uniba.sk/~garabik/zshist.html
- Copyright is public domain - do whatever you want with this.
- Special thanks to Milan Matos <matos@fmph.uniba.sk> for suggesting the name of this script.
