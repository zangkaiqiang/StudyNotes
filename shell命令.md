### 杀死进程
ps -a|grep openpose.bin|awk '{print $1}'|xargs -r kill -9 
