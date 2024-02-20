# risetek.ecos.tools
Build tools for eCos
```
mkdir build && pushd build && . ../build_ecosconfig && export BINUTILS_VERSION=2.41 && export NEWLIB_VERSION=4.1.0 && . ../prepare_gnutools && . ../build_gnutools && mv ecosconfig ~/.bin && mv gnutools ~/.bin && popd
```
