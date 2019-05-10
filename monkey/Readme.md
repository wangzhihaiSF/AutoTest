将文件 push 到 手机模拟器并运行 monkey
```
adb boot
adb remount
adb push monkey.script /data/temp/monkey.script
adb shell monkey -f /data/temp/monkey.script
```