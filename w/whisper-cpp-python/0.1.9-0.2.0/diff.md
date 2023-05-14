# Comparing `tmp/whisper_cpp_python-0.1.9.tar.gz` & `tmp/whisper_cpp_python-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_cpp_python-0.1.9.tar", last modified: Tue May  9 03:55:33 2023, max compression
+gzip compressed data, was "whisper_cpp_python-0.2.0.tar", last modified: Sun May 14 21:58:47 2023, max compression
```

## Comparing `whisper_cpp_python-0.1.9.tar` & `whisper_cpp_python-0.2.0.tar`

### file list

```diff
@@ -1,531 +1,537 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.036630 whisper_cpp_python-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-09 03:55:17.000000 whisper_cpp_python-0.1.9/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-09 03:55:33.036630 whisper_cpp_python-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:17.000000 whisper_cpp_python-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-09 03:55:17.000000 whisper_cpp_python-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 03:55:33.036630 whisper_cpp_python-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-05-09 03:55:17.000000 whisper_cpp_python-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.976630 whisper_cpp_python-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-09 03:55:17.000000 whisper_cpp_python-0.1.9/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.964629 whisper_cpp_python-0.1.9/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.964629 whisper_cpp_python-0.1.9/vendor/pycparser/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.964629 whisper_cpp_python-0.1.9/vendor/pycparser/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.984630 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.984630 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/X11/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/X11/Intrinsic.h
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/X11/Xlib.h
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/X11/_X11_fake_defines.h
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/X11/_X11_fake_typedefs.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/_ansi.h
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/_fake_defines.h
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/_fake_typedefs.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/_syslist.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/aio.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/alloca.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/ar.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/argz.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.984630 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/arpa/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/arpa/inet.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.988630 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/asm-generic/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/asm-generic/int-ll64.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/assert.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/complex.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/cpio.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/ctype.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/dirent.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/dlfcn.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/emmintrin.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/endian.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/envz.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/errno.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/fastmath.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/fcntl.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/features.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/fenv.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/float.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/fmtmsg.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/fnmatch.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/ftw.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/getopt.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/glob.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/grp.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/iconv.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/ieeefp.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/immintrin.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/inttypes.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/iso646.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/langinfo.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/libgen.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/libintl.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/limits.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.988630 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/linux/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/linux/socket.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/linux/version.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/locale.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/malloc.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/math.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.988630 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/mir_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/mir_toolkit/client_types.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/monetary.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/mqueue.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/ndbm.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.988630 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/net/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/net/if.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/netdb.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.988630 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/netinet/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/netinet/in.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/netinet/tcp.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/newlib.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/nl_types.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.988630 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/openssl/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/openssl/err.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/openssl/evp.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/openssl/hmac.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/openssl/ssl.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/openssl/x509v3.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/paths.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/poll.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/process.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/pthread.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/pwd.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/reent.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/regdef.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/regex.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sched.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/search.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/semaphore.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/setjmp.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/signal.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/smmintrin.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/spawn.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/stdalign.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/stdarg.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/stdatomic.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/stdbool.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/stddef.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/stdint.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/stdio.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/stdlib.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/stdnoreturn.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/string.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/strings.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/stropts.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.988630 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sys/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sys/ioctl.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sys/ipc.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sys/mman.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sys/msg.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sys/poll.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sys/resource.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sys/select.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sys/sem.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sys/shm.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sys/socket.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sys/stat.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sys/statvfs.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sys/sysctl.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sys/time.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sys/times.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sys/types.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sys/uio.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sys/un.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sys/utsname.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/sys/wait.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/syslog.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/tar.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/termios.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/tgmath.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/threads.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/time.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/trace.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/ulimit.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/unctrl.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/unistd.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/utime.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/utmp.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/utmpx.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/wchar.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/wctype.h
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/wordexp.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.988630 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/xcb/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/xcb/xcb.h
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/zlib.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.992630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.964629 whisper_cpp_python-0.1.9/vendor/whisper.cpp/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.992630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/.github/workflows/bindings-go.yml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/.github/workflows/bindings-ruby.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/.github/workflows/examples.yml
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11058 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    28943 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.992630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.996630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/doc.go
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.964629 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.996630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/examples/go-model-download/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/examples/go-model-download/context.go
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/examples/go-model-download/main.go
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.996630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/examples/go-whisper/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/examples/go-whisper/color.go
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/examples/go-whisper/flags.go
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/examples/go-whisper/main.go
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/examples/go-whisper/process.go
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/go.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/go.sum
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/params.go
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.964629 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.996630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/pkg/whisper/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/pkg/whisper/consts.go
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/pkg/whisper/context.go
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/pkg/whisper/context_test.go
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/pkg/whisper/doc.go
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/pkg/whisper/interface.go
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/pkg/whisper/model.go
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.996630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/samples/
--rw-r--r--   0 runner    (1001) docker     (123)   352078 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/samples/jfk.wav
--rw-r--r--   0 runner    (1001) docker     (123)    14538 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/whisper.go
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/whisper_test.go
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.996630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.968629 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.996630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-09 03:55:19.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/.github/workflows/swift.yml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-09 03:55:19.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-09 03:55:19.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-09 03:55:19.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-09 03:55:19.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Makefile-tmpl
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-09 03:55:19.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Package.swift
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-09 03:55:19.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.968629 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Sources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.996630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Sources/test-objc/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-09 03:55:19.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Sources/test-objc/main.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.996630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Sources/test-swift/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-09 03:55:19.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Sources/test-swift/main.swift
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.000630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Sources/whisper/
--rw-r--r--   0 runner    (1001) docker     (123)   425638 2023-05-09 03:55:19.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml.c
--rw-r--r--   0 runner    (1001) docker     (123)    30532 2023-05-09 03:55:19.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.000630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Sources/whisper/include/
--rw-r--r--   0 runner    (1001) docker     (123)    23720 2023-05-09 03:55:19.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Sources/whisper/include/whisper.h
--rw-r--r--   0 runner    (1001) docker     (123)   183212 2023-05-09 03:55:19.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Sources/whisper/whisper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.000630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/models/
--rw-r--r--   0 runner    (1001) docker     (123)   586836 2023-05-09 03:55:19.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/models/for-tests-ggml-base.en.bin
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:19.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/publish-trigger
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.000630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/javascript/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/javascript/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/javascript/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/javascript/emscripten.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/javascript/libwhisper.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/javascript/package-tmpl.json
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/javascript/package.json
--rw-r--r--   0 runner    (1001) docker     (123)   795866 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/javascript/whisper.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.968629 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ruby/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.000630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ruby/ext/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ruby/ext/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ruby/ext/extconf.rb
--rw-r--r--   0 runner    (1001) docker     (123)    15308 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ruby/ext/ruby_whisper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ruby/ext/ruby_whisper.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.000630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ruby/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ruby/tests/test_whisper.rb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.004630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/cmake/BuildTypes.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/cmake/DefaultTargetOptions.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/cmake/GitVars.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.004630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/coreml/
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/coreml/whisper-decoder-impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/coreml/whisper-decoder-impl.m
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/coreml/whisper-encoder-impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/coreml/whisper-encoder-impl.m
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/coreml/whisper-encoder.h
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/coreml/whisper-encoder.mm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.004630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.008630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/addon.node/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/addon.node/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/addon.node/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/addon.node/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.008630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/addon.node/__test__/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/addon.node/__test__/whisper.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/addon.node/addon.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/addon.node/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/addon.node/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.008630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/bench/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/bench/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/bench/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/bench/bench.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.008630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/bench.wasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/bench.wasm/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/bench.wasm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/bench.wasm/emscripten.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/bench.wasm/index-tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.008630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/command/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/command/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/command/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    24877 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/command/command.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/command/commands.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.008630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/command.wasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/command.wasm/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/command.wasm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/command.wasm/emscripten.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16219 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/command.wasm/index-tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/common-ggml.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/common-ggml.h
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/common-sdl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/common-sdl.h
--rw-r--r--   0 runner    (1001) docker     (123)    15650 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/common.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/common.h
--rw-r--r--   0 runner    (1001) docker     (123)   241358 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/dr_wav.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1197 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/generate-karaoke.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/helpers.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     2955 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/livestream.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.008630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/main/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/main/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/main/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    36271 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/main/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.008630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/quantize/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/quantize/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/quantize/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/quantize/quantize.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.008630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/stream/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/stream/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/stream/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/stream/stream.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.008630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/stream.wasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/stream.wasm/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/stream.wasm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/stream.wasm/emscripten.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16188 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/stream.wasm/index-tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.012630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk/eleven-labs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27945 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk/gpt-2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk/gpt-2.h
--rwxr-xr-x   0 runner    (1001) docker     (123)      563 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk/speak.sh
--rw-r--r--   0 runner    (1001) docker     (123)    14593 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk/talk.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.012630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk-llama/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk-llama/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk-llama/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk-llama/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk-llama/eleven-labs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk-llama/llama-util.h
--rw-r--r--   0 runner    (1001) docker     (123)    94701 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk-llama/llama.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk-llama/llama.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.012630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk-llama/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk-llama/prompts/talk-alpaca.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk-llama/speak.sh
--rw-r--r--   0 runner    (1001) docker     (123)    27971 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk-llama/talk-llama.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.012630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk.wasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk.wasm/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk.wasm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk.wasm/emscripten.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    27945 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk.wasm/gpt-2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk.wasm/gpt-2.h
--rw-r--r--   0 runner    (1001) docker     (123)    33143 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk.wasm/index-tmpl.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     2757 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/twitch.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.016630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.016630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/.idea/compiler.xml
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/.idea/gradle.xml
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.016630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/build.gradle
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/proguard-rules.pro
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.972629 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.968629 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.968629 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/java/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.968629 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.016630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/whispercppdemo/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/whispercppdemo/ExampleInstrumentedTest.kt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.016630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/AndroidManifest.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.968629 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.968629 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.016630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/MainActivity.kt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.016630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/media/
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/media/RiffWaveHelper.kt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.016630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/recorder/
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/recorder/Recorder.kt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.968629 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.016630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreen.kt
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreenViewModel.kt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.016630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Color.kt
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Theme.kt
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Type.kt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.016630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/whisper/
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/whisper/LibWhisper.kt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.968629 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.016630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Android.mk
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Application.mk
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Whisper.mk
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/jni.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.972629 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.016630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_background.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_foreground.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.016630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/mipmap-anydpi/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/mipmap-anydpi/ic_launcher.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.020630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/values/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/values/colors.xml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/values/strings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/values/themes.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.020630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/xml/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/xml/backup_rules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/xml/data_extraction_rules.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.972629 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.972629 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/test/java/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.972629 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/test/java/com/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.020630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/test/java/com/whispercppdemo/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/test/java/com/whispercppdemo/ExampleUnitTest.kt
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/build.gradle
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.972629 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/gradle/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.020630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/gradle/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)    59203 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.jar
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.properties
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/gradle.properties
--rwxr-xr-x   0 runner    (1001) docker     (123)     5766 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/gradlew
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/gradlew.bat
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/settings.gradle
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.020630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.nvim/
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.nvim/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     2032 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.nvim/whisper.nvim
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.020630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.020630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.h
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.020630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.020630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AccentColor.colorset/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AccentColor.colorset/Contents.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.020630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AppIcon.appiconset/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AppIcon.appiconset/Contents.json
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/Contents.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.020630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/LaunchScreen.storyboard
--rw-r--r--   0 runner    (1001) docker     (123)     8419 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/Main.storyboard
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Info.plist
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.h
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.m
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.h
--rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.m
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/main.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.020630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/
--rw-r--r--   0 runner    (1001) docker     (123)    17120 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.pbxproj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.020630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/contents.xcworkspacedata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.020630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/xcshareddata/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.020630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.024630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/LibWhisper.swift
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/WhisperCppDemo-Bridging-Header.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.024630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.024630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Models/
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Models/WhisperState.swift
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.972629 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.024630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/models/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.024630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/samples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/samples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.024630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/UI/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/UI/ContentView.swift
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.024630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/Recorder.swift
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/RiffWaveUtils.swift
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/WhisperCppDemoApp.swift
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.024630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    21447 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.pbxproj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.024630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.024630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/xcshareddata/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:32.972629 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.024630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/xcschemes/
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/xcschemes/WhisperCppDemo.xcscheme
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.024630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.wasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.wasm/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.wasm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.wasm/emscripten.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    33017 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.wasm/index-tmpl.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     6932 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/yt-wsp.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.024630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/extra/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2459 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/extra/bench-all.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/extra/bench-wts.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      297 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/extra/convert-all.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1152 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/extra/deploy-wasm.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2034 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/extra/quantize-all.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      134 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/extra/sha-all.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      596 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/extra/sync-ggml.sh
--rw-r--r--   0 runner    (1001) docker     (123)    24594 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/ggml-cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/ggml-cuda.h
--rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/ggml-opencl.c
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/ggml-opencl.h
--rw-r--r--   0 runner    (1001) docker     (123)   423265 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/ggml.c
--rw-r--r--   0 runner    (1001) docker     (123)    31202 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/ggml.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.032630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/convert-h5-to-ggml.py
--rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/convert-pt-to-ggml.py
--rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/convert-whisper-to-coreml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2128 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/download-coreml-model.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/download-ggml-model.cmd
--rwxr-xr-x   0 runner    (1001) docker     (123)     2010 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/download-ggml-model.sh
--rw-r--r--   0 runner    (1001) docker     (123)   575451 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/for-tests-ggml-base.bin
--rw-r--r--   0 runner    (1001) docker     (123)   586836 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/for-tests-ggml-base.en.bin
--rw-r--r--   0 runner    (1001) docker     (123)   575451 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/for-tests-ggml-large.bin
--rw-r--r--   0 runner    (1001) docker     (123)   575451 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/for-tests-ggml-medium.bin
--rw-r--r--   0 runner    (1001) docker     (123)   586836 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/for-tests-ggml-medium.en.bin
--rw-r--r--   0 runner    (1001) docker     (123)   575451 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/for-tests-ggml-small.bin
--rw-r--r--   0 runner    (1001) docker     (123)   586836 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/for-tests-ggml-small.en.bin
--rw-r--r--   0 runner    (1001) docker     (123)   575451 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/for-tests-ggml-tiny.bin
--rw-r--r--   0 runner    (1001) docker     (123)   586836 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/for-tests-ggml-tiny.en.bin
--rwxr-xr-x   0 runner    (1001) docker     (123)     1471 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/generate-coreml-interface.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      769 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/generate-coreml-model.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.032630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/samples/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/samples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/samples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   352078 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/samples/jfk.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.036630 whisper_cpp_python-0.1.9/vendor/whisper.cpp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/tests/en-0-ref.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/tests/en-1-ref.txt
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/tests/en-2-ref.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/tests/es-0-ref.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     3432 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/tests/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/tests/test-whisper.js
--rw-r--r--   0 runner    (1001) docker     (123)   184690 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/whisper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23750 2023-05-09 03:55:18.000000 whisper_cpp_python-0.1.9/vendor/whisper.cpp/whisper.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.036630 whisper_cpp_python-0.1.9/whisper_cpp_python/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 03:55:17.000000 whisper_cpp_python-0.1.9/whisper_cpp_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-09 03:55:17.000000 whisper_cpp_python-0.1.9/whisper_cpp_python/whisper.py
--rw-r--r--   0 runner    (1001) docker     (123)    30596 2023-05-09 03:55:32.000000 whisper_cpp_python-0.1.9/whisper_cpp_python/whisper_cpp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:33.036630 whisper_cpp_python-0.1.9/whisper_cpp_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-09 03:55:32.000000 whisper_cpp_python-0.1.9/whisper_cpp_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22209 2023-05-09 03:55:32.000000 whisper_cpp_python-0.1.9/whisper_cpp_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 03:55:32.000000 whisper_cpp_python-0.1.9/whisper_cpp_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-09 03:55:32.000000 whisper_cpp_python-0.1.9/whisper_cpp_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-09 03:55:32.000000 whisper_cpp_python-0.1.9/whisper_cpp_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.629019 whisper_cpp_python-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-14 21:58:31.000000 whisper_cpp_python-0.2.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-14 21:58:31.000000 whisper_cpp_python-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-14 21:58:47.629019 whisper_cpp_python-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-14 21:58:31.000000 whisper_cpp_python-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-14 21:58:31.000000 whisper_cpp_python-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 21:58:47.633019 whisper_cpp_python-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-05-14 21:58:31.000000 whisper_cpp_python-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.549019 whisper_cpp_python-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-14 21:58:31.000000 whisper_cpp_python-0.2.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.537020 whisper_cpp_python-0.2.0/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.537020 whisper_cpp_python-0.2.0/vendor/pycparser/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.537020 whisper_cpp_python-0.2.0/vendor/pycparser/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.561020 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.561020 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/X11/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/X11/Intrinsic.h
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/X11/Xlib.h
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/X11/_X11_fake_defines.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/X11/_X11_fake_typedefs.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/_ansi.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/_fake_defines.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/_fake_typedefs.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/_syslist.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/aio.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/alloca.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/ar.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/argz.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.561020 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/arpa/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/arpa/inet.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.561020 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/asm-generic/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/asm-generic/int-ll64.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/assert.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/cpio.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/ctype.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/dirent.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/dlfcn.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/emmintrin.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/endian.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/envz.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/errno.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/fastmath.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/fcntl.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/features.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/fenv.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/float.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/fmtmsg.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/fnmatch.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/ftw.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/getopt.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/glob.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/grp.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/iconv.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/ieeefp.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/immintrin.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/inttypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/iso646.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/langinfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/libgen.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/libintl.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/limits.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.561020 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/linux/socket.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/linux/version.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/locale.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/malloc.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/math.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.561020 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/mir_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/mir_toolkit/client_types.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/monetary.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/mqueue.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/ndbm.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.561020 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/net/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/net/if.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/netdb.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.565019 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/netinet/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/netinet/in.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/netinet/tcp.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/newlib.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/nl_types.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.565019 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/openssl/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/openssl/err.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/openssl/evp.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/openssl/hmac.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/openssl/ssl.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/openssl/x509v3.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/paths.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/poll.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/process.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/pthread.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/pwd.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/reent.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/regdef.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/regex.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sched.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/search.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/semaphore.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/setjmp.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/signal.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/smmintrin.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/spawn.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/stdalign.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/stdarg.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/stdatomic.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/stdbool.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/stddef.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/stdint.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/stdio.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/stdlib.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/stdnoreturn.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/string.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/strings.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/stropts.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.565019 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sys/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sys/ioctl.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sys/ipc.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sys/mman.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sys/msg.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sys/poll.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sys/resource.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sys/select.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sys/sem.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sys/shm.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sys/socket.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sys/stat.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sys/statvfs.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sys/sysctl.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sys/time.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sys/times.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sys/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sys/uio.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sys/un.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sys/utsname.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/sys/wait.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/syslog.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/tar.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/termios.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/tgmath.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/threads.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/time.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/trace.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/ulimit.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/unctrl.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/unistd.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/utime.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/utmp.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/utmpx.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/wchar.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/wctype.h
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/wordexp.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.565019 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/xcb/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/xcb/xcb.h
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/zlib.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.569019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.537020 whisper_cpp_python-0.2.0/vendor/whisper.cpp/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.569019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/.github/workflows/bindings-go.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/.github/workflows/bindings-ruby.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/.github/workflows/examples.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11058 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    28943 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.569019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.573019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/doc.go
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.537020 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.573019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/examples/go-model-download/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/examples/go-model-download/context.go
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/examples/go-model-download/main.go
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.573019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/examples/go-whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/examples/go-whisper/color.go
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/examples/go-whisper/flags.go
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/examples/go-whisper/main.go
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/examples/go-whisper/process.go
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/go.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/go.sum
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/params.go
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.537020 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.573019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/pkg/whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/pkg/whisper/consts.go
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/pkg/whisper/context.go
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/pkg/whisper/context_test.go
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/pkg/whisper/doc.go
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/pkg/whisper/interface.go
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/pkg/whisper/model.go
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.573019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)   352078 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/samples/jfk.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    14538 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/whisper.go
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/whisper_test.go
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.573019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.537020 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.573019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-14 21:58:33.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/.github/workflows/swift.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-14 21:58:33.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-14 21:58:33.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-14 21:58:33.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-14 21:58:33.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Makefile-tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-14 21:58:33.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Package.swift
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-14 21:58:33.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.541020 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Sources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.573019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Sources/test-objc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-14 21:58:33.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Sources/test-objc/main.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.577019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Sources/test-swift/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-14 21:58:33.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Sources/test-swift/main.swift
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.577019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Sources/whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)   425638 2023-05-14 21:58:33.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30532 2023-05-14 21:58:33.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.577019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Sources/whisper/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    23720 2023-05-14 21:58:33.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Sources/whisper/include/whisper.h
+-rw-r--r--   0 runner    (1001) docker     (123)   183212 2023-05-14 21:58:33.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Sources/whisper/whisper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.577019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/models/
+-rw-r--r--   0 runner    (1001) docker     (123)   586836 2023-05-14 21:58:33.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/models/for-tests-ggml-base.en.bin
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:33.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/publish-trigger
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.577019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/javascript/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/javascript/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/javascript/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/javascript/emscripten.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/javascript/libwhisper.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/javascript/package-tmpl.json
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/javascript/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)   795866 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/javascript/whisper.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.541020 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ruby/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.581019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ruby/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ruby/ext/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ruby/ext/extconf.rb
+-rw-r--r--   0 runner    (1001) docker     (123)    15308 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ruby/ext/ruby_whisper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ruby/ext/ruby_whisper.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.581019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ruby/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ruby/tests/test_whisper.rb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.581019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/cmake/BuildTypes.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/cmake/DefaultTargetOptions.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/cmake/GitVars.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.581019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/coreml/
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/coreml/whisper-decoder-impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/coreml/whisper-decoder-impl.m
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/coreml/whisper-encoder-impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/coreml/whisper-encoder-impl.m
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/coreml/whisper-encoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/coreml/whisper-encoder.mm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.581019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.585019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/addon.node/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/addon.node/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/addon.node/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/addon.node/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.585019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/addon.node/__test__/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/addon.node/__test__/whisper.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/addon.node/addon.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/addon.node/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/addon.node/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.585019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/bench/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/bench/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/bench/bench.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.585019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/bench.wasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/bench.wasm/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/bench.wasm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/bench.wasm/emscripten.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/bench.wasm/index-tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.585019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/command/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/command/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    24877 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/command/command.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/command/commands.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.585019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/command.wasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/command.wasm/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/command.wasm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/command.wasm/emscripten.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16219 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/command.wasm/index-tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/common-ggml.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/common-ggml.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/common-sdl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/common-sdl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15650 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/common.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)   241358 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/dr_wav.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1197 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/generate-karaoke.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/helpers.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2955 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/livestream.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.585019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/main/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/main/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/main/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    36271 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/main/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.585019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/quantize/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/quantize/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/quantize/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/quantize/quantize.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.589019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/stream/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/stream/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/stream/stream.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.589019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/stream.wasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/stream.wasm/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/stream.wasm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/stream.wasm/emscripten.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16188 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/stream.wasm/index-tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.589019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk/eleven-labs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27945 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk/gpt-2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk/gpt-2.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)      563 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk/speak.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    14593 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk/talk.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.589019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk-llama/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk-llama/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk-llama/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk-llama/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk-llama/eleven-labs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk-llama/llama-util.h
+-rw-r--r--   0 runner    (1001) docker     (123)    94701 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk-llama/llama.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk-llama/llama.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.589019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk-llama/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk-llama/prompts/talk-alpaca.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk-llama/speak.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    27971 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk-llama/talk-llama.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.593019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk.wasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk.wasm/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk.wasm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk.wasm/emscripten.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27945 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk.wasm/gpt-2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk.wasm/gpt-2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    33143 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk.wasm/index-tmpl.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2757 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/twitch.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.593019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.593019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/.idea/compiler.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/.idea/gradle.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.597019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/build.gradle
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/proguard-rules.pro
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.545019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.541020 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.541020 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/java/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.541020 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.597019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/whispercppdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/whispercppdemo/ExampleInstrumentedTest.kt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.597019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/AndroidManifest.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.541020 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.541020 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.597019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/MainActivity.kt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.597019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/media/
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/media/RiffWaveHelper.kt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.597019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/recorder/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/recorder/Recorder.kt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.541020 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.597019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreen.kt
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreenViewModel.kt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.597019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Color.kt
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Theme.kt
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Type.kt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.597019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/whisper/LibWhisper.kt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.545019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.601019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Android.mk
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Application.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Whisper.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/jni.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.545019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.601019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_background.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_foreground.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.601019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/mipmap-anydpi/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/mipmap-anydpi/ic_launcher.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.601019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/values/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/values/colors.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/values/strings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/values/themes.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.601019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/xml/backup_rules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/xml/data_extraction_rules.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.545019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.545019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/test/java/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.545019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/test/java/com/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.601019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/test/java/com/whispercppdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/test/java/com/whispercppdemo/ExampleUnitTest.kt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/build.gradle
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.545019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/gradle/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.601019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/gradle/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)    59203 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.jar
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.properties
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/gradle.properties
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5766 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/gradlew
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/gradlew.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/settings.gradle
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.605019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.nvim/
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.nvim/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2032 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.nvim/whisper.nvim
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.605019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.605019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.605019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.605019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AccentColor.colorset/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AccentColor.colorset/Contents.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.609019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AppIcon.appiconset/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/Contents.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.609019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/LaunchScreen.storyboard
+-rw-r--r--   0 runner    (1001) docker     (123)     8419 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/Main.storyboard
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Info.plist
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.m
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.m
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/main.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.605019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/
+-rw-r--r--   0 runner    (1001) docker     (123)    17120 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.pbxproj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.605019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/contents.xcworkspacedata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.605019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/xcshareddata/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.609019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.609019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/LibWhisper.swift
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/WhisperCppDemo-Bridging-Header.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.609019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.609019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Models/WhisperState.swift
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.545019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.609019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/models/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.609019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/samples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.609019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/UI/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/UI/ContentView.swift
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.609019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/Recorder.swift
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/RiffWaveUtils.swift
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/WhisperCppDemoApp.swift
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.613019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    21447 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.pbxproj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.613019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.613019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/xcshareddata/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.545019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.613019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/xcschemes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/xcschemes/WhisperCppDemo.xcscheme
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.613019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.wasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.wasm/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.wasm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.wasm/emscripten.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    33017 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.wasm/index-tmpl.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6932 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/yt-wsp.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.613019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/extra/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2459 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/extra/bench-all.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/extra/bench-wts.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      297 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/extra/convert-all.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1152 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/extra/deploy-wasm.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2034 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/extra/quantize-all.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      134 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/extra/sha-all.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      596 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/extra/sync-ggml.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    24594 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/ggml-cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/ggml-cuda.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/ggml-opencl.c
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/ggml-opencl.h
+-rw-r--r--   0 runner    (1001) docker     (123)   423265 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/ggml.c
+-rw-r--r--   0 runner    (1001) docker     (123)    31202 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/ggml.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.625019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/convert-h5-to-ggml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/convert-pt-to-ggml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/convert-whisper-to-coreml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2128 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/download-coreml-model.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/download-ggml-model.cmd
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2010 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/download-ggml-model.sh
+-rw-r--r--   0 runner    (1001) docker     (123)   575451 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/for-tests-ggml-base.bin
+-rw-r--r--   0 runner    (1001) docker     (123)   586836 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/for-tests-ggml-base.en.bin
+-rw-r--r--   0 runner    (1001) docker     (123)   575451 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/for-tests-ggml-large.bin
+-rw-r--r--   0 runner    (1001) docker     (123)   575451 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/for-tests-ggml-medium.bin
+-rw-r--r--   0 runner    (1001) docker     (123)   586836 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/for-tests-ggml-medium.en.bin
+-rw-r--r--   0 runner    (1001) docker     (123)   575451 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/for-tests-ggml-small.bin
+-rw-r--r--   0 runner    (1001) docker     (123)   586836 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/for-tests-ggml-small.en.bin
+-rw-r--r--   0 runner    (1001) docker     (123)   575451 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/for-tests-ggml-tiny.bin
+-rw-r--r--   0 runner    (1001) docker     (123)   586836 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/for-tests-ggml-tiny.en.bin
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1471 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/generate-coreml-interface.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      769 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/generate-coreml-model.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.625019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/samples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/samples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   352078 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/samples/jfk.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.629019 whisper_cpp_python-0.2.0/vendor/whisper.cpp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/tests/en-0-ref.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/tests/en-1-ref.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/tests/en-2-ref.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/tests/es-0-ref.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3432 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/tests/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/tests/test-whisper.js
+-rw-r--r--   0 runner    (1001) docker     (123)   184690 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/whisper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23750 2023-05-14 21:58:32.000000 whisper_cpp_python-0.2.0/vendor/whisper.cpp/whisper.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.629019 whisper_cpp_python-0.2.0/whisper_cpp_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-14 21:58:31.000000 whisper_cpp_python-0.2.0/whisper_cpp_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.629019 whisper_cpp_python-0.2.0/whisper_cpp_python/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:31.000000 whisper_cpp_python-0.2.0/whisper_cpp_python/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-14 21:58:31.000000 whisper_cpp_python-0.2.0/whisper_cpp_python/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-14 21:58:31.000000 whisper_cpp_python-0.2.0/whisper_cpp_python/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-14 21:58:31.000000 whisper_cpp_python-0.2.0/whisper_cpp_python/whisper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30596 2023-05-14 21:58:47.000000 whisper_cpp_python-0.2.0/whisper_cpp_python/whisper_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-14 21:58:31.000000 whisper_cpp_python-0.2.0/whisper_cpp_python/whisper_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:47.629019 whisper_cpp_python-0.2.0/whisper_cpp_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-14 21:58:47.000000 whisper_cpp_python-0.2.0/whisper_cpp_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22362 2023-05-14 21:58:47.000000 whisper_cpp_python-0.2.0/whisper_cpp_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 21:58:47.000000 whisper_cpp_python-0.2.0/whisper_cpp_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-14 21:58:47.000000 whisper_cpp_python-0.2.0/whisper_cpp_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 21:58:47.000000 whisper_cpp_python-0.2.0/whisper_cpp_python.egg-info/top_level.txt
```

### Comparing `whisper_cpp_python-0.1.9/pyproject.toml` & `whisper_cpp_python-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whisper_cpp_python"
-version = "0.1.9"
+version = "0.2.0"
 description = "Python bindings for the whisper.cpp library"
 authors = ["Carlos Cardoso Dias <carlosdias.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/carloscdias/whisper-cpp-python"
 repository = "https://github.com/carloscdias/whisper-cpp-python"
 packages = [{include = "whisper_cpp_python"}]
```

### Comparing `whisper_cpp_python-0.1.9/setup.py` & `whisper_cpp_python-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -215,23 +215,27 @@
 
     # Copy built C-extensions back to the project.
     setup(
         name="whisper_cpp_python",
         description="A Python wrapper for whisper.cpp",
         long_description=long_description,
         long_description_content_type="text/markdown",
-        version="0.1.9",
+        version="0.2.0",
         author="Carlos Cardoso Dias",
         author_email="carlosdias.dev@gmail.com",
         license="MIT",
-        package_dir={"whisper_cpp_python": "whisper_cpp_python"},
-        packages=["whisper_cpp_python"],
+        package_dir={"whisper_cpp_python": "whisper_cpp_python", "whisper_cpp_python.server": "whisper_cpp_python/server"},
+        packages=["whisper_cpp_python", "whisper_cpp_python.server"],
         install_requires=[
             "librosa>=0.10.0.post2",
+            "typing-extensions>=4.5.0",
         ],
+        extras_require={
+            "server": ["uvicorn>=0.21.1", "fastapi>=0.95.0", "sse-starlette>=1.3.3", "python-multipart>=0.0.6"],
+        },
         python_requires=">=3.9",
         classifiers=[
             "Programming Language :: Python :: 3",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: 3.11",
         ],
```

### Comparing `whisper_cpp_python-0.1.9/tests/test.py` & `whisper_cpp_python-0.2.0/tests/test.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/X11/_X11_fake_typedefs.h` & `whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/X11/_X11_fake_typedefs.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/_fake_defines.h` & `whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/_fake_defines.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/_fake_typedefs.h` & `whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/_fake_typedefs.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/pycparser/utils/fake_libc_include/zlib.h` & `whisper_cpp_python-0.2.0/vendor/pycparser/utils/fake_libc_include/zlib.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/.github/workflows/build.yml` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/.github/workflows/examples.yml` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/.github/workflows/examples.yml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/.gitignore` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/.gitignore`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/CMakeLists.txt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/LICENSE` & `whisper_cpp_python-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/Makefile` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/Makefile`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/README.md` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/CMakeLists.txt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/LICENSE` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/Makefile` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/Makefile`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/README.md` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/examples/go-model-download/context.go` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/examples/go-model-download/context.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/examples/go-model-download/main.go` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/examples/go-model-download/main.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/examples/go-whisper/color.go` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/examples/go-whisper/color.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/examples/go-whisper/flags.go` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/examples/go-whisper/flags.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/examples/go-whisper/main.go` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/examples/go-whisper/main.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/examples/go-whisper/process.go` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/examples/go-whisper/process.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/go.sum` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/go.sum`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/params.go` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/params.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/pkg/whisper/consts.go` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/pkg/whisper/consts.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/pkg/whisper/context.go` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/pkg/whisper/context.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/pkg/whisper/context_test.go` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/pkg/whisper/context_test.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/pkg/whisper/interface.go` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/pkg/whisper/interface.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/pkg/whisper/model.go` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/pkg/whisper/model.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/samples/jfk.wav` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/samples/jfk.wav`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/whisper.go` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/whisper.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/go/whisper_test.go` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/go/whisper_test.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/LICENSE` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Makefile` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Makefile`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Makefile-tmpl` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Makefile-tmpl`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Package.swift` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Package.swift`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/README.md` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Sources/test-objc/main.m` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Sources/test-objc/main.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Sources/test-swift/main.swift` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Sources/test-swift/main.swift`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml.c` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml.c`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml.h` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Sources/whisper/include/whisper.h` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Sources/whisper/include/whisper.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/Sources/whisper/whisper.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/Sources/whisper/whisper.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ios/models/for-tests-ggml-base.en.bin` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ios/models/for-tests-ggml-base.en.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/javascript/CMakeLists.txt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/javascript/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/javascript/README.md` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/javascript/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/javascript/emscripten.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/javascript/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/javascript/libwhisper.worker.js` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/javascript/libwhisper.worker.js`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/javascript/package-tmpl.json` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/javascript/package-tmpl.json`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/javascript/package.json` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/javascript/package.json`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/javascript/whisper.js` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/javascript/whisper.js`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ruby/ext/extconf.rb` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ruby/ext/extconf.rb`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ruby/ext/ruby_whisper.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ruby/ext/ruby_whisper.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/bindings/ruby/tests/test_whisper.rb` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/bindings/ruby/tests/test_whisper.rb`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/cmake/BuildTypes.cmake` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/cmake/BuildTypes.cmake`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/cmake/GitVars.cmake` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/cmake/GitVars.cmake`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/coreml/whisper-decoder-impl.h` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/coreml/whisper-decoder-impl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/coreml/whisper-decoder-impl.m` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/coreml/whisper-decoder-impl.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/coreml/whisper-encoder-impl.h` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/coreml/whisper-encoder-impl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/coreml/whisper-encoder-impl.m` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/coreml/whisper-encoder-impl.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/coreml/whisper-encoder.h` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/coreml/whisper-encoder.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/coreml/whisper-encoder.mm` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/coreml/whisper-encoder.mm`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/CMakeLists.txt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/addon.node/CMakeLists.txt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/addon.node/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/addon.node/README.md` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/addon.node/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/addon.node/__test__/whisper.spec.js` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/addon.node/__test__/whisper.spec.js`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/addon.node/addon.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/addon.node/addon.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/addon.node/index.js` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/addon.node/index.js`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/bench/README.md` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/bench/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/bench/bench.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/bench/bench.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/bench.wasm/CMakeLists.txt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/bench.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/bench.wasm/emscripten.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/bench.wasm/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/bench.wasm/index-tmpl.html` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/bench.wasm/index-tmpl.html`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/command/README.md` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/command/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/command/command.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/command/command.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/command.wasm/CMakeLists.txt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/command.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/command.wasm/README.md` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/command.wasm/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/command.wasm/emscripten.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/command.wasm/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/command.wasm/index-tmpl.html` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/command.wasm/index-tmpl.html`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/common-ggml.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/common-ggml.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/common-sdl.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/common-sdl.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/common-sdl.h` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/common-sdl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/common.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/common.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/common.h` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/common.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/dr_wav.h` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/dr_wav.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/generate-karaoke.sh` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/generate-karaoke.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/helpers.js` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/helpers.js`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/livestream.sh` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/livestream.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/main/README.md` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/main/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/main/main.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/main/main.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/quantize/quantize.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/quantize/quantize.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/stream/README.md` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/stream/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/stream/stream.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/stream/stream.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/stream.wasm/CMakeLists.txt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/stream.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/stream.wasm/emscripten.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/stream.wasm/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/stream.wasm/index-tmpl.html` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/stream.wasm/index-tmpl.html`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk/README.md` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk/eleven-labs.py` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk/eleven-labs.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk/gpt-2.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk/gpt-2.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk/gpt-2.h` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk/gpt-2.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk/speak.sh` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk/speak.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk/talk.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk/talk.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk-llama/CMakeLists.txt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk-llama/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk-llama/README.md` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk-llama/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk-llama/eleven-labs.py` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk-llama/eleven-labs.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk-llama/llama-util.h` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk-llama/llama-util.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk-llama/llama.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk-llama/llama.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk-llama/llama.h` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk-llama/llama.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk-llama/prompts/talk-alpaca.txt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk-llama/prompts/talk-alpaca.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk-llama/speak.sh` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk-llama/speak.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk-llama/talk-llama.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk-llama/talk-llama.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk.wasm/CMakeLists.txt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk.wasm/README.md` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk.wasm/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk.wasm/emscripten.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk.wasm/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk.wasm/gpt-2.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk.wasm/gpt-2.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk.wasm/gpt-2.h` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk.wasm/gpt-2.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/talk.wasm/index-tmpl.html` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/talk.wasm/index-tmpl.html`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/twitch.sh` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/twitch.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/.idea/gradle.xml` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/.idea/gradle.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/README.md` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/build.gradle` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/build.gradle`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/proguard-rules.pro` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/proguard-rules.pro`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/whispercppdemo/ExampleInstrumentedTest.kt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/whispercppdemo/ExampleInstrumentedTest.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/AndroidManifest.xml` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/AndroidManifest.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/MainActivity.kt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/MainActivity.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/media/RiffWaveHelper.kt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/media/RiffWaveHelper.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/recorder/Recorder.kt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/recorder/Recorder.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreen.kt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreen.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreenViewModel.kt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreenViewModel.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Theme.kt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Theme.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Type.kt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Type.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/whisper/LibWhisper.kt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/whisper/LibWhisper.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Android.mk` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Android.mk`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Whisper.mk` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Whisper.mk`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/jni.c` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/jni.c`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_background.xml` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_background.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_foreground.xml` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_foreground.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/xml/data_extraction_rules.xml` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/xml/data_extraction_rules.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.jar` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.jar`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/gradle.properties` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/gradle.properties`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/gradlew` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/gradlew`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.android/gradlew.bat` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.android/gradlew.bat`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.nvim/README.md` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.nvim/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.nvim/whisper.nvim` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.nvim/whisper.nvim`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/README.md` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.m` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/LaunchScreen.storyboard` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/LaunchScreen.storyboard`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/Main.storyboard` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/Main.storyboard`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Info.plist` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Info.plist`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.m` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.h` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.m` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.pbxproj` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/README.md` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/LibWhisper.swift` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/LibWhisper.swift`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Models/WhisperState.swift` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Models/WhisperState.swift`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/UI/ContentView.swift` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/UI/ContentView.swift`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/Recorder.swift` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/Recorder.swift`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.pbxproj` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/xcschemes/WhisperCppDemo.xcscheme` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/xcschemes/WhisperCppDemo.xcscheme`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.wasm/CMakeLists.txt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.wasm/README.md` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.wasm/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.wasm/emscripten.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.wasm/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/whisper.wasm/index-tmpl.html` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/whisper.wasm/index-tmpl.html`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/examples/yt-wsp.sh` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/examples/yt-wsp.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/extra/bench-all.sh` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/extra/bench-all.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/extra/bench-wts.sh` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/extra/bench-wts.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/extra/deploy-wasm.sh` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/extra/deploy-wasm.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/extra/quantize-all.sh` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/extra/quantize-all.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/extra/sync-ggml.sh` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/extra/sync-ggml.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/ggml-cuda.cu` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/ggml-cuda.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/ggml-cuda.h` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/ggml-cuda.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/ggml-opencl.c` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/ggml-opencl.c`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/ggml-opencl.h` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/ggml-opencl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/ggml.c` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/ggml.c`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/ggml.h` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/ggml.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/README.md` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/convert-h5-to-ggml.py` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/convert-h5-to-ggml.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/convert-pt-to-ggml.py` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/convert-pt-to-ggml.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/convert-whisper-to-coreml.py` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/convert-whisper-to-coreml.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/download-coreml-model.sh` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/download-coreml-model.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/download-ggml-model.cmd` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/download-ggml-model.cmd`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/download-ggml-model.sh` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/download-ggml-model.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/for-tests-ggml-base.bin` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/for-tests-ggml-base.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/for-tests-ggml-base.en.bin` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/for-tests-ggml-base.en.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/for-tests-ggml-large.bin` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/for-tests-ggml-large.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/for-tests-ggml-medium.bin` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/for-tests-ggml-medium.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/for-tests-ggml-medium.en.bin` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/for-tests-ggml-medium.en.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/for-tests-ggml-small.bin` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/for-tests-ggml-small.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/for-tests-ggml-small.en.bin` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/for-tests-ggml-small.en.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/for-tests-ggml-tiny.bin` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/for-tests-ggml-tiny.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/for-tests-ggml-tiny.en.bin` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/for-tests-ggml-tiny.en.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/generate-coreml-interface.sh` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/generate-coreml-interface.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/models/generate-coreml-model.sh` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/models/generate-coreml-model.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/samples/jfk.wav` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/samples/jfk.wav`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/tests/CMakeLists.txt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/tests/en-0-ref.txt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/tests/en-0-ref.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/tests/en-1-ref.txt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/tests/en-1-ref.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/tests/en-2-ref.txt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/tests/en-2-ref.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/tests/es-0-ref.txt` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/tests/es-0-ref.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/tests/run-tests.sh` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/tests/run-tests.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/tests/test-whisper.js` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/tests/test-whisper.js`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/whisper.cpp` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/whisper.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/vendor/whisper.cpp/whisper.h` & `whisper_cpp_python-0.2.0/vendor/whisper.cpp/whisper.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/whisper_cpp_python/whisper_cpp.py` & `whisper_cpp_python-0.2.0/whisper_cpp_python/whisper_cpp.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.9/whisper_cpp_python.egg-info/SOURCES.txt` & `whisper_cpp_python-0.2.0/whisper_cpp_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CMakeLists.txt
+LICENSE
 README.md
 pyproject.toml
 setup.py
 tests/test.py
 vendor/pycparser/utils/fake_libc_include/_ansi.h
 vendor/pycparser/utils/fake_libc_include/_fake_defines.h
 vendor/pycparser/utils/fake_libc_include/_fake_typedefs.h
@@ -399,12 +400,16 @@
 vendor/whisper.cpp/tests/en-2-ref.txt
 vendor/whisper.cpp/tests/es-0-ref.txt
 vendor/whisper.cpp/tests/run-tests.sh
 vendor/whisper.cpp/tests/test-whisper.js
 whisper_cpp_python/__init__.py
 whisper_cpp_python/whisper.py
 whisper_cpp_python/whisper_cpp.py
+whisper_cpp_python/whisper_types.py
 whisper_cpp_python.egg-info/PKG-INFO
 whisper_cpp_python.egg-info/SOURCES.txt
 whisper_cpp_python.egg-info/dependency_links.txt
 whisper_cpp_python.egg-info/requires.txt
-whisper_cpp_python.egg-info/top_level.txt
+whisper_cpp_python.egg-info/top_level.txt
+whisper_cpp_python/server/__init__.py
+whisper_cpp_python/server/__main__.py
+whisper_cpp_python/server/app.py
```

