```
docker build buildenv -t my_kernel_buildenv .
docker run --rm -it -v ${PWD}:/root/env my_kernel_buildenv
# in docker
make build-x86_64

# in machine
qemu-system-x86_64 -cdrom dist/x86_64/kernel.iso

```
