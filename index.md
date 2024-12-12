<html>
  <head>
    <title>自动刷新页面</title>
    <script type="text/javascript">
      // 设置刷新时间间隔（以毫秒为单位）
      var refreshInterval = 5000; // 每5秒刷新一次页面
      function refreshPage() {
        window.location.reload(); // 刷新页面
      }
      // 在指定的时间间隔内重复调用refreshPage函数
      setInterval(refreshPage, refreshInterval);
    </script>
  </head>
  <body>
    <h1>这是一个自动刷新的页面</h1>
    <p>页面将在5秒钟后自动刷新。</p>
  </body>
</html>


<html>
 <head> 
  
  <!-- 次数统计 start -->
<center>
<script>
var caution = false
        function setCookie(name, value, expires, path, domain, secure) {
            var curCookie = name + "=" + escape(value) + ((expires) ? "; expires=" + expires.toGMTString() : "") + ((path) ? "; path=" + path : "") + ((domain) ? "; domain=" + domain : "") + ((secure) ? "; secure" : "")
            if (!caution || (name + "=" + escape(value)).length <= 4000)
                document.cookie = curCookie
            else if (confirm("Cookie exceeds 4KB and will be cut!"))
                document.cookie = curCookie
        }
        function getCookie(name) {
            var prefix = name + "="
            var cookieStartIndex = document.cookie.indexOf(prefix)
            if (cookieStartIndex == -1)
                return null
            var cookieEndIndex = document.cookie.indexOf(";", cookieStartIndex + prefix.length)
            if (cookieEndIndex == -1)
                cookieEndIndex = document.cookie.length
            return unescape(document.cookie.substring(cookieStartIndex + prefix.length,
                cookieEndIndex))
        }
        function deleteCookie(name, path, domain) {
            if (getCookie(name)) {
                document.cookie = name + "=" + ((path) ? "; path=" + path : "") + ((domain) ? "; domain=" + domain : "") + "; expires=Thu, 01-Jan-70 00:00:01 GMT"
            }
        }
        function fixDate(date) {
            var base = new Date(0)
            var skew = base.getTime()
            if (skew > 0)
                date.setTime(date.getTime() - skew)
        }
        var now = new Date()
        fixDate(now)
        now.setTime(now.getTime() + 730 * 24 * 60 * 60 * 1000)
        var visits = getCookie("counter")
        if (!visits)
            visits = 1
        else
            visits = parseInt(visits) + 1
        setCookie("counter", visits, now)
        document.write("<font size=2color=black>欢迎您，您是第：" + visits + " 个访问该站点的访客")

    </script>
    </center>
<!-- 次数统计 over -->

$(document).ready(function() {

var int = setinterval(fixcount, 50); // 50ms周期检测函数

var countoffset = 20000; // 初始化首次数据

function fixcount() {

if (document.getelementbyid("busuanzi_container_site_pv").style.display != "none")

{

$("#busuanzi_value_site_pv").html(parseint($("#busuanzi_value_site_pv").html()) + countoffset);

clearinterval(int);

}

if ($("#busuanzi_container_site_pv").css("display") != "none")

{

$("#busuanzi_value_site_uv").html(parseint($("#busuanzi_value_site_uv").html()) + countoffset); // 加上初始数据

clearinterval(int); // 停止检测

}

}

});
