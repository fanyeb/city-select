# city-select
城市选择插件，支持简拼、全拼或文字输入搜索，支持鼠标、键盘选择；

## 使用方法：

1. 引入css和js
```
<link rel="stylesheet" href="cityselect/cityselect.css">
<script type="text/javascript" src="cityselect/cityselect.js"></script>
```
2. 在输入框加入id
```
<input type="text" class="cityinput" id="citySelect" placeholder="请输入目的地">
```
3. JS创建实例，传入输入框id
```
<script type="text/javascript">
    var test=new Vcity.CitySelector({input:'citySelect'});
</script>
```

## 几点建议：
- 城市数据按照固定格式添加'北京|beijing|bj' => (名称/全拼/简拼),请按照自己的需要自己维护一份符合项目需要的城市数据,从自己的服务端获取而不是写死在js会更好.
- 很难提供一份大家都满足的全数据,加上地区的行政区划一直在调整变动,所以数据的维护还是得自己来搞定(当前的数据是仅选择到市).
- 关于城市数据的格式,其实可以按照自己的需求改变掉,变成自己更加习惯的格式,在源码里再调整下数据解析的几行代码即可.
- 插件是源码,修改起来还是很方便的,有一些小bug或者更多样的需求,可以通过阅读源码来解决.
- UI应该是最好修改的部分,按需求修改css,可能偶尔需要动几行js.

## 其它:
- city.json跟插件无关,是我留做参考的一份比较全的数据.
- 插件不是原创,有做较大幅度的改动,以前的项目使用过这个插件,现在用不到了,所以没有做什么改进,仅放在这做个分享.