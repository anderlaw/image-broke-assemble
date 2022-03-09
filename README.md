# image-broke-assemble
一个图片效果插件，一张图片即可实现一些好玩有趣的动画效果

![20220309080801-7c011ad592 gif-2-mp4 com](https://user-images.githubusercontent.com/21139011/157376986-2f11e38b-c02c-4c6c-9051-7a2150319af2.gif)

## 使用方法
### 实例化容器
```
const imgTransformer = new ImageTransformer('#img-container')
```
### 配置项（可选）
```
imgTransformer.config({
    containerWidth: 450,//容器的限宽
    effect: 'grow',//动作效果：有slide、grow、fly三种
    columnCount: 6,//水平方向切块个数
    rowCount: 6,//垂直方向切块个数
})
```
### 开启运动轨迹
```
imgTransformer.initImgData(base64OrUrl, () => {
    imgTransformer.execute()
})
```
提示：如果因某种原因导致图片跨域不能访问，你可以考虑将其转换为base64的形式

### 在线demo
https://anderlaw.github.io/image-broke-assemble/
