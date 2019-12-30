# zwtcss预设快速css

## 安装项目依赖包
```
npm install zwtcss
```

### 引入（建议main.js里引入）
```
import "zwtcss"
```

### css说明，一共分为以下几个模块，具体使用在对应css文件里，打开node_modules->zwtcss->dist->zwtcss.css查看
```
/**********盒子布局模型*/
box()
```
import "zwtcss/zc_box"
```

/**********内外边距快速预设*/
pm()
```
import "zwtcss/zc_pm"
```

/**********背景颜色和字体颜色快速预设*/
co()
```
import "zwtcss/zc_color"
```

/**********文本相关样式快速预设*/
fz()
```
import "zwtcss/zc_fz"
```

/**********边框相关快速预设*/
br()
```
import "zwtcss/zc_br"
```

/**********文宽高相关样式快速预设*/
wh()
```
import "zwtcss/zc_wh"
```

/**********定位相关样式快速预设*/
po()
```
import "zwtcss/zc_po"
```
```

### 默认引入的是rem单位为基础的，可用换单位但需要重新编译
把整个zwtcss包复制在其他文件夹，然后打开lib/base.styl 修改$u=0
然后运行npm i 安装依赖，再运行 npm run all 就会自动编译，这时编译的单位为px。
$u的值对应的数组为：[px,rem,vw,vh,vmin,vmax]，默认等于1


### 也可以分模块映入，在dist里有对应模块的css，比如内外边距模块 zc_pm.css

