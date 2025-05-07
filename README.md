Compiling Command:

```
make install -j PROG_SUFFIX=-prof REDIS_LDFLAGS=-no-pie
```

* `PROG_SUFFIX=-prof`: Prevents conflicts with the original redis-server by appending a suffix.
* `REDIS_LDFLAGS=-no-pie`: Disables position-independent executable (PIE) to enable call stack capturing.