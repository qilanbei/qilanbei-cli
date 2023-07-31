## 创建 cli 步骤如下：
- 1、创建一个项目 `npm init -y`
- 2、创建一个 bin 目录，bin 目录里面创建一个 qilanbei （可随意命名，就是要以这个 name 为命令）文件
- 3、qilanbei 文件： `#! /usr/bin/env node` 标识当前文件需要使用 `node` 去执行
- 4、在 `package.json` 中配置 bin 参数：
```javascript
"bin": "./bin/qilanbei"
```
- 5、想要在终端执行 qilanbei 命令，我们必须要做成全局的，所以我们需要用到测试本地的包的工具指令 `npm link` 命令，故在本地终端执行：
```
npm link --force
```
- 6、这样我们在使用我们定义的命令 qilanbei，就可以看到终端的输出了