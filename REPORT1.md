# TIMP-LAB01
## Задание №1
```
wget https://sourceforge.net/projects/boost/files/boost/1.72.0/boost_1_72_0.tar.gz
```
## Задание №2
```
gzip -d boost_1_72_0.tar.gz
tar -xf boost_1_72_0.tar
rm boost_1_72_0.tar
```
## Задание №3
```
find . -mindepth 1 -maxdepth 1 -type f| wc
      7       7     106
```
Ответ: 7

## Задание №4
```
find . -mindepth 1 -type f| wc
  89939   90249 6047303
```
Ответ: 89939

## Задание №5
```
find -name "*.cpp" | wc -l
```
15904
```
find -name "*.hpp" | wc -l
```
29410
```
find -name "*.h" | wc -l
```
509
```
find . -not \( -name "*.h" -o -name "*.hpp" -o -name "*.cpp" \) | wc -l
```
53354
## Задание №6
```
find -name "any.hpp"
```
```
./boost-libs/boost/fusion/include/any.hpp
./boost-libs/boost/fusion/algorithm/query/detail/any.hpp
./boost-libs/boost/fusion/algorithm/query/any.hpp
./boost-libs/boost/xpressive/detail/utility/any.hpp
...
```
20
## Задание №7
```
grep -lr boost::asio
```
## Задание №8
```
./bootstrap.sh --prefix=boost_output
./b2 install
```
## Задание №9
```
mkdir ~/boost-libs
mv * ~/boost-libs
```
## Задание №10
```
ls -hl
```
```
total 388K
-rw-r--r--   1 parallels parallels  291 Dec 10  2019 INSTALL
-rw-r--r--   1 parallels parallels  12K Dec 10  2019 Jamroot
...
```
## Задание №11
```
find . -type f -exec du -h {} +|sort -rh | head -n 10
```
```
186M	./bin.v2/libs/math/build/gcc-11/release/threading-multi/src/tr1/pch.hpp.gch
186M	./bin.v2/libs/math/build/gcc-11/release/link-static/threading-multi/src/tr1/pch.hpp.gch
15M	./libs/math/doc/math.pdf
8.1M	./libs/graph/test/weighted_matching.dat
4.7M	./boost_output/lib/libboost_math_tr1.a
4.7M	./bin.v2/libs/math/build/gcc-11/release/link-static/threading-multi/visibility-hidden/libboost_math_tr1.a
4.4M	./boost_output/lib/libboost_wave.a
4.4M	./boost_output/lib/libboost_math_tr1l.a
4.4M	./bin.v2/libs/wave/build/gcc-11/release/link-static/threadapi-pthread/threading-multi/visibility-hidden/libboost_wave.a
4.4M	./bin.v2/libs/math/build/gcc-11/release/link-static/threading-multi/visibility-hidden/libboost_math_tr1l.a
```

