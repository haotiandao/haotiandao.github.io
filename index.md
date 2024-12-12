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

本站已运行：<span id=span_dt_dt style="color: #2F889A;"></span>
<script language=javascript>
    function show_date_time(){
        window.setTimeout("show_date_time()", 1000);
        // 这里修改站点开启日期
        BirthDay=new Date("12/03/2023 00:00:00");
        today=new Date();
        timeold=(today.getTime()-BirthDay.getTime());
        sectimeold=timeold/1000
        secondsold=Math.floor(sectimeold);
        msPerDay=24*60*60*1000
        e_daysold=timeold/msPerDay
        daysold=Math.floor(e_daysold);
        e_hrsold=(e_daysold-daysold)*24;
        hrsold=Math.floor(e_hrsold);
        e_minsold=(e_hrsold-hrsold)*60;
        minsold=Math.floor((e_hrsold-hrsold)*60);
        seconds=Math.floor((e_minsold-minsold)*60);
        span_dt_dt.innerHTML='<font style=color:#C40000>'+daysold+'</font> 天 <font style=color:#C40000>'+hrsold+'</font> 时 <font style=color:#C40000>'+minsold+'</font> 分 <font style=color:#C40000>'+seconds+'</font> 秒';
    }
    show_date_time();
</script>
   
