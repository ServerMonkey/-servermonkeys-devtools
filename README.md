servermonkeys-devtools(1) -- Servermonkeys Development tools
=============================================

## DESCRIPTION

Just a bunch of tools I use to develop Debian and fastpkg packages.  
Also some wine and virtualization related tools.

## LIST OF TOOLS

* `add-repo_servermonkey` : Add APT repo muspekaren.se/repo-debian to
  sources.list.d, same as Ansible task: servermonkey.ww.cfg_apt-servermonkey
* `applist2exploitdb <IN> <OUT>` : Generate a list of possible exploits from a
  list of applications
* `apt-listlocalpkgs` : List all packages from the local apt repo
* `dir2html <TITLE>` : Create a simple HTML index from current directory
* `monkeyrepo-sftp-uploader` : Upload a fastpkg repo to a sftp-only server,
  uses the 'pass' tool
* `oldversion2fastpkg <SRC> <DES> <URL_PREFIX>` : Convert oldversion.com .tar
  archive to a fastpkg repo
* `remove-lines <TARGET_FILE> <FILE_WITH_LIST_OF_LINES>` : Remove lines from a
  file that are in another file
* `setup-cinac-unattended` : CinaC unattended installer example
* `upgrade-now` : Same as 'apt update and upgrade', also updates fastpkg if
  installed
* `vmclip` : Copy clipboard to VM without clipboard enabled in VM
* `websitedownloader2fastpkg <DIR_IN> <FILE_OUT> <WWW_ROOT>` : Convert a
  directory of zip files to a fastpkg packages repo file

## LIST OF DOCUMENTS

* `dictionary` : Servermonkeys IT-dictionary for dummies
* `software-philosophy` : Servermonkeys software philosophy
* `ventoy` : Ventoy with Debian Preseed and fastpkg

## COPYRIGHT

See license file
