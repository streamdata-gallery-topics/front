swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite VWAP
  description: provides-delayed-and-historical-volumeweightedaverage-price-vwap-information-
  version: 1.0.0
host: www.xignite.com
basePath: xVWAP.json/XigniteVWAP
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ListFrontMonthContracts:
    get:
      summary: List Front Month Contracts
      description: List all commodity future Front Month Contracts.
      operationId: postListfrontmonthcontracts
      x-api-path-slug: listfrontmonthcontracts-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Front
      - Month
      - Contracts
  /GetDelayedFrontFuture:
    get:
      summary: Get Delayed Front Future
      description: Returns a delayed quote for a future contract.
      operationId: postGetdelayedfrontfuture
      x-api-path-slug: getdelayedfrontfuture-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Delayed
      - Front
      - Future
  /GetFrontMonthFuture:
    get:
      summary: Get Front Month Future
      description: Returns master data on the front month future contract
      operationId: GetFrontMonthFuture
      x-api-path-slug: getfrontmonthfuture-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Front
      - Month
      - Future
  /GetLatestFrontMonthFutureQuotes:
    get:
      summary: Get Latest Front Month Future Quotes
      description: Returns latest quotes for front month futures
      operationId: GetLatestFrontMonthFutureQuotes
      x-api-path-slug: getlatestfrontmonthfuturequotes-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Latest
      - Front
      - Month
      - Future
      - Quotes