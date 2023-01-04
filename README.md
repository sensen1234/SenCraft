# SenCraft
SenCraft Minecraft creative server official repository
![zzHI78.md.png](https://s1.ax1x.com/2022/12/28/zzHI78.md.png)

这个仓库会公布SenCraft的一些配置文件&插件代码

This repository will publish some configuration files & plugin code for SenCraft
![SenCraft](ttps://tietu.mclists.cn/banner/purple/5545/1.jpg)
-----------
启动参数：
```java
@echo off&setlocal enabledelayedexpansion set a=-1 :start set /a a+=1 echo ***************************************************** echo                    重启次数:%a% echo ***************************************************** title 创造 重启次数:%a% set /a s=1 for /l %%i in (1,1,!s!) do ( set /a s-=1 ping -n %s% 127.0.0.1>nul echo 倒计时开始！ !s!) echo 服务器开始运行！ "zulu18.32.13-ca-jdk18.0.2.1-win_x64\bin\java.exe" -server -Xlog:gc+init -Xlog:gc -Xmx10g -Xms10g -XX:+UseG1GC -XX:+ParallelRefProcEnabled -XX:MaxGCPauseMillis=200 -XX:+UnlockExperimentalVMOptions -XX:+UnlockDiagnosticVMOptions -XX:+DisableExplicitGC -XX:+AlwaysPreTouch -XX:G1NewSizePercent=30 -XX:G1MaxNewSizePercent=40 -XX:G1HeapRegionSize=8M -XX:G1ReservePercent=20 -XX:G1HeapWastePercent=5 -XX:G1MixedGCCountTarget=4 -XX:InitiatingHeapOccupancyPercent=15 -XX:G1MixedGCLiveThresholdPercent=90 -XX:G1RSetUpdatingPauseTimePercent=5 -XX:SurvivorRatio=32 -XX:+PerfDisableSharedMem -XX:MaxTenuringThreshold=1 -XX:-UseBiasedLocking -XX:UseAVX=3 -XX:+UseStringDeduplication -XX:+UseFastUnorderedTimeStamps -XX:+UseAES -XX:+UseAESIntrinsics -XX:UseSSE=4 -XX:+UseFMA -XX:AllocatePrefetchStyle=1 -XX:+UseLoopPredicate -XX:+RangeCheckElimination -XX:+EliminateLocks -XX:+DoEscapeAnalysis -XX:+UseCodeCacheFlushing -XX:+SegmentedCodeCache -XX:+UseFastJNIAccessors -XX:+OptimizeStringConcat -XX:+UseCompressedOops -XX:+UseThreadPriorities -XX:+OmitStackTraceInFastThrow -XX:+TrustFinalNonStaticFields -XX:ThreadPriorityPolicy=1 -XX:+UseInlineCaches -XX:+RewriteBytecodes -XX:+RewriteFrequentPairs -XX:+UseNUMA -XX:-DontCompileHugeMethods -XX:+UseFPUForSpilling -XX:+UseFastStosb -XX:+UseNewLongLShift -XX:+UseVectorCmov -XX:+UseXMMForArrayCopy -XX:+UseXmmI2D -XX:+UseXmmI2F -XX:+UseXmmLoadAndClearUpper -XX:+UseXmmRegToRegMoveAll -Dfile.encoding=UTF-8 -Xlog:async -Djava.security.egd=file:/dev/urandom --add-modules jdk.incubator.vector -jar  paper-1.19.2-307.jar -nogui goto start
```
