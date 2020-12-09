# bioformats-tests
playing around with bioformats

## Hello

This is just for a graal test, as I'm not a java person usually.

### Graal
Assuming graal is installed, you need to:

* Install native-code with `gu install native-image`
* Compile Java with `javac Hello.java`
* Make into native code with `native-image Hello`

### The Executable
My main interest here is for multi-stage builds or otherwise sharing prebuild executables. What libraries does this use?
```bash
> ldd hello
	linux-vdso.so.1 (0x00007ffd6b6dd000)
	libpthread.so.0 => /lib/x86_64-linux-gnu/libpthread.so.0 (0x00007fa2aaf79000)
	libdl.so.2 => /lib/x86_64-linux-gnu/libdl.so.2 (0x00007fa2aad75000)
	libz.so.1 => /lib/x86_64-linux-gnu/libz.so.1 (0x00007fa2aab58000)
	librt.so.1 => /lib/x86_64-linux-gnu/librt.so.1 (0x00007fa2aa950000)
	libc.so.6 => /lib/x86_64-linux-gnu/libc.so.6 (0x00007fa2aa55f000)
	/lib64/ld-linux-x86-64.so.2 (0x00007fa2abc27000)
```

Nothing here looks concerning to me as is, so continuing hopefully.
