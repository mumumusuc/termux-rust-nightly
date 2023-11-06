# termux-rust-nightly
rust-1.71.0-nightly for Termux

## Install
1. download [release file](https://github.com/mumumusuc/termux-rust-nightly/releases/tag/1.71.0-nightly)
2. in Termux run
    ``` bash
    apt install ./rust-nightly_1.71.0-nightly_aarch64.deb
    ```

## Build 

```
CARGO_TARGET_AARCH64_LINUX_ANDROID_RUSTFLAGS="-L$PREFIX/aarch64-linux-android/lib -C link-arg=-lc++_shared -C default-linker-libraries=y" ./x.py build -i --stage 1 --host aarch64-linux-android --target aarch64-linux-android compiler/rustc compiler/std
```
