<h1 align="center"><img title="The Long Night Is Coming" src="https://raw.githubusercontent.com/ZirtysPerzys/DRGL-wallet/master/src/images/splash.png" width="1800" height="500" ><img/></h1>

Binaries are made available by community members. If you are able to compile on your operating system, please consider helping others by adding to the release. Also if your OS is available, please consider donating to the community member who made it possible. 


### Building on *nix

**1. Clone wallet sources**

```
git clone https://github.com/zirtysperzys/DRGL-wallet.git
```

**2. Set symbolic link to coin sources at the same level as `src`. For example:**

```
ln -s ../Dragonglass cryptonote
```

Alternative way is to create git submodule:

```
git submodule add https://github.com/zirtysperzys/Dragonglass.git cryptonote
```

**3. Build**

```
mkdir build && cd build && cmake .. && make
```
### Build instructions for Mac
Same as *nix build instructions.  But cmake will likely need your qt path, so 
cmake -DCMAKE_PREFIX_PATH:STRING=<Qt path/Qt version/clang_64/> 
Additional build step to bundle static libraries with app package: <Qt path/Qt version/clang_64/bin/macdeployqt> <path to your project/build/DRAGONGLASS.app
