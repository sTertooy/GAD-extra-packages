# gda-extra-pkg v1

This action downloads and installs additional packages into a docker image
of GAP. It is intended to be used by the Continuous Integration (CI)
action of a GAP package, in conjunction with a gap-alpine-docker image.

This action is based on the `setup-gap`-action at 
https://github.com/gap-actions/setup-gap


## Usage

The action `GAD-extra-packages` has to be called by the workflow of a GAP
package. By default it does absolutely nothing.

This can be customized via the variable `PACKAGES`:

- `PACKAGES`:
   - Clones and builds any packages specified in the PACKAGES parameter
   - default: `''`
   - example: `'AutoDoc Example GapDoc'`
