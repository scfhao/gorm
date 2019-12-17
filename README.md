# GORM

The fantastic ORM library for Golang, aims to be developer friendly.

[![go report card](https://goreportcard.com/badge/github.com/jinzhu/gorm "go report card")](https://goreportcard.com/report/github.com/jinzhu/gorm)
[![wercker status](https://app.wercker.com/status/8596cace912c9947dd9c8542ecc8cb8b/s/master "wercker status")](https://app.wercker.com/project/byKey/8596cace912c9947dd9c8542ecc8cb8b)
[![codecov](https://codecov.io/gh/jinzhu/gorm/branch/master/graph/badge.svg)](https://codecov.io/gh/jinzhu/gorm)
[![Join the chat at https://gitter.im/jinzhu/gorm](https://img.shields.io/gitter/room/jinzhu/gorm.svg)](https://gitter.im/jinzhu/gorm?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![Open Collective Backer](https://opencollective.com/gorm/tiers/backer/badge.svg?label=backer&color=brightgreen "Open Collective Backer")](https://opencollective.com/gorm)
[![Open Collective Sponsor](https://opencollective.com/gorm/tiers/sponsor/badge.svg?label=sponsor&color=brightgreen "Open Collective Sponsor")](https://opencollective.com/gorm)
[![MIT license](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)
[![GoDoc](https://godoc.org/github.com/jinzhu/gorm?status.svg)](https://godoc.org/github.com/jinzhu/gorm)

## Overview

参考[此博客](https://www.jianshu.com/p/d65aafd66852)增加的对 Oracle 数据库的支持。版本号与原版将保持一致。如未用到 Oracle 数据库，请使用原版。

建立此仓库旨在维护 dialect_oracle.go 文件，此文件来自上述博客。

## 使用方法

```Go
import (
	_ "github.com/mattn/go-oci8"
	_ "github.com/scfhao/gorm/dialects/oci8"
	"github.com/scfhao/gorm"
)

// if use SID, "username/password@tnsname"
db, err := gorm.Open("oci8", "username/password@127.0.0.1:1521/ServiceName")
```

## License

© Jinzhu, 2013~time.Now

Released under the [MIT License](https://github.com/jinzhu/gorm/blob/master/License)
