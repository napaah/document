### 项目结构

```
├── build                      # 构建相关
├── node_modules               # 项目依赖
├── public                     # 静态资源
│   │── favicon.ico            # favicon图标
│   └── index.html             # html模板
├── src                        # 源代码
│   ├── api                    # 所有请求
│   ├── assets                 # 主题 字体等静态资源
│   ├── common                 # 全局公共js方法 css样式
│   │   ├── config             # 所有请求
│   │   │   ├── errorLog       # 全局错误处理
│   │   │   ├── permission     # 全局路由处理
│   │   ├── js                 # 全局方法
│   │   │   ├── handleApi      # element全局提示处理
│   │   │   ├── initRules      # element初始化规则
│   │   │   ├── prototype      # v添加原型方法
│   │   │   ├── request        # axios 全局配置
│   │   │   ├── utils          # 工具
│   │   │   ├── validate       # 校验
│   │   ├── style              # css样式
│   │   │   ├── mixin.scss     # 
│   │   │   ├── bass.scss      # 
│   │   │   ├── custom.scss    # 
│   │   │   ├── ...            # 
│   ├── components             # 全局公用组件
│   ├── directive              # 全局指令
│   ├── filters                # 全局 filter
│   ├── icons                  # 项目所有 svg icons
│   ├── layout                 # 全局 layout
│   ├── layout                 # 项目mock 模拟数据
│   ├── router                 # 路由
│   ├── store                  # 全局 store管理
│   ├── utils                  # 全局公用方法
│   ├── views                  # views 所有页面
│   │   ├── mobile             # m端
│   │   ├── mobile             # PC端
│   ├── App.vue                # 入口页面
│   ├── main.js                # 入口文件 加载组件 初始化等
├── .editorconfig              # 编辑器配置
├── .eslintrc.js               # eslint 配置项
├── .babel.config              # babel-loader 配置
└── package.json               # package.json
```

### 安装 启动 打包

~~~

# 进入项目目录
cd 项目目录

# 安装依赖
npm install

# 本地开发 启动项目
npm run serve

# 打包项目
npm run build
~~~

