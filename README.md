# risetek.ecos.tools

## 下载并准备好源代码：prepare_gnutools
- 下载 binutils
- 下载 gcc 及其 附加的依赖包
- 下载 newlib 并安装到 gcc 源代码目录下
- 将 gcc 所有源代码打包，为其它阶段做准备

## Build tools for eCos
```
mkdir -p build && pushd build \
  && export TARGET=i386-elf && export BINUTILS_VERSION=2.41 && export NEWLIB_VERSION=4.1.0 && export GCC_VERSION=13.2.0 \
  && . ../prepare_gnutools && . ../build_gnutools && mv gnutools ~/.bin \
  && popd

mkdir -p build && pushd build \
  . ../build_ecosconfig && mv ecosconfig ~/.bin \
  && popd
```
