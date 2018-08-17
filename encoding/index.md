
[TOC]

API文档地址：godoc.org/github.com/johng-cn/gf/g/encoding

>[danger] # gbase64

BASE64编码解析。

使用方式：
```go
import "gitee.com/johng/gf/g/encoding/gbase64"
```
方法列表：
```go
func Decode(str string) (string, error)
func Encode(str string) string
```

>[danger] # gcompress

二进制数据压缩/解压，支持Zlib/GZip算法。

使用方式：
```go
import "gitee.com/johng/gf/g/encoding/gcompress"
```
方法列表：
```go
func Gzip(data []byte) []byte
func UnGzip(data []byte) []byte
func UnZlib(data []byte) []byte
func Zlib(data []byte) []byte
```




>[danger] # ghash

常用经典哈希函数，提供uint32及uint64类型的哈希函数。

使用方式：
```go
import "gitee.com/johng/gf/g/encoding/ghash"
```
方法列表：
```go
func APHash(str []byte) uint32
func APHash64(str []byte) uint64
func BKDRHash(str []byte) uint32
func BKDRHash64(str []byte) uint64
func DJBHash(str []byte) uint32
func DJBHash64(str []byte) uint64
func ELFHash(str []byte) uint32
func ELFHash64(str []byte) uint64
func JSHash(str []byte) uint32
func JSHash64(str []byte) uint64
func PJWHash(str []byte) uint32
func PJWHash64(str []byte) uint64
func RSHash(str []byte) uint32
func RSHash64(str []byte) uint64
func SDBMHash(str []byte) uint32
func SDBMHash64(str []byte) uint64
```

>[danger] # ghtml

HTML编码解析。

使用方式：
```go
import "gitee.com/johng/gf/g/encoding/ghtml"
```
方法列表：
```go
func SpecialChars(s string) string
func SpecialCharsDecode(s string) string
```





>[danger] # gurl

URL编码解析。

使用方式：
```go
import "gitee.com/johng/gf/g/encoding/gurl"
```
方法列表：
```go
func Decode(str string) (string, error)
func Encode(str string) string
```

>[danger] # gxml

XML数据格式编码解析。

使用方式：
```go
import "gitee.com/johng/gf/g/encoding/gxml"
```
方法列表：
```go
func Decode(xmlbyte []byte) (map[string]interface{}, error)
func Encode(v map[string]interface{}, rootTag ...string) ([]byte, error)
func EncodeWithIndent(v map[string]interface{}, rootTag ...string) ([]byte, error)
func ToJson(xmlbyte []byte) ([]byte, error)
```

>[danger] # gyaml

YAML数据格式编码解析。

使用方式：
```go
import "gitee.com/johng/gf/g/encoding/gyaml"
```
方法列表：
```go
func Decode(v []byte) (interface{}, error)
func DecodeTo(v []byte, result interface{}) error
func Encode(v interface{}) ([]byte, error)
func ToJson(v []byte) ([]byte, error)
```

>[danger] # gtoml

TOML数据格式编码解析。

使用方式：
```go
import "gitee.com/johng/gf/g/encoding/gtoml"
```
方法列表：
```go
func Decode(v []byte) (interface{}, error)
func DecodeTo(v []byte, result interface{}) error
func Encode(v interface{}) ([]byte, error)
func ToJson(v []byte) ([]byte, error)
```























