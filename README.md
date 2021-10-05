## tokenaddressio_api_document

####  service:   Universal token address generator

##### update:  Util September 2021, tokenaddress.io has created a total of 17.6 million wallets

#### website:   https://tokenaddress.io

#### twitter:   https://twitter.com/tokenaddressio

#### supported token list: BTC、ETH、TRX、LTC、ETC、BCH、BSC、HECO、OKT、USDT(ERC20、TRC20、OMNI)、MATIC、DOGE、BNB、EOS、NEO、BSV、VET、ATOM、XLM、WAVES、XRP、ONT

# API interface request frequency rate limit：
  2 times/second And 1000 times/day ,No authentication required.
  
## request domain
  https://tokenaddress.io
  
## Generate Token Address And Private Key

  GET    /create/< token>


  token options : btc、eth、trx、ltc、etc、bch、bsc、heco、okt、usdt_erc20、usdt_trc20、usdt_omni、matic、doge、bnb、eos、neo、bsv、vet、atom、xlm、waves、xrp、ont

  # request Example
  GET https://www.tokenaddress.io/create/btc

## Return Parameters
    ParameterName         ParameterType	  Description
    state                 String	    state value: success 、error
    code                  String      state code
    symbol                String	    symbol
    addr                  String	    wallet address
    privateKey            String	    wallet private key

## state code
    code      description
    1000      success
    1001      request exceed limit
    1002      symbol not supported
    1003      service internal error
    1004      ip blocked
 
### Donations
    BTC Address: 15AEAHyMjFGqKvSgsbmUBD1M7xVXJaBsHz
    ETH Address: 0x3d61db050fc4810c64012ac260dc9c73b902f641
    DOGE Address: D8BAJrtK4W3jZ8XNQAyjxiEQgogCbboyZb

  
