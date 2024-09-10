g++ -O0 -g -shared -fPIC -rdynamic hooks.cpp -o libhooks.so -ldl

g++ -O0 -g -finstrument-functions -rdynamic -o myprog2 myprog2.cpp

LD_PRELOAD=./libhooks.so ./myprog2

Project presentation Video demo: https://drive.google.com/drive/u/0/folders/1XH0uIaNqUIzmmArvGMAOdy5fa9TW_3-b



