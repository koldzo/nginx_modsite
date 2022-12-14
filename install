#!/bin/bash
if ! [ $SUDO_USER ];
then
  printf -- '\033[31m You need to use SUDO command! \033[0m\n';
  exit
fi
printf -- 'Downloading required script to /usr/bin/...\n';
wget -q https://github.com/koldzo/nginx_modsite/blob/main/nginx_modsite -P /usr/bin/
chmod +x /usr/bin/nginx_modsite
printf -- '\033[32m Script successfully added! \033[0m\n';

if ! command -v nginx &> /dev/null
then
    printf -- '\033[31m Nginx could not be found! \033[0m\n';
    printf -- '\033[37m Get it: sudo apt install nginx \033[0m\n';
    exit
fi
