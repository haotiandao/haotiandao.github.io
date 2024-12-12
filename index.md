<!DOCTYPE html>
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

 <div class="form-group"><label class="col-sm-2 control-label"> 刷新网址： </label>
                                <div class="col-sm-10">
                                    <input class="form-control" id="url" name="url" type="text" value="http://tool.bingdou.com.cn" placeholder="如：http://tool.bingdou.com.cn" style="width: 60%;"/>
                                </div>
                            </div>
                            <div class="form-group"><label class="col-sm-2 control-label"> 刷新频率(秒/次)： </label>
                                <div class="col-sm-10"><input class="form-control" id="frequency" type="text" value="5" style="width: 30%;"/></div>
                            </div>
                            <div class="form-group"><label class="col-sm-2 control-label"> 已刷新次数： </label>
                                <div class="col-sm-10"><input class="form-control" id="times" type="text" value="0" style="width: 30%;" disabled=""/></div>
                            </div>
                            <div class="form-group"><label class="col-sm-2 control-label"> 刷新网址： </label>
                                <div class="col-sm-10"><input type="button" id="startButton" onClick="startRefresh();" value="开始刷新" class="btn btn-success"> <input type="button" id="endButton" onclick="endRefresh();" value="停止刷新" class="btn btn-danger" style="display: none">
                                </div>
                          
                            <div class="form-group">
                                <div class="col-sm-12">
                                    <iframe id="frame" style="width: 100%; height: 600px; padding: 10px; border: 1px solid #66be8c;"></iframe>
                                </div>
                         
                
