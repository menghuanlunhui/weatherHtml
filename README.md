# weather
##### html获取实时天气
made by @menghuanlunhui   <br>

###说明：
	点击weather.html获取天气，链接后面需要添加参数 ?city=XX（城市名称），比如XXX/todayWeather/weather.html?city=合肥，如果没有城市名，默认查询合肥

### 天气对接使用API参考
* 1、中国天气网	http://m.weather.com.cn/data/101110101.html 已失效
* 2、中国天气网	http://www.weather.com.cn/data/sk/101010100.html    有数据，乱码，不全，没有生活指数，没有天气图标
{
	"weatherinfo": {
		"city": "北京",
		"cityid": "101010100",
		"temp": "22",
		"WD": "北风",
		"WS": "2级",
		"SD": "19%",
		"WSE": "2",
		"time": "16:05",
		"isRadar": "1",
		"Radar": "JC_RADAR_AZ9010_JB"
	}
}

* 3、http://www.weather.com.cn/data/cityinfo/101010100.html  有数据，乱码，不全，没有生活指数，没有天气图标
{
	"weatherinfo": {
		"city": "北京",
		"cityid": "101010100",
		"temp1": "24℃",
		"temp2": "11℃",
		"weather": "雷阵雨转多云",
		"img1": "d4.gif",
		"img2": "n1.gif",
		"ptime": "11:00"
	}
}

* 4、http://www.weather.com.cn/data/zs/101010100.html  有数据，乱码，信息比较全
* 5、中华万年历	http://wthrcdn.etouch.cn/weather_mini?city=北京 通过城市名字获得天气数据，json数据
* 6、中华万年历	http://wthrcdn.etouch.cn/weather_mini?citykey=101010100 通过城市id获得天气数据，json数据
* 7、中华万年历	http://wthrcdn.etouch.cn/WeatherApi?citykey=101010100 通过城市id获得天气数据，xml文件数据,当错误时会有<error>节点
* 8、中华万年历	http://wthrcdn.etouch.cn/WeatherApi?city=北京 通过城市名字获得天气数据，xml文件数据
* 9、https://github.com/jokermonn/-Api/blob/master/CenterWeather.md 获取中国天气预报，但获取的不是实时的数据
* 10、天气网	http://api.k780.com:88/?app=weather.history&weaid=hefei&date=2018-06-22&appkey=10003&sign=b59bc3ef6191eb9f747dd4e83c99f2a4&format=json 
* 11、天气网	http://api.k780.com:88/?app=weather.future&weaid=1&&appkey=10003&sign=b59bc3ef6191eb9f747dd4e83c99f2a4&format=json 获取未来几天天气
* 12、中央天气预报	http://weather.51wnl.com/weatherinfo/GetMoreWeather?cityCode=101040100&weatherType=0 已失效
* 13、中央天气预报	http://weather.51wnl.com/weatherinfo/GetMoreWeather?cityCode=101040100&weatherType=1  已失效
* 14、天气预报：https://www.juhe.cn/docs/api/id/73
* 15、全国天气预报：https://www.juhe.cn/docs/api/id/39
* 16、小米 http://weatherapi.market.xiaomi.com/wtr-v2/weather?cityId=101121301  有数据、乱码
* 17、新浪天气预报API：http://php.weather.sina.com.cn/xml.php?city=%B1%B1%BE%A9&password=DJOYnieT8234jlsK&day=0  已失效

### 友情链接
* 天气API接口大全（nohacks.cn 收集整理）：http://www.nohacks.cn/post-35.html
* 网上的天气 API 哪一个更加可靠？：https://www.zhihu.com/question/20575288
* 免费的天气接口（满足你的大部分需求）：http://blog.csdn.net/wanghao940101/article/details/72123184
* 真正的中国天气api接口xml，json（求加精） ...：http://blog.csdn.net/fancylovejava/article/details/26102635
* 免费的天气接口（满足你的大部分需求）：http://blog.csdn.net/wanghao940101/article/details/72123184

### 通过城市名（北京/北京市）获取当前城市当前温度及未来一周天气预报 (Json数据) ：包含台湾的主要县市 
* http://wthrcdn.etouch.cn/weather_mini?city=北京市；
* https://www.sojson.com/open/api/weather/json.shtml?city=北京
* https://www.sojson.com/open/api/weather/xml.shtml?city=北京 
* http://i.tianqi.com/index.php?c=code&id=12&icon=1&py=hefei&num=5

*如有任何问题或者疑问，请留言。