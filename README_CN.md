mod_bcg729
==========

> 适用于Centos7源码安装freeswitch

切换到`freeswitch`源码的`src/mod/codecs`目录下

例如： `cd /usr/local/src/freeswitch/src/mod/codecs`

```bash
git clone https://github.com/niaiai/mod_bcg729.git
cd mod_bcg729
make
# 拷贝 mod_bcg729.so 到freeswitch的mod目录中

# 卸载g729
fs_cli -x "unload mod_g729"
# 加载bcg729
fs_cli -x "load mod_bcg729"

# 修改 autoload_configs/modules.conf.xml
```
