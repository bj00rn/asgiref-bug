# asgiref-bug


Example of regression asgiref using channels 2.3.1.

The code was taken from the official Channels 2.x [tutorial](https://channels.readthedocs.io/en/2.x/tutorial/part_1.html)

Running `./manage.py runworker websocket` with `asgiref==3.4.0` gives the following error:
 
 ```
../lib/python3.8/site-packages/asgiref/server.py", line 59, in run
    event_loop = get_running_loop()
RuntimeError: no running event loop
```

using `asgiref==3.3.4` works fine

