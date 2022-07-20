# GAD-extra-packages v0.1

This action downloads and installs additional packages into a docker image
of GAP. It is intended to be used by the Continuous Integration (CI)
action of a GAP package, in conjunction with a gap-alpine-docker image.

This action is based on the `setup-gap`-action at 
https://github.com/gap-actions/setup-gap


## Usage

The action `GAD-extra-packages` has to be called by the workflow of a GAP
package. By default it does absolutely nothing.

This can be customized via the PACKAGES-variable:

- `PACKAGES`:
   - Clones and builds any packages specified in the PACKAGES parameter
   - default: `''`
   - example: `'alnuth autpgrp polycyclic'`


## License
The action `GAD-extra-packages` is free software; you can redistribute
and/or modify it under the terms of the GNU General Public License as published
by the Free Software Foundation; either version 2 of the License, or (at your
opinion) any later version. For details, see the file `LICENSE` distributed
with this action or the FSF's own site.
