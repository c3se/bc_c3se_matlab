# Batch Connect - Matlab proxy

![GitHub Release](https://img.shields.io/github/release/c3se/bc_c3se_matlab.svg)
[![GitHub License](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)

An interactive app designed for OpenOnDemand that launches a matlab proxy server.

## Prerequisites

Requires MATLAB and matlab-proxy to be installed on the **compute nodes** (**NOT** the
OnDemand node):

- [Lmod] or any other `module purge` and `module load <modules>` based
  CLI used to load appropriate environments within the batch job before
  launching.
- [matlab-proxy] 1.0.1+ (actual software)
- [MATLAB] 2020b+ (minimum version required for matlab-proxy)

[Lmod]: https://www.tacc.utexas.edu/research-development/tacc-projects/lmod
[matlab-proxy]: https://github.com/mathworks/matlab-proxy/
[MATLAB]: https://mathworks.com

## Install

Clone the app, customize the form and scripts to your liking and deploy as an app in OpenOndemand.

`main` branch of kept "neutral" of site specific customizations.

## Customizations
You can set which versions of `MATLAB` and `matlab-proxy` is used by setting
the following variables in `~/portal/matlabproxy/matlabproxy.sh`.

You can find configuration examples in `/apps/portal/matlabproxy` on Alvis.

```
$ MATLAB_MODULE_VERSION= # See versions by running module spider MATLAB
$ MATLABPROXY_MODULE_VERSION= # See versions by running module spider matlab-proxy
```

Please note that not all variations of `MATLAB` and `matlab-proxy` has been tested.


## Contributing

1. Fork it ( <https://github.com/c3se/bc_c3se_matlab/fork> )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request against `main` branch.

## License

* Documentation, website content is licensed under
  [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/)
* Code is licensed under MIT (see LICENSE)
* The Jupyter logo is a trademark of Mathworks.
