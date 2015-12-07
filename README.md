# area
省市区三级联动pc版

手机版的地区三级联动请至 [mobile-select-area](https://github.com/tianxiangbing/mobile-select-area)

效果图如下：

![mobile-select-area](example/area.jpg)

例子见[DEMO](http://www.lovewebgames.com/jsmodule/area.html)

##js:
        <script src="jquery-1.9.1.min.js"></script>
        <script src="area-data.js"></script>
        <script src="area.js"></script>
        <script>
        Area.init(AreaData);
        </script>

`AreaData是取的area-data.js的静态数据，也可以通过ajax一次性全读出来`

##html:

    <div class="area-input">
        <div class="area province">
            <input type="hidden" id="hd_province">
            <span>-- 省份 --</span><i></i>
            <div class="area-content"></div>
        </div>
        <div class="area city">
            <input type="hidden" id="hd_city">
            <span>-- 城市 --</span><i></i>
            <div class="area-content"><ul></ul></div>
        </div>
        <div class="area downtown">
            <input type="hidden" id="hd_downtown">
            <span>-- 市区 --</span><i></i>
            <div class="area-content"><ul></ul></div>
        </div>
    </div>

##area-data:

    "data": [{
            "id": "2",
            "name": "\u5317\u4eac\u5e02",
            "child": [{
                "id": "2288",
                "name": "\u4e1c\u57ce\u533a"
            }]
            ...
            }]