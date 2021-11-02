# Install Lua
```
wget http://www.lua.org/ftp/lua-5.4.3.tar.gz  
tar zxf lua-5.4.3.tar.gz  
cd lua-5.4.3  
make all test
lua
```

# Install LuaJIT
```
wget http://luajit.org/download/LuaJIT-2.0.5.tar.gz
tar -zxvf LuaJIT-2.0.5.tar.gz
cd LuaJIT-2.0.5
make
sudo make install
export LUAJIT_LIB=/usr/local/lib
luajit
```