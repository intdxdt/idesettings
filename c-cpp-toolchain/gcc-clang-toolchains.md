### gcc-clang-toolchains

#### (for libstdc++).

```sh 
sudo add-apt-repository ppa:ubuntu-toolchain-r/test
sudo apt-get update
```


```sh
wget -O - https://apt.llvm.org/llvm-snapshot.gpg.key | sudo apt-key add -
sudo apt-add-repository "deb http://apt.llvm.org/xenial/ llvm-toolchain-xenial-6.0 main"
sudo apt-get update
sudo apt-get install -y clang-6.0
```

#### update alternatives

```sh

update-alternatives --install /usr/bin/clang++ clang++ /usr/bin/clang++-3.8 100
update-alternatives --install /usr/bin/clang++ clang++ /usr/bin/clang++-6.0 1000

update-alternatives --install /usr/bin/clang clang /usr/bin/clang-3.8 100
update-alternatives --install /usr/bin/clang clang /usr/bin/clang-6.0 1000


update-alternatives --install /usr/bin/clang-tidy clang-tidy /usr/bin/clang-tidy-3.8 100
update-alternatives --install /usr/bin/clang-tidy clang-tidy /usr/bin/clang-tidy-6.0 1000


update-alternatives --install /usr/bin/clang-query clang-query /usr/bin/clang-query-3.8 100
update-alternatives --install /usr/bin/clang-query clang-query /usr/bin/clang-query-6.0 1000


update-alternatives --install /usr/bin/clang-format-diff clang-format-diff /usr/bin/clang-format-diff-3.8 100
update-alternatives --install /usr/bin/clang-format-diff clang-format-diff /usr/bin/clang-format-diff-6.0 1000


update-alternatives --install /usr/bin/clang-format clang-format /usr/bin/clang-format-3.8 100
update-alternatives --install /usr/bin/clang-format clang-format /usr/bin/clang-format-6.0 1000


update-alternatives --install /usr/bin/clang-check clang-check /usr/bin/clang-check-3.8 100
update-alternatives --install /usr/bin/clang-check clang-check /usr/bin/clang-check-6.0 1000


update-alternatives --install /usr/bin/clang-apply-replacements clang-apply-replacements /usr/bin/clang-apply-replacements-3.8 100
update-alternatives --install /usr/bin/clang-apply-replacements clang-apply-replacements /usr/bin/clang-apply-replacements-6.0 1000

update-alternatives --config clang
update-alternatives --config clang++

```