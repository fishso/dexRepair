# dexRepair
使用FART-frida脚本脱壳后生成*.dex和*.bin文件, 使用jadx打开dex文件后无法解析, 利用010查看二进制后发现dex缺少头部信息, 补充即可打开.

## 具体操作布置
1. 找一个正常的dex 用010 打开, 观察头部信息.
2. 找到FART脱壳后的dex 用010打开, 观察头部信息, 发现缺少 dex.035 信息, 
3. 把正常的dex头部信息c-p到缺少头部信息的dex即可.

再尝试用jadx打开, 一切正常.

# 以上操作仅适用于头部缺失的修复.



其它:
http://ascii.911cha.com/

https://www.cnblogs.com/luoyesiqiu/p/dexfix.html

https://github.com/hanbinglengyue/FART
