# LogUp

### Input

```golang
type Input interface {
    Start() error
    Stop()
}
```

### Queue

```golang
type LogMessage struct {
    RawData   []byte // Dữ liệu gốc nhận được
    Type      string
    Dataset   string
    Namespace string
    Timestamp time.Time // Thời điểm nhận được log
}
```

