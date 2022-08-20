https://uwsgi-docs.readthedocs.io/en/latest/WSGIquickstart.html

for macOS:

> If you install Python using brew, the relevant headers are already installed for you.

use virtualenv

https://virtualenv.pypa.io/en/latest/index.html


看来init.d不是什么好方法
> If you are thinking about firing up vi and writing an init.d script for spawning uWSGI, just sit (and calm) down and make sure your system doesn’t offer a better (more modern) approach first.

https://geekflare.com/systemd-start-services-linux-7/

centos可以用systemd



https://stackoverflow.com/questions/38601440/what-is-the-point-of-uwsgi

> *"What the what?! Another thing called uwsgi?!"* you ask. Yeah, it's confusing. When you reference `uWSGI` you are talking about an http server. When you talk about `uwsgi` (all lowercase) you are talking about a [binary protocol](http://uwsgi-docs.readthedocs.io/en/latest/Protocol.html) that the `uWSGI` *server* uses to talk to other servers like `nginx`. They picked a bad name on this one.



为什么不直接Nginx到Python呢？因为Nginx没有自己实现uwsgi协议。但实现了是uWSGI支持，就这么简单。

