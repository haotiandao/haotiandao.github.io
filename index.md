
                    
                   
                        </li>
                    </ul>
                    <div class="panel">
                        <form id="form1" class="form-horizontal" action="" method="post">
                            <div class="form-group"><label class="col-sm-2 control-label"> 刷新网址： </label>
                                <div class="col-sm-10"><input class="form-control" id="url" name="url" type="text"
                                                              value="http://tools.wujingquan.com"
                                                              placeholder="如：http://tools.wujingquan.com" style="width: 60%;"/>
                                </div>
                            </div>
                            <div class="form-group"><label class="col-sm-2 control-label"> 刷新频率(秒/次)： </label>
                                <div class="col-sm-10"><input class="form-control" id="frequency" type="text" value="5"
                                                              style="width: 30%;"/></div>
                            </div>
                            <div class="form-group"><label class="col-sm-2 control-label"> 已刷新次数： </label>
                                <div class="col-sm-10"><input class="form-control" id="times" type="text" value="0"
                                                              style="width: 30%;" disabled=""/></div>
                            </div>
                            <div class="form-group"><label class="col-sm-2 control-label"> 刷新网址： </label>
                                <div class="col-sm-10"><input type="button" id="startButton" onclick="startRefresh();"
                                                              value="开始刷新" class="btn btn-success"> <input type="button"
                                                                                                           id="endButton"
                                                                                                           onclick="endRefresh();"
                                                                                                           value="停止刷新"
                                                                                                           class="btn btn-danger"
                                                                                                           style="display: none">
                                </div>
                            </div>
                            <div class="form-group"><label class="col-sm-2 control-label"> </label>
                                <div class="col-sm-10">
                                    <div class="alert alert-danger alert-dismissible text-center" id="errdiv"
                                         role="alert" style="display: none;"></div>
                                </div>
                            </div>
                            <div class="form-group">
                                <div class="col-sm-12">
                                    <iframe id="frame"
                                            style="width: 100%; height: 600px; padding: 10px; border: 1px solid #66be8c;"></iframe>
                                </div>
                            </div>
                        </form>
                    </div>
                </div>
                <div class="alert alert alert-success alert-dismissible"><h4>在线定时自动刷新网页</h4>
                    <p>1,在线定时刷新网址,定时刷新网页增加网页请求量,可在线测试网页压力,可自定义刷新间隔时间</p>
                    <p>2,如果间隔时间太短，本工具可能会给你的网站带来一些访问压力。</p>
                    <p>3,请不要恶意操作刷新别的网站,文明友善地使用本工具</p></div>
                <div class="accordion-group"></div>
            </div>
        </div>
    </div>
</div>
<
})();
</script>
        </div>
    </div>
</div>
<a class="gotop" href="#top" title="返回顶部" style="display: none;"><span class="arrow"></span><span
        class="arrow lit"></span></a>
<script>tj();</script>
</body>
</html>
