# iwyu-sample

```
apt-get update
apt install -y git cmake
git clone https://github.com/include-what-you-use/include-what-you-use.git
cd include-what-you-use
git checkout clang_12
cd ..
mkdir build && cd build
cmake -G "Unix Makefiles" -DCMAKE_PREFIX_PATH=/usr/lib/llvm-12 ../include-what-you-use
make -j 16
ls bin/include-what-you-use
./bin/include-what-you-use main.cpp
```