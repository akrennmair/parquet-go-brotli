# parquet-go-brotli

<p align="center">
<a href="https://pkg.go.dev/github.com/akrennmair/parquet-go-brotli"><img src="https://pkg.go.dev/badge/github.com/akrennmair/parquet-go-brotli.svg" alt="Go Reference"></a>
<a href="https://github.com/akrennmair/parquet-go-brotli/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-Apache%202-blue"></a>
</p>

This library implements the Brotli compression algorithms for [github.com/fraugster/parquet-go](github.com/fraugster/parquet-go). By default,
`parquet-go` library only supports `GZIP` and `SNAPPY` as compression algorithms to minimize the list
of dependencies.

All you need to do is import this package into your program and the compression algorithm will be automatically available in `parquet-go`.

```go
import (
    _ "github.com/akrennmair/parquet-go-brotli" // registers the Brotli block compressor with parquet-go
)
```

## License

See the file `LICENSE` for further license information.

## Author

Andreas Krennmair <ak@synflood.at>
