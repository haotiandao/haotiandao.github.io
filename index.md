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
