---
title: Tilt CLI Reference
layout: docs
hideEditButton: true
---
## tilt dump logstore

dump the log store

### Synopsis

Dumps the state of the Tilt log store to stdout.

Every log of a Tilt-managed resource is aggregated into a central structured log
store before display. Dumps the JSON representation of this store.

The format of the dump state does not make any API or compatibility promises,
and may change frequently.


```
tilt dump logstore [flags]
```

### Options

```
  -h, --help       help for logstore
      --port int   Port for the Tilt HTTP server (default 10350)
```

### Options inherited from parent commands

```
  -d, --debug                          Enable debug logging
      --klog int                       Enable Kubernetes API logging. Uses klog v-levels (0-4 are debug logs, 5-9 are tracing logs)
      --log-flush-frequency duration   Maximum number of seconds between log flushes (default 5s)
      --trace                          Enable tracing
      --traceBackend string            Which tracing backend to use. Valid values are: 'windmill', 'lightstep', 'jaeger' (default "windmill")
  -v, --verbose                        Enable verbose logging
```

### SEE ALSO

* [tilt dump](tilt_dump.html)	 - Dump internal Tilt state

###### Auto generated by spf13/cobra on 10-Mar-2020