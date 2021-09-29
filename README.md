# cleanhelper
用终端丝滑的清洗音频数据

## 使用说明

1. 安装依赖
pip install sounddevice
pip install pydub

2. 运行
python cleanhelper.py  指定文件夹

3. 使用
←（方向键左）： 播放上一个
↓（方向键下）： 删除当前
→（方向键右）： 播放下一个
q：退出

4. 说明
假如指定文件夹为 `./test`
- 删除的文件会被移到 `./trash/tset` 里
- 退出后会保存当前状态到文件`./test/state.plk`
- 下次运行时会读取文件`./test/state.plk`, 恢复上次退出时的状态
- 清洗完毕后可运行指令 `rm ./test/state.plk` 删除状态文件



