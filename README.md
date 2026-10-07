About ismip7-interpolation-feedstock
====================================

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/ismip7-interpolation-feedstock/blob/main/LICENSE.txt)

Home: https://github.com/ismip/ismip7-interpolation

Package license: MIT

Summary: Regrid ISMIP7 ice sheet model output onto the standard ISMIP7 grids

Development: https://github.com/ismip/ismip7-interpolation

Documentation: https://ismip.github.io/ismip7-interpolation/

ismip7-interpolation regrids ISMIP7 ice sheet model output, for Greenland
(GrIS) and Antarctica (AIS), onto the standard ISMIP7 grids so that models
on different native grids can be compared.  CDO does the remapping; this
package decides what to remap, how, and where to put it.  It works on an
archive laid out as an ISMIP7 submission, and can process a single file,
an experiment or a whole archive, as well as take an inventory of what an
archive holds.

Current build status
====================


<table><tr>
    <td>All platforms:</td>
    <td>
      <a href="https://github.com/conda-forge/ismip7-interpolation-feedstock/actions/workflows/conda-build.yml">
        <img src="https://github.com/conda-forge/ismip7-interpolation-feedstock/actions/workflows/conda-build.yml/badge.svg?event=push&branch=main">
      </a>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-ismip7--interpolation-green.svg)](https://anaconda.org/conda-forge/ismip7-interpolation) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/ismip7-interpolation.svg)](https://anaconda.org/conda-forge/ismip7-interpolation) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/ismip7-interpolation.svg)](https://anaconda.org/conda-forge/ismip7-interpolation) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/ismip7-interpolation.svg)](https://anaconda.org/conda-forge/ismip7-interpolation) |

Installing ismip7-interpolation
===============================

Installing `ismip7-interpolation` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
conda config --set channel_priority strict
```

How to use
----------

<details>
<summary>With conda</summary>

```
conda install ismip7-interpolation
```

</details>

<details>
<summary>With mamba</summary>

```
mamba install ismip7-interpolation
```

</details>

<details>
<summary>With pixi</summary>

```
# for adding to your local project
pixi add ismip7-interpolation
# for installing globally
pixi global install ismip7-interpolation
```

</details>

Search package versions
-----------------------

It is possible to list all of the versions of `ismip7-interpolation` available on your platform:

<details>
<summary>With conda</summary>

```
conda search ismip7-interpolation --channel conda-forge
```

</details>

<details>
<summary>With mamba</summary>

```
mamba search ismip7-interpolation --channel conda-forge
```

</details>

<details>
<summary>With pixi</summary>

```
pixi search ismip7-interpolation --channel conda-forge
```

</details>

<details>
<summary>With mamba repoquery, which may provide more information</summary>

```
# Search all versions available on your platform:
mamba repoquery search ismip7-interpolation --channel conda-forge

# List packages depending on `ismip7-interpolation`:
mamba repoquery whoneeds ismip7-interpolation --channel conda-forge

# List dependencies of `ismip7-interpolation`:
mamba repoquery depends ismip7-interpolation --channel conda-forge
```

</details>


About conda-forge
=================

[![Powered by
NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[Azure](https://azure.microsoft.com/en-us/services/devops/), [GitHub](https://github.com/),
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/),
[Drone](https://cloud.drone.io/welcome), and [TravisCI](https://travis-ci.com/)
it is possible to build and upload installable packages to the
[conda-forge](https://anaconda.org/conda-forge) [anaconda.org](https://anaconda.org/)
channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance,
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information, please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating ismip7-interpolation-feedstock
=======================================

If you would like to improve the ismip7-interpolation recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/ismip7-interpolation-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks, and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@xylar](https://github.com/xylar/)

