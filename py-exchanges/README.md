Functionality of an exchange implementation
- connect to the appropriate api endpoint
- subscribe to the appropriate channels
- receive the data
- parse the data to the common template

Common data template:
* Orderbooks:
  - rec_tmstmp - timestamp marked when the data reached the host
  - exchange
  - base
  - quote
  - ex_tmstmp - timestamp received in exchange's message
  - bids - array of bid prices sorted from the best to the worst
  - bids_vol - array of bid volumes accordingly to the prices in bids array
  - asks - array of ask prices sorted from the best to the worst
  - asks_vol - array of ask volumes accordingly to the prices in asks array

* Tops:
  - rec_tmstmp - timestamp marked when the data reached the host
  - exchange
  - base
  - quote
  - ex_tmstmp - timestamp received in exchange's message
  - bid - best bid price
  - bid_vol - best bid volume
  - ask - best ask price
  - ask_vol - best ask volume

* Trades:
  - rec_tmstmp - timestamp marked when the data reached the host
  - exchange
  - base
  - quote
  - ex_tmstmp - timestamp received in exchange's message
  - price - price of the trade
  - vol - volume of the trade
  - side - false for buy, true for sell
