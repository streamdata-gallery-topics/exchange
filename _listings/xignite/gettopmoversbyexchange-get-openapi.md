---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Historical Get Top Movers By Exchange
  description: This operation returns quote information about the top moving equities
    from NYSE, NASDAQ and AMEX.
  version: 1.0.0
host: www.xignite.com
basePath: xHistorical.json/XigniteHistorical
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ListFuturesByExchange:
    get:
      summary: List Futures By Exchange
      description: List futures information by exchange.
      operationId: postListfuturesbyexchange
      x-api-path-slug: listfuturesbyexchange-get
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
      - Futures
      - By
      - Exchange
  /ListSwapsByExchange:
    get:
      summary: List Swaps By Exchange
      description: List swaps information by exchange.
      operationId: postListswapsbyexchange
      x-api-path-slug: listswapsbyexchange-get
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
      - Swaps
      - By
      - Exchange
  /GetTopMoversByExchange:
    get:
      summary: Get Top Movers By Exchange
      description: This operation returns quote information about the top moving equities
        from NYSE, NASDAQ and AMEX.
      operationId: postGettopmoversbyexchange
      x-api-path-slug: gettopmoversbyexchange-get
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
      - Top
      - Movers
      - Exchange
  /GetTopGainersByExchange:
    get:
      summary: Get Top Gainers By Exchange
      description: This operation returns quote information about the top gaining
        equities for the requested exchange.
      operationId: postGettopgainersbyexchange
      x-api-path-slug: gettopgainersbyexchange-get
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
      - Top
      - Gainers
      - By
      - Exchange
  /GetTopLosersByExchange:
    get:
      summary: Get Top Losers By Exchange
      description: This operation returns quote information about the top losing equities
        for the requested exchange.
      operationId: postGettoplosersbyexchange
      x-api-path-slug: gettoplosersbyexchange-get
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
      - Top
      - Losers
      - By
      - Exchange
  /GetAllSplitsByExchange:
    get:
      summary: Get All Splits By Exchange
      description: Get all splits for a date range in the specified exchange.
      operationId: postGetallsplitsbyexchange
      x-api-path-slug: getallsplitsbyexchange-get
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
      - Splits
      - By
      - Exchange
  /GetAllCashDividendsByExchange:
    get:
      summary: Get All Cash Dividends By Exchange
      description: Get all cash dividends for a date range in the specified exchange.
      operationId: postGetallcashdivendsbyexchange
      x-api-path-slug: getallcashdividendsbyexchange-get
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
      - Cash
      - Dividends
      - By
      - Exchange
  /GetAllCorporateActionsByExchange:
    get:
      summary: Get All Corporate Actions By Exchange
      description: Get all corporate actions for a date range in the specified exchange.
      operationId: postGetallcorporateactionsbyexchange
      x-api-path-slug: getallcorporateactionsbyexchange-get
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
      - Corporate
      - Actions
      - By
      - Exchange
  /GetExchangeDateTime:
    get:
      summary: Get Exchange Date Time
      description: Get exchange date time.
      operationId: GetExchangeDateTime
      x-api-path-slug: getexchangedatetime-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Exchange
      - Date
      - Time
  /GetExchangeHours:
    get:
      summary: Get Exchange Hours
      description: Get exchange hours.
      operationId: GetExchangeHours
      x-api-path-slug: getexchangehours-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Exchange
      - Hours
  /GetExchangeHoursRange:
    get:
      summary: Get Exchange Hours Range
      description: Get exchange hours range.
      operationId: GetExchangeHoursRange
      x-api-path-slug: getexchangehoursrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Exchange
      - Hours
      - Range
  /IsExchangeOpenOnDate:
    get:
      summary: Is Exchange Open On Date
      description: Is exchange open on date.
      operationId: IsExchangeOpenOnDate
      x-api-path-slug: isexchangeopenondate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Exchange
      - Open
      - "On"
      - Date
  /AreExchangesOpen:
    get:
      summary: Are Exchanges Open
      description: Are exchanges open.
      operationId: AreExchangesOpen
      x-api-path-slug: areexchangesopen-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Are
      - Exchanges
      - Open
  /GetMasterByExchange:
    get:
      summary: Get Master By Exchange
      description: Get master records by exchange.
      operationId: GetMasterByExchange
      x-api-path-slug: getmasterbyexchange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Exchange
  /GetMasterByExchangeChanges:
    get:
      summary: Get Master By Exchange Changes
      description: Get a master record by exchange and the last modified since date
      operationId: GetMasterByExchangeChanges
      x-api-path-slug: getmasterbyexchangechanges-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Exchange
      - Changes
  /ListMICToLegacyExchange:
    get:
      summary: List MIC To Legacy Exchange
      description: Get the legacy exchanges.
      operationId: ListMICToLegacyExchange
      x-api-path-slug: listmictolegacyexchange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - MIC
      - Legacy
      - Exchange
  /ListIdentifiersByExchange:
    get:
      summary: List Identifiers By Exchange
      description: Returns all the Indetifiers and names for securities listed on
        an exchange.
      operationId: ListIdentifiersByExchange
      x-api-path-slug: listidentifiersbyexchange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - Identifiers
      - Exchange
  /GetMasterStatisticsByExchange:
    get:
      summary: Get Master Statistics By Exchange
      description: Get statistical information about exchanges.
      operationId: GetMasterStatisticsByExchange
      x-api-path-slug: getmasterstatisticsbyexchange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Statistics
      - Exchange
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---