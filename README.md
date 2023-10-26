## DISCLAIMER

In this repository there are a few unofficial Dockerfiles to run [SMASH](https://github.com/smash-transport/smash), where *unofficial* means that they are modified versions of the official ones, distributed according to the GPLv3 license, but they are not sponsored, reviewed or approved by the SMASH Team.
Compared to the official ones distributed with SMASH, they are more experimental in nature and they might have some additional programs, more recent versions of third part software/libraries like Root or Rivet or they can be based on different GNU/Linux distributions (e.g. Fedora instead of Ubuntu). However, they also lack the internal reviews and the checks that are done by the SMASH Team, they are provided "as they are", without any guarantee that they work correctly, so, please, *use at your own risk*.

## LIST

- Dockerfile_smash_basic_dev: Unofficial test version of the basic SMASH image, based on Ubuntu 22.04 Jammy Jellyfish. Just the _smash_ executable, Pythia 8.310 and a few tools like git or vim.
- Dockerfile_smash_max_dev: Unofficial test version of the max SMASH image, based on the basic image (i.e. on Ubuntu 22.04). It delivers Pythia 8.310, Root 6.28.06, Rivet 3.1.8, HEPMC3 3.2.6, cppcheck 2.8, cpplint 1.6, cmake 3.22.1, gcc 11.3, Doxygen 1.9.1, Clang 13.0.1, Python 3.10, Numpy 1.21.5, Scipy 1.8.0, Matplotlib 3.5.1, Gnuplot 5.4.2, Pandas 1.3.5 and Julia 1.9.3
- Dockerfile_dev_environment_ubuntu_20_04_w_gcc8_pythia_8310: Based on Ubuntu 20.04 Focal Fossa, tested with stable version 2.2.1 and parallel dev version. Pythia 8.310, Root 6.26.00, Rivet 3.1.5, HEPMC3 3.2.5, cppcheck 2.8, cpplint 1.6, matplotlib 3.5.1, cmake 3.16.3, gcc 9.4.0 and 8.4.0, Doxgen 1.8.17 (wich has known issues)
- Dockerfile_jammy_latex : Based on Ubunut 22.04 Jammy Jellyfish, it does not contain SMASH, but only a fairly complete latex environment
- Dockerfile_fedora_38_only_std_pkg: Based on Fedora 38, it does not provide SMASH, but only a development environment
- Dockerfile_smash_all_in: In comparison with the max container image, it has also vHLLE (https://github.com/yukarpenko/vhlle) and the smash hadron sampler (https://github.com/smash-transport/smash-hadron-sampler)

### DISCONTINUED:
- Dockerfile_smash_2_2_and_2_2-dev_ubuntu_22_04 : Based on Ubuntu 22.04 Jammy Jellyfish, tested with stable version 2.2.1 and parallel dev version. Pythia 8.307, Root 6.26.06, Rivet 3.1.7, HEPMC3 3.2.5, cppcheck 2.8, cpplint 1.6, cmake 3.22.1, gcc 11.3, Doxygen 1.9.1
- Dockerfile_fedora_37: Based on Fedora 37, it does not provide SMASH, but only a development environment (clang-format 13.0.0 and doxygen are not included)
- Dockerfile_fedora_29: Based on Fedora 29, it does not provide SMASH, but only a basic development environment with the minimum supported gcc version 8.1
- Dockerfile_smash_2_2_and_dev_pythia8307_ubuntu_20_04_w_gcc8: Based on Ubuntu 20.04, with gcc 8 and Pythia 8.037
- Dockerfile_dev_environment_ubuntu_20_04_w_gcc8_pythia_8309: Based on Ubuntu 20.04, with gcc 8 and Pythia 8.039
