# nginx跨域配置

在nginx.conf中配置

```
http {
  ......
  add_header Access-Control-Allow-Origin *;
  add_header Access-Control-Allow-Headers X-Requested-With;
  add_header Access-Control-Allow-Methods GET,POST,OPTIONS;
  ......
}
```
这样就可以实现GET,POST,OPTIONS的跨域请求的支持

也可以 add_header Access-Control-Allow-Origin http://api.dotalk.cn; --指定允许的url;

