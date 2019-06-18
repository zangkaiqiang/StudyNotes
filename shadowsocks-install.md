### install
apt install python3-pip
pip install shadowsocks

### fix
vim /usr/local/lib/python3.6/dist-packages/shadowsocks/crypto/openssl.py
修改libcrypto.EVP_CIPHER_CTX_cleanup.argtypes
:%s/cleanup/reset/
:wq

### start
ssserver -p 443 -k password -m rc4-md5
sudo ssserver -p 443 -k password -m rc4-md5 --user nobody -d start

sudo ssserver -d stop
sudo less /var/log/shadowsocks.log
