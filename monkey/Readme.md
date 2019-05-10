将文件 push 到 手机模拟器并运行 monkey
```
adb boot
adb remount
adb push monkey.script /data/temp/monkey.script
adb shell monkey -f /data/temp/monkey.script
```

由于模拟器的分辨率不同，脚本定位的元位置就不一样，需要你用 automatorviewer 重新修改下参数值
主要修改的是 DispatchPointer() 和 DispatchPress()