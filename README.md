# rust-embedded-workshop
Learing embedded boards with Rust and Discovery &amp; Blue Pill boards

## Materials

1. [Rust website](https://www.rust-lang.org/)
2. [The Book - The Rust Programming Language](https://doc.rust-lang.org/1.30.0/book/2018-edition/foreword.html)
3. [Discovery](https://docs.rust-embedded.org/discovery/)
4. [The Embedded Book](https://docs.rust-embedded.org/book/intro/index.html)

## Projects

1. [Discovery Project](https://github.com/rust-embedded/discovery)
2. [Blue Pill Project](https://github.com/japaric/stm32f103xx-hal)

## Documents

1. [STM32F3DISCOVERY User Manual](http://www.st.com/resource/en/user_manual/dm00063382.pdf)
2. [STM32F303VC Datasheet](http://www.st.com/resource/en/datasheet/stm32f303vc.pdf)
3. [STM32F303VC Reference Manual](http://www.st.com/resource/en/reference_manual/dm00043574.pdf)
4. [LSM303DLHC - compass datasheet](http://www.st.com/resource/en/datasheet/lsm303dlhc.pdf)
5. [L3GD20H - gyroscope datasheet](https://www.st.com/resource/en/datasheet/l3gd20h.pdf)

1. [STM32F103C8T6 Datasheet](https://www.st.com/resource/en/datasheet/CD00161566.pdf)
2. [STM32F103C8T6 Reference manual](https://www.st.com/resource/en/reference_manual/cd00171190.pdf)

## Seting up environment
1. Install rustup tool
```sh
curl https://sh.rustup.rs -sSf | sh
```
2. Install itm tool
```sh
cargo install itm --vers 0.3.1
```
3. Install cargo-binutils
```sh
rustup component add llvm-tools-preview
cargo install cargo-binutils --vers 0.1.4
```

----
[Linux](https://docs.rust-embedded.org/discovery/03-setup/linux.html)

**Macos**
vvvv

4. Install debug tools
```
brew install minicom openocd
```
5. Download GNU ARM Embedded Toolchain

[Link for macos](https://developer.arm.com/-/media/Files/downloads/gnu-rm/8-2018q4/gcc-arm-none-eabi-8-2018-q4-major-mac.tar.bz2?revision=1041bf49-06d4-4174-866f-0e5259fa9d8d?product=GNU%20Arm%20Embedded%20Toolchain,64-bit,,Mac%20OS%20X,8-2018-q4-major)

6. Add GNU ARM Embedded Toolchain to PATH
```sh
export PATH="$HOME/mike/dev/gcc-arm-none-eabi-8-2018-q4-major/bin:$PATH"
```

7. Add Rust toolchain for Discovery Board
```sh
rustup target add thumbv7em-none-eabihf
```

8. Add Rust toolchain for Blue Pill
```sh
rustup target add thumbv7m-none-eabi
```
