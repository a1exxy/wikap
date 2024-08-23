apt install python-mutagen

pip3 install mutagen

find -iname /нужный/нам/каталог '*.mp3' -print0 | xargs -0 mid3iconv -eCP1251 --remove-v1

