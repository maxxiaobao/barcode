> 用于条码生成，支持 code128 ABC类编码和EAN13标准码，C类需要将barcode.js中注释的代码，重新打开

### 安装
```
浏览器导入：
<script src="js/EAN13_b.js" type="text/javascript" charset="utf-8"></script>
<script src="js/code128.js" type="text/javascript" charset="utf-8"></script>

NPM：install --save-dev canvas-barcode
var barcode=require('canvas-barcode');
```

**调用draw方法，第一个参数是canvas的id，第二个参数为每个条形模块的宽度，第三个参数为条形码高度**
```
var barcode=require('canvas-barcode');
new barcode.EAN13('535350244626').draw('canvas', 2, 100);
new barcode.code128('535350244626').draw('canvas', 2, 100);
```


```
<script src='js/EAN13_b.js'></script>
<script src='js/code128.js'></script>

<canvas id="EAN" width="500" height="300"></canvas>
<canvas id="code" width="500" height="300"></canvas>

<script>
new EAN13('123456789215').draw('EAN',2,100);
new code128('SH125896').draw('code',2,100);
console.log(a);
</script>
```