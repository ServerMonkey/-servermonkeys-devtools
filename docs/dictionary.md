# Servermonkeys IT-dictionary for dummies

_This dictionary is intended to assist people who are not familiar with the
complexities of IT. It is specifically designed as a reference for my
programs._

**Agent**: A computer program that is installed on a computer and used to
monitor and manage that computer. It is like a spy that reports back to you and
does what you tell it to do. Using or not using an agent is a matter of
architecture and preference. Adding agents to a computer system always adds
complexity.

**Ansible**: A computer program that is used to configure computers. It uses
SSH to connect to the computers but is more versatile than just SSH and more
suited for configuration management and automation. See 'SSH'

**Ansible collection**: Is a collection of Ansible roles and other files that
are used to configure a computer system. It is like a LEGO set with multiple
LEGO sets inside. See: 'Ansible role', 'Ansible namespace', 'Galaxy-collection'

**Ansible role**: Is a collection of Ansible playbooks and other files that are
used to configure a computer system. It is like a LEGO set. Usually a role is
made of multiple Ansible tasks.

**Ansible task**: Is a computer program that is used to configure a computer
system. It is like a LEGO figure that is part of a LEGO set.

**Ansible namespace**: In Ansible, a namespace is like a container or a label
that groups together related things like variables, functions, or modules.
Think of it like a folder on your computer. A namespace usually references to
an Ansible role or an Ansible collection.

**API (application programming interface)**: Is a way for two or more computer
programs to communicate with each other.

**APT (Advanced Packaging Tool)**: A package/software manager for Debian and
derived. It is similar to an app-store on a smartphone.

**Asset inventory**: A list of all the computers and other devices that are
connected to a network. It is like an inventory list for the IT department. If
used as a SSOT it can also be a shopping and a to-do list. This makes
IT-management very easy. See. 'SSOT'

**Debian**: An operating system that is based on the Linux kernel. Unlike
Windows and macOS, Debian is free and open source. Can be used by governments
or companies without paying a license fee. It's OpenSource nature and UNIX
based architecture makes it easier to develop for. Debian can also be seen as a
framework with a CLI API. It comes with over 50000 programs, many of those
programs can be combined into automated products. See: 'CLI' and 'API'

**Debian PackageManagement system**: See 'APT'

**Debian preseed**: A file that is used to automate the installation of Debian.
It is similar to an unattended installation of Windows. See: 'Ventoy'

**Debian repo**: A collection of software packages that can be installed on a
Debian system. It is similar to an app-store on a smartphone with the addition
that you can create your own store. See 'APT'

**Derived Debian Distribution**: Is a Debian distribution that is based on
another Debian distribution. For example, Ubuntu is derived from Debian. A
derived distribution usually includes preinstalled or custom packages. It is
like buying a car, then painting it with a new color or adding a new stereo
system.

**CLI (Command-line interface)**: A computer program that is used to interact
with a computer system in a text based fashion. Much like a chat program. CLI
enables you to automate tasks and is more versatile than a graphical interface
but initaly has a harder learning curve.

**Cloud platform**: Is a computer system that allows users to access software
and store data over the internet, instead of their own computer. Usually
maintained by a company that charges a monthly subscription fee.

**CSV (Comma Separated Values)**: A file format that is used to store tabular
data. Much like Excel, but less complex. It can easily be processed by a human
or a computer. Software like Excel or libreOffice can be used to view and edit.

**Galaxy-collection**: Are Ansible namespaces that are available online at
[galaxy.ansible.com](https://galaxy.ansible.com/). They are like a collection
of LEGO bricks that can be used to build something. See: 'Ansible namespace'

**Golden Image**: Is a pre-configured template of a computer system. Mostly it
has all the necessary software and configurations already installed. It is used
to quickly create multiple identical copies of the same computer system. Think
of it like a cookie cutter that can be used to create many cookies that all
look and taste the same. See: 'Hypervisor'

**Guest computer**: A computer in a network that is controlled by another
computer. See: 'Host computer'

**Host computer**: The main computer in a network that controls other
computers. See: 'Guest computer'

**Hypervisor**: Is a software that allows multiple virtual machines (VMs)
to run on a single physical computer. VMs are like simulated computers that can
run their own operating systems and software. This allows multiple users or
applications to share the same physical resources of a computer. The word
Hypervisor is a marketing term, a better word would be 'virtualization
platform'.

**Hyper-converged infrastructure (HCI)**: Is a marketing term simply meaning
that all parts of an IT-infrastructure are virtualized. The word has no real
meaning because it is not useful. It is like saying that a car has wheels. This
is because all modern IT-infrastructures are virtualized in one way or another.

**IaC (Infrastructure as code)**: Is a way of creating and managing
IT-infrastructure using computer programs. It is like sheet music but for
computer infrastructure. Instead of playing by ear, a music sheet (code)
can be easily changed, shared and will produce the same results every time.

**Immutable host/server**: Is a computer that once deployed, is never modified,
merely replaced with a new updated instance. An immutable host is like a car
that you can't change once it's made. This makes sure that you get exactly the
same computer system each time you build it.

**INI (initialization)**: A file format that is used to store configuration
data. It is similar to JSON and YAML, but less complex. It can easily be
processed by a human or a computer.

**Kiosk application**: Is a computer program designed to run on a self-service
kiosk or touch screen device, allowing users to interact with the program and
complete tasks without needing assistance from a person. Kiosk applications are
usually run on Thin clients.

**KVM (Kernel-based Virtual Machine)**: Is a virtualization technology built
into Linux. Lets you turn Linux into a virtualization platform. See: 'QEMU', '
Hypervisor'

**libvirt**: Is a virtualization platform. It is similar to VirtualBox or
VMWare ESXi. Can be used by governments or companies without paying a license
fee. See '
Hypervisor', 'KVM' and 'QEMU'

**Microservice**: Is usually a web application, that is part of a larger
network of web applications that work together. This makes the program easier
to maintain and scale as it grows larger and more complex.

**MIT license**: Is a legal agreement that allows people to use and modify
software for free. It's like sharing your toys with friends and telling them
they can play with them as much as they want and even change them if they want
to. However, the MIT license also says that if you use the software, you have
to give credit to the person who made it and not hold them responsible if
something goes wrong. It's a way for people to share their work with others and
let them build upon it in a fair and open way.

**Monolithic software architecture**: A way of building computer programs where
all the different parts of the program are built and run as a single piece of
software. This means that if one part of the program needs to be updated or
changed, the entire program needs to be updated or changed at once. It can make
the program harder to maintain and scale as it grows larger and more complex.

**Nested virtualization**: When running virtual machines within virtual
machines. It is like the movie with Leonardo DiCaprio, 'Inception' but for
computer infrastructure.

**Provisioning**: Is a confusing term that, depends on whom you ask, can mean
all kinds of things. Sometimes it means installing software, sometimes it means
creating a virtual machine, sometimes it means creating a user account. It is
like saying 'I am going to the store' but not specifying what you are going to
buy. Sometimes it is used interchangeably with 'deployment' sometimes
'provisioning' is a part of the 'deployment' process. It usually means that you
are creating a computer system from scratch and also configuring it. It is
better to use the words 'automated configuration' or 'automated installation'.
See 'deployment'

**Deployment** Is a confusing term that depends on whom you ask can mean all
kinds of things. See: 'Provisioning'

**QEMU (Quick Emulator)**: Is a computer program that emulates a machine's
processor. It can interoperate with KVM. An emulator is like a pretend computer
that can act like a different real computer. See 'KVM'

**Shell**: A computer program that is used to interact with a computer system
in a text based fashion. A user interface much like a chat program.

**SSH (Secure Shell Protocol)**: A computer program that is used to securely
connect to a remote computer. Used to copy files or control programs on the
remote computer. See: 'CLI' and 'Shell'.

**SSOT (Single Source Of Truth)**: Is a way of organizing information so that
there is only one place where it is stored. This makes it easier to keep track
of information and prevents mistakes from happening.

**Unix (\*nix)**: Is an operating system known for being very powerful and
reliable. It is used by many big companies, universities and governments around
the world. It's also the foundation of many other operating systems like macOS
and Linux (including distributions like Debian). Most modern IT-infrastructure
is based on the legacy of Unix and the culture behind it.

**Ventoy**: Is a computer program that is used to easily create a bootable USB
drive. A bootable USB drive is like a special key that can start your computer
and run different programs, like installing a new operating system or fixing
computer problems. With Ventoy, you can add many operating systems to the same
USB drive. This makes it really convenient. See: 'Debian preseed'

**Virtualization platform**: See 'Hypervisor'

**Web application**: Is a computer program that is stored on a remote computer
and accessed by users through a web browser. To use a web application, you
often need an Internet connection. Web applications are more complex than
command-line interface (CLI) applications. Modern companies often prefer web
applications because they can offer services that users can pay for on a
subscription basis.

**Thin client**: Is a computer that relies on a server to do most of its work.
Mostly used as user interfaces for Kiosk application or web applications. A
thin client is usually small and cheap. Almost any modern computer, Laptop,
Phone or Tablet can be turned into a Thin Client. Thin clients are different
from web applications because web applications can be run inside a thin client,
but thin clients are more powerful because they can also use local resources
and programs. When used with kiosk applications, thin clients can prevent user
errors such as accidentally closing a browser tab. See 'Kiosk application', '
Web application'
