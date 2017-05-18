### 最近在全局安装npm包时，报一个很奇怪的错误。
### 例如：
```
npm install -g omi-cli
```
安装成功，但是输入omi --help 后，报错：env: node\r: No such file or directory

刚开始已经是npm 安装的问题，尝试cnpm，yarn 后还是报错。


百度很久，原来是因为\r这个字符的缘故。在linux终端下，输出\r会什么都不显示，只是把光标移到行首。

解决方案如下：
```
$brew install dos2unix
$cd /usr/local/lib/node_modules/omi/bin
$sudo dos2unix omi
```

上述命令成功执行之后，omi --help，一切ok了
