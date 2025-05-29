# 安装软件

npm install -g pnpm
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
source $HOME/.cargo/env
cargo --version

# 安装依赖

pnpm install

# 桌面端开发

pnpm tauri dev

# 桌面端打包

pnpm tauri build

# Android 初始化与打包

pnpm tauri android init
pnpm tauri android build

# iOS 初始化与打包

pnpm tauri ios init
pnpm tauri ios build

# 如果有报错，可以尝试手动编译

cd src-tauri
cargo build
