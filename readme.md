纯前端的工程化构建打包工具,使用gulp,适合 传统多页面.

安装环境
 ```npm install```

生产实时更新
 ```npm run dev```

打包
 ```npm run build```

打包并在目标目录运行
 ```npm run start```

将图片合并成精灵图
 ```npm run sprites```

将图片转成webp
 ```npm run webp```

### 资源引用:
1. 模板的继承关系 和 css 中的资源引用 使用相对路径
2. js 文件 和 css 文件 使用绝对路径引用, 根路径为 src

### 需要全局安装的包
1. 如果需要单元测试 请运行  ```npm i -g karma```

2. 如果需要接口测试 请运行  ```npm i -g mocha```

3. 如果需要UI测试   请运行  

   ```
   npm i -g backstopjs --ignore-scripts
   npm i --save-dev puppeteer --ignore-scripts
   npm i --save-dev chromium
   npm i --save-dev backstopjs
   ```

   初始化 ```backstop init```
   测试   ```backstop start```

4. 如果需要功能测试 请运行  ```npm i -D selenium-webdriver``` <已集成>

具体支持请看 todo

### 注意
在安装包时,有可能会出现 
```
Error: UNABLE_TO_VERIFY_LEAF_SIGNATURE
request to https://registry.npmjs.org/yarn failed, reason: unable to verify the first certificate
```
这个错误, 请设置 ```npm config set strict-ssl false ``` 将包安装完成后 修改为 true
