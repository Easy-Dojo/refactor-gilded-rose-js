# Gilded Rose

This is the Gilded Rose kata in JavaScript with Jest

## Getting started

Install dependencies

```sh
npm install
```

## Running tests

To run all tests

```sh
npm test
```

To run all tests in watch mode

```sh
npm run test:watch
```

To generate test coverage report

```sh
npm run test:coverage
```


## 需求描述
“镶金玫瑰”!这是一家魔兽世界里的小商店。出售的商品也都是高质量的。但不妙的是，随着商品 逐渐接近保质期，它们的质量也不断下滑。现邀请你开发一个IT系统，从而能够在每过去一天后， 对商店中商品的信息做出对应的更新。

### 首先，简单介绍一下我们的系统:
- 所有商品都有一个SellIn值，这是商品距离过期的天数，最好在这么多天之内卖掉
- 所有商品都有一个Quality值，代表商品的价值
- 商品的SellIn值和Quality值，它们每天会发生变化，但是会有特例

### 商品的价格规则说明如下:
- 商品每过一天价值会下滑1点 ，一旦过了保质期，价值就以双倍的速度下滑
- 商品的价值永远不会小于0，也永远不会超过50
- 陈年干酪(Aged Brie)是一种特殊的商品，放得越久，价值反而越高
- 萨弗拉斯(Sulfuras)是一种传奇商品，没有保质期的概念，质量也不会下滑
    - 后台门票(Backstage pass)和陈年干酪(Aged Brie)有相似之处:
    - 越接近演出日，商品价值Quality值反而上升 - 在演出前10天，价值每天上升2点
    - 演出前5天，价值每天上升3点
    - 一旦过了演出日，价值就马上变成0

## 要求
1. 不更改测试，不可破坏测试
2. 小步提交，Commit信息要表意
3. 每次Commit前保持测试是通过的