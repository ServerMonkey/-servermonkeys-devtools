servermonkeys-devtools(1) -- Servermonkeys Development tools
=============================================

## DESCRIPTION

Just a bunch of tools I use to develop Debian and fastpkg packages.

## LIST OF TOOLS

This is a collection of programs and scripts. After installing this as APT
package you can just run each program directly from your shell. Most of them
support a '-h' option for additional help.

* `add-repo_servermonkey` : Add APT repo muspekaren.se/repo-debian to
  sources.list.d, same as Ansible task: servermonkey.ww.cfg_apt-servermonkey
* `applist2exploitdb <IN> <OUT>` : Generate a list of possible exploits from a
  list of applications
* `apt-listlocalpkgs` : List all packages from the local apt repo
* `chmod-default <DIRECTORY>` : Recursively change file and folder permissions
  to default. Directories: 755, Files: 644
* `chmod-secret <DIRECTORY>` : Recursively change file and folder permissions
  to secret. Directories: 700, Files: 600
* `cinac-bootstrap [ -h | dl ]` : Install CinaC to a new unconfigured
  Debian installation, supports offline installation.
* `cinac-bootstrap.ini` : Example configuration file for cinac-bootstrap
* `cinac-unittest <OPTION>` : Create a VM, isntall CinaC and run a test
  blueprint. Useful for developing CinaC blueprints and CinaC itself. Run
  with '-h, --help' for more information.
* `dir2html <TITLE>` : Create a simple HTML index from current directory
* `guake-dc <PATH>` : Opens a new guake tab in the target path. Use it in
  DoubleCommander as terminal.
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
* `windows-isos` : Note on Microsoft Windows ISO files

## COPYRIGHT

See license file
