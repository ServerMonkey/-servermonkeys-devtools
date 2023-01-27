servermonkeys-devtools(1) -- Servermonkeys Development tools
=============================================

## DESCRIPTION

Just a bunch of tools I use to develop Debian and fastpkg packages.  
Also some wine and virtualization related tools.

## LIST OF TOOLS

* `add-repo_servermonkey` : Add APT repo muspekaren.se/repo-debian to
  sources.list.d, same as Ansible task: servermonkey.ww.cfg_apt-servermonkey
* `apt-listlocalpkgs` : List all packages from the local apt repo
* `dir2html <TITLE>` : Create a simple HTML index from current directory
* `remove-lines <TARGET_FILE> <FILE_WITH_LIST_OF_LINES>` : Remove lines from a
  file that are in another file
* `setup_debian_cygwin-setup` : Install and run Cygwin-setup on Debian via Wine
  and fastpkg, includes a Cygwin packages repack archive for Windows XP
* `setup_debian_nlite` : Install and run Nlite on Debian via Wine and fastpkg
* `upgrade-now` : Same as 'apt update and upgrade', also updates fastpkg if
  installed
* `vmclip` : Copy clipboard to VM without clipboard enabled in VM
* `setup_cygwin-sshd` : Configure and enable SSHD, requires Cygwin, run this
  inside Windows XP. Copy from:
  /usr/local/share/servermonkey-tools/setup_cygwin-sshd

## COPYRIGHT

See license file
