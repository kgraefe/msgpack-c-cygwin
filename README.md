# msgpack-c-cygwin

This a recipe to build and package [msgpack for C][1] on [Cygwin][2]. The
recipe is based on the [recipe in cascent's old neovim port][3].

To build the package run the following command:
```sh
cygport msgpack-c-cygwin.cygport download prepare compile install package
```

To install the package you can extract it into the root directory:
```sh
eval "$(cygport msgpack-c.cygport vars PVR)"
tar -C / -xjvf msgpack-c-$PVR.x86_64/dist/msgpack-c/libmsgpack2-$PVR.tar.xz
```

[1]: https://github.com/msgpack/msgpack-c
[2]: http://www.cygwin.com/
[3]: https://github.com/cascent/neovim-cygwin/blob/09277e3f76981189a2f15d1dbc2f5a4ab4b6c86f/msgpack-c/msgpack-c.cygport
[4]: https://github.com/kgraefe/luajit-cygwin
