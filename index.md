<html>
  <head>
    <title>自动刷新页面</title>
    <script type="text/javascript">
      // 设置刷新时间间隔（以毫秒为单位）
      var refreshInterval = 50000000; // 每5秒刷新一次页面
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


</ul> 
   <center>
  <script id="LA-DATA-WIDGET" crossorigin="anonymous" charset="UTF-8" src="https://v6-widget.51.la/v6/KLPEMIxYMeMTDBgN/quote.js?theme=#969696,#333333,#999999,#333333,#FFFFFF,#969696,12&f=12&display=0,0,1,0,0,0,0,1"></script>
  </center>
   </footer> 
  </div> 
  <!-- Scripts --> 
  <script src="https://static.yzcdn.net/gh-proxy-ui/js/jquery.min.js"></script> 
  <script src="https://static.yzcdn.net/gh-proxy-ui/js/jquery.dropotron.min.js"></script> 
  <script src="https://static.yzcdn.net/gh-proxy-ui/js/jquery.scrollex.min.js"></script> 
  <script src="https://static.yzcdn.net/gh-proxy-ui/js/browser.min.js"></script> 
  <script src="https://static.yzcdn.net/gh-proxy-ui/js/breakpoints.min.js"></script> 
  <script src="https://static.yzcdn.net/gh-proxy-ui/js/util.js"></script> 
  <script src="https://static.yzcdn.net/gh-proxy-ui/js/main.js"></script>
  <script>
   
    document.addEventListener('DOMContentLoaded', (event) => {
        const Domain = window.location.hostname;
        const CapitalizedDomain = Domain.charAt(0).toUpperCase() + Domain.slice(1);
              https_domain = 'https://' + Domain;
        document.querySelectorAll('*').forEach(element => {
            if (element.innerHTML.includes('[DOMAIN]')) {
                element.innerHTML = element.innerHTML.replace(/\[DOMAIN\]/g, https_domain);
            }
            if (element.innerHTML.includes('[NO_HTTPS_DOMAIN]')) {
                element.innerHTML = element.innerHTML.replace(/\[NO_HTTPS_DOMAIN\]/g, Domain);
            }
            if (element.innerHTML.includes('[BIG_DOMAIN]')) {
                element.innerHTML = element.innerHTML.replace(/\[BIG_DOMAIN\]/g, CapitalizedDomain);
            }
        });
     // 显示网页内容
        document.body.style.display = 'block';
    });
</script>
 </body>
</html>

