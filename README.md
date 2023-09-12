golog
=====

Severity-based key/value logging replacement for Go's standard logger.

Outputs a message, along with a set key/value pairs for easy parsing.

Example:

```go
// import "github.com/adsbynimbus/golog/log"

log.Error("MyLibrary", "Could not connect to server.", "url", url, "error", err.Error())
log.Info("MyLibrary", "Something happened.")
```

Would output something like:

```
ERROR | MyLibrary | Could not connect to server. | url='http://adsbynimbus.com/' error='timed out'
INFO  | MyLibrary | Something happened.
```

## License

MIT
