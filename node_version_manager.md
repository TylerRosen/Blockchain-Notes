> nodist
# Lists installed versions highlighting the active ones.
> nodist global 4.x
# Sets the global node version requirement
> nodist local 4.x
# Sets the node version requirement per directory (including all subdirectories).
> nodist env 4.x
# Sets the node version requirement per terminal.
> nodist npm global 3.x
# Set global npm version requirement.

> nodist npm global match
# Tell nodist to always choose the npm version that matches the current node version.
# (the current node version may be determined by env, local or global requirements)
> nodist npm local 2.x
# Set the npm version requirement for the current directory.
> nodist npm env 2.x
# Set the npm version requirement for the current terminal environment.
call nodist env 4.x
# In a batch script use `call`.
> nodist dist
# Lists all available node versions.
> nodist + 4.x
# Just checks, if the version is installed and installs it if not.

> nodist + all
# will install *everything*.
> nodist - 4.1.1
# Removes a version.
> nodist --help
# Displays a complete list of commands with examples.