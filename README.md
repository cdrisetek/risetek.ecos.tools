# risetek.ecos.tools
Build tools for eCos
```
mkdir -p build && pushd build \
  && export TARGET=i386-elf && export BINUTILS_VERSION=2.41 && export NEWLIB_VERSION=4.1.0 \
  && . ../build_ecosconfig \
  && . ../prepare_gnutools && . ../build_gnutools \
  && mv ecosconfig ~/.bin && mv gnutools ~/.bin \
  && popd
```
