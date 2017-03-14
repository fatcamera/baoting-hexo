## 部署
执行 hexo clean 之后，需要将 app.conf 拷贝到 public 目录。

## 创建图标
python c:/Python27/Scripts/icon-font-to-png --css css/font-awesome.css --ttf fonts/fontawesome-webfont.ttf  --size 64 paint-brush

参见[Icon Font to PNG](https://github.com/Pythonity/icon-font-to-png)

## 图像处理
### 封面图片
convert -strip -define jpeg:dct-method=float -sampling-factor 4:2:0 -interlace Plane -density 72 -filter Lanczos -geometry "500x500^" -quality 75 input output

### 批处理正文图片
for %i in (*.jpg) do convert -strip -define jpeg:dct-method=float -sampling-factor 4:2:0 -interlace Plane -density 72 -filter Lanczos -geometry "960x300^" -quality 75 %i %~ni-960%~xi

### 压缩图片
convert -strip -define jpeg:dct-method=float -sampling-factor 4:2:0 -interlace Plane -density 72 -filter Lanczos -quality 75
