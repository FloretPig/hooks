# @midwayjs/hooks-request

> [中文文档](./README.zh-cn.md)

Midway Hooks Front End Request SDK

## Usage

```typescript
import { request } from '@midwayjs/hooks/request'

function fetch(...args) {
  return request({
    url: '/api',
    method: 'GET',
    data: {
      args: args,
    },
    meta: {
      functionName: 'lambda-index',
      gateway: 'http',
      functionGroup: 'midway-faas-react-demo',
    },
  })
}

const response = await fetch()
console.log(response)
```
