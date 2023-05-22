# Servermonkeys software philosophy

This is just my personal opinion on how to develop software and build
IT-infrastructure. Mostly in the context of automation. These are guidelines,
not rules, so chill. It is called 'philosophy' for a reason.

## Basic philosophies

Now bank these philosophies into your head, if necessary, with a hammer.

- **Follow Eric Raymond's 17 Unix Rules**  
  [en.wikipedia.org/wiki/Unix_philosophy#Eric_Raymond's_17_Unix_Rules](https://en.wikipedia.org/wiki/Unix_philosophy#Eric_Raymond's_17_Unix_Rules)  
  [medium.com/programming-philosophy/eric-raymond-s-17-unix-rules-399ac802807](https://medium.com/programming-philosophy/eric-raymond-s-17-unix-rules-399ac802807)
- **Only use Phoenix configurations** (Martin Fowler / Kornelis Sietsma)  
  [martinfowler.com/bliki/SnowflakeServer.html](https://martinfowler.com/bliki/SnowflakeServer.html)  
  [martinfowler.com/bliki/PhoenixServer.html](https://martinfowler.com/bliki/PhoenixServer.html)  
  [martinfowler.com/bliki/ImmutableServer.html](https://martinfowler.com/bliki/ImmutableServer.html)  
  This will avoid Configuration drift and specific staff dependency.

- **Write amazing documentation.** Programs without good documentation are
  incomplete programs and should be treated as Alpha versions. You want others
  to use your programs? Write a top to bottom style manual. The reason why to
  write 'amazing' documentation and not 'good enough' documentation is because
  good enough documentation is what we have now, and it is still not enough.
  You don't want to write a manual? Maybe you should work somewhere else. You
  are not allowed to write a manual? Tell your boss that documentation is PART
  of the code, not separated from it, documentation must be a part of every
  project budget. Computer programs without documentation are absolutely
  worthless. Nobody cares that your bicycle fell into the river if you can't
  tell them where.

- **Prefer stable software over shiny software.** As much as you want that new
  feature. Do you really need it right now? New features are usually there to
  increase productivity. But then, what is really hindering productivity? Is it
  that you don't have access to that one new shiny function, that you think you
  need? Or is it rather that things are not working just because they are too
  new? Do you have more problems because you lack functionality or do you have
  problems because someone wrote code that you can't run because you are
  missing a library that can only be installed by following some obscure guide
  on the internet? Are you unproductive because everyone is developing on the
  same old system or is it because everyone in your team uses a different
  version, because they happened to install that latest python pip package on a
  particular day?

- **Don't be clever.** Before you were even born there have been other
  developers and sysadmins that had the same challenges you have today. All
  these people could solve all those problems before you. They left behind a
  legacy of documentation, Open source programs, forum posts and more. If you
  have a problem there is a 99.9 % chance someone else already solved it long
  before you. - Don't be clever and think you are in a special situation. If,
  after month of research and learning, you still don't have a solution, then
  maybe (a big maybe), you can give yourself permission to develop a new
  software or doohickey, that solves your specific problem. And even then. Do
  not reinvent the whole doohickey, try to build your solution on someone
  elses, well tested, doohickey.

* **Code like it's the 1980s.** Modern computing is made of layers on top of
  layers of previous technologies. The technologies of the 70s and 80s has not
  disappeared, nor has it been replaced, but is mainly hidden underneath all
  those other layers and front-ends. Did computers work in the 80s? Yes! Did we
  have Docker, snapd and web applications back then? No! So do we really need
  them then? No. All computer systems are someone's personal garbage opinions
  layered on top of other garbage opinions. It is simply easier to dig trough
  one garbage bin than a dozen. So, develop with the pretense that the target
  system is from the 80s:
    * Software installation should always be possible fully offline. Do not
      make your software require internet access to install or to run.
    * Software should not require bizarre amounts of computing resources to
      function.
    * Software should be backwards compatible as much as possible. Your
      software should be able to run on the previous two stable releases of any
      operating system.
    * Software should be as portable as possible.
    * Stick to \*NIX standards or at least the philosophy behind it.
    * Web applications did not exist in the 80s. So don't write any. If you
      have to, think long and hard about why you want to make your life more
      miserable.
    * Write a CLI application before you write a GUI for it.
    * Don't use weird libraries that are not part of the standard library.

## Automation philosophies

* **Take your time automating.** Initial development of automation tasks takes
  more time than hands-on setups. But is much more worth it in the long run.

* **Abstract away, don't add complexity.** If you have two buttons and after
  your automation you have three buttons, you are doing it wrong. Turning a CLI
  interface into a graphical interface, is not automation. It is just turning
  the interface into another interface. It is the amount of possibilities that
  defines complexity. Automation means to take lots of possibilities and
  turning them into a minimal set of the right possibilities. Human error in
  computing is caused by information overload, not by the information itself.

* **Fewer choices.** In software architecture having fewer choices can be
  better because it simplifies the decision-making process and makes it easier
  to maintain and scale the software. When there are too many choices, it can
  be overwhelming and time-consuming to decide which options to use. It can
  also lead to compatibility issues and make it harder to update or change the
  software in the future. By limiting the number of choices, developers can
  focus on building a solid foundation for the software and avoid unnecessary
  complexity.

* **Write code that is easily comprehensible** by other human beings. Do not
  try to be smart and write complicated code that looks cool or crunch all code
  into one line, just because you can. Impress your colleges by making is easy
  for them to understand your program.

* **Avoid multidimensional data**. Humans have a very hard time understanding
  more than three spacial dimensions. Imagine a JSON file with four or more
  dimensions in comparison to a spreadsheet with only two dimensions. And
  compare that to a simple text file with a list, that is only one dimension.
  Now it is pretty clear that working with the one-dimensional list is easiest.
  So when you develop, try to avoid multidimensional data and instead split
  your data into multiple files. Sometimes multidimensional data is
  unavoidable, but think long and hard before you make others and your own life
  miserable. Do you have terra-bytes of data? Does your program really need a
  database?

* **Write Ansible playbooks** in favor of shell/python-scripts where you can.
  Playbooks are more readable and reliable. The same goes for any other
  automation tools of your choice.

* **Write none-interactive programs.** All automation programs/scripts should
  be strictly none-interactive. Meaning don't make your program suddenly stop
  and wait for user input. Use variables and 'export' functions. It is called
  automation for a reason.

* **Avoid parametrization** where you can. Parameters (arguments) gives room
  for human error. It is almost impossible not to use parameters in programs
  and scripts. But when writing code, think about if your program really needs
  parameters.

* **Avoid Feature creep**. Do not add useless things to your program because
  someone 'might' need them in the future. Only add features that are really
  used.

* **Adhere to the default behavior of standard streams.** Meaning don't write
  scripts that spit out errors where there are none. And the other way around.
  Adhere to return-codes and print errors to std-err.

* **Avoid unnecessary output.** Only use silent confirmation. Meaning if the
  requests action/task worked, do not print out unnecessary confirmations,
  exceptions can be made for tasks that take a long time. This will keep
  log-files readable. Especially if you run lots of tasks. Only print
  information if something went wrong in your script/program. Remember that
  Ansible can properly parse standard streams and return-codes.

* **Use Static Code Analysis.** Also known as linting. Use it for every
  programming language you use. For example when writing Shell-Script in
  PyCharm add #!/bin/sh to the first line and install the Shell Script coding
  assistance plugin. Now fix all issues the coding assistance points out. If
  you use another IDE look at ShellCheck, Shfmt and Explainshell. The same goes
  For Ansible playbooks (ansible-lint) and any other programming language.

* **Humans are lazy and stupid.** Write software in a way that a five-year-old
  can use and understand it. Nobody is interested in how cool or complex your
  software is. They just want to achieve a specific goal and then go on with
  theyr lives. Make others live easier, not more complex.

* **Be meticulous.** Because everything that is mediocre does not last. If you
  have even minor errors in your software, people will very fast loose
  interest.