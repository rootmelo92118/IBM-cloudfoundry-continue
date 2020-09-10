# 以後我有心情再來寫makedown

```shell
wget --no-check-certificate -O install.sh https://raw.githubusercontent.com/rootmelo92118/IBM-cloudfoundry-continue/master/install.sh && chmod +x install.sh  && ./install.sh
```


echo '#!/bin/bash'>>start.sh
echo 'cd v2ray'>>start.sh
echo './v2ray&'>>start.sh
echo 'sleep 9d'>>start.sh
echo 'kill -9 $(ps -ef|grep v2ray|grep -v grep|awk "'"{print \$2}"'")'>>start.sh
echo 'web: ./start.sh'>Procfile
