父子仓库使用方法（使用git submodule）目标：保证服务器上的代码永远是正确可运行的

注：以下内容参见[SnapdragonLee/Newbee-English: 软件工程 Newbee-English 项目 总仓库 (github.com)](https://github.com/SnapdragonLee/Newbee-MiniProgram/tree/324eacfa197fb2944fb31baa4b3875a060e8e1e3)



**主仓库不要使用`git add .`，尽量单个文件add**



1. 克隆本仓库：使用recursive

   ```
   git clone --recursive path
   ```

2. 拉取代码

   ```
   git pull 
   git submodule update --init --recursive
   ```

3. 标准提交

   1. 平时仅在子仓库文件夹中commit、push
   2. 需要更新服务器代码（确保所有子仓库代码正确性后）再push主仓库

4. 初始化

   ```
   git submodule add miniProgram_http_path miniProgram
   ```

