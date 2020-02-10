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
│   ├── mock                   # 项目mock 模拟数据
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

### 编码规范

+ **样式文件命名说明** 

  注：【css处理程序统一使用scss，并放在“src/common/style”目录下】

（1）重置样式：reset.scss

（2）基础布局样式：base.scss

（3）公共样式：custom.scss

（4）混合类型(函数样式)：mixin.scss

-  ##### 命名规范

   (1）文件命名：以英文命名，后缀为.js，例：（共用）common.js，其他命名可根据模块需求命名；

 （2）变量命名：驼峰式命名，原生JavaScript变量要求是纯英文字母， 首字母须小写，变量集中声明， 避免全局      变量
 （3）类命名：首字母大写， 驼峰式命名。eg：StudentInfo、UserInfo、ProductInfo；

（ 4）函数命名：首字母小写驼峰式命名。eg：getUserInfo；

 （5）命名语义化，尽可能利用英文单词或其缩写。

 （6）常量：必须采用全大写的命名，且单词以_分割，常量通常用于ajax请求url，和一些不会改变的数据；

   命名规范：使用大写字母和下划线来组合命名，下划线用以分割单词。

例：const MAX_LENGTH = 20;const URL = 'http://www.star.com'

（7）变量：必须采用小驼峰式命名法，例：let maxCount = 10;



命名方法：小驼峰式命名法；

命名规范：前缀应当为动词；

命名建议：可使用常见动词约定。

| **动词** | **含义**                     | **返回值**                                            |
| -------- | ---------------------------- | ----------------------------------------------------- |
| can      | 判断是否可执行某个动作(权限) | 函数返回一个布尔值。true：可执行；false：不可执行     |
| has      | 判断是否含有某个值           | 函数返回一个布尔值。true：含有此值；false：不含有此值 |
| is       | 判断是否为某个值             | 函数返回一个布尔值。true：为某个值；false：不为某个值 |
| get      | 获取某个值                   | 函数返回一个非布尔值                                  |
| set      | 设置某个值                   | 无返回值、返回是否设置成功或者返回链式对象            |
| load     | 加载某些数据                 | 无返回值或者返回是否加载完成的结果                    |

 