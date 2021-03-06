[![Go Report Card](https://goreportcard.com/badge/github.com/yittg/ving)](https://goreportcard.com/report/github.com/yittg/ving)

# 🐸 ving

`ving` is a visualization ping utility written in Golang(1.11+).
Special thanks to the amazing [termui](https://github.com/gizak/termui) library.

# 🦁 Features

* ping multiple targets concurrently and independently;
* ping gateway conveniently, `-g`;
* ping interval option, `-i`;
* error rate and speed statistics in sliding window, as emoji;
* responsive terminal display (based on termui).

# 🙈 Install

```
$ go get -u github.com/yittg/ving
```

> __Notes__ for linux users, run `ving` with `sudo` or `setcap` in advance, 
for more information, see the [man page](http://linux.die.net/man/7/capabilities).
>
>    ```
>    $ sudo setcap "cap_net_raw+ep" ving
>    ``` 

# ⚡ Usage

```
$ ving 192.168.0.1 127.0.0.1 8.8.8.8

$ ving -i 100ms 192.168.0.1

$ ving -g
```

![](./assets/screenshot.png)
