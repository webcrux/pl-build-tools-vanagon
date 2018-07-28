## Missing path fixed with symlinks

This should be fixed in project configs, but this is a quick temp fix.

After installing **pl-gcc** fix these paths:

```
mkdir -p /opt/pl-build-tools/arm-linux-gnueabihf
ln -s /opt/pl-build-tools/bin /opt/pl-build-tools/arm-linux-gnueabihf/bin
ln -s /opt/pl-build-tools/bin/armv7l-unknown-linux-gnueabihf-g++ /opt/pl-build-tools/bin/arm-linux-gnueabihf-g++
ln -s /opt/pl-build-tools/bin/armv7l-unknown-linux-gnueabihf-gcc /opt/pl-build-tools/bin/arm-linux-gnueabihf-gcc
```

After installing **pl-cmake** fix this path:

```
ln -s /opt/pl-build-tools/arm-linux-gnueabihf/share/cmake-3.2 /opt/pl-build-tools/share/cmake-3.2
```


