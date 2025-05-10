how to build

git clone -b master-x11-submodule https://github.com/jiaxinchen-max/termux-app &&
cd termux-app &&
git submodule update --init --recursive &&
./gradlew syncDebugLIbJars &&
./gradlew assembleDebug

then, waiting for a while.

But,推荐克隆仓库使用github action 自动构建