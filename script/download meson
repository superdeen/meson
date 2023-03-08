#!/bin/bash
#this script is to download meson file
#download and install
wget 'https://staticassets.meson.network/public/meson_cdn/v3.1.19/meson_cdn-linux-amd64.tar.gz' && tar -zxf meson_cdn-linux-amd64.tar.gz && rm -f meson_cdn-linux-amd64.tar.gz && cd ./meson_cdn-linux-amd64 && sudo ./service install meson_cdn

#continue download 
cd meson_cdn-linux-amd64 && sudo./service install meson_cdn
#show files
ls
#set token and config
sudo ./meson_cdn config set --token=opvkvyhbbgdthqckvopswayo
          --https_port=443 --cache.size=30 || true
#start service        
sudo ./service start meson_cdn  
echo "node is started"
