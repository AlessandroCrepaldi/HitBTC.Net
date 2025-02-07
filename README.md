# ![Icon](https://github.com/intelligences/HitBTC.Net/blob/master/src/HitBTC.Net/Icon/icon.png?raw=true) HitBTC.Net

![Build status](https://travis-ci.org/intelligences/HitBTC.Net.svg?branch=master)

HitBTC.Net is a .Net wrapper for the HitBTC API as described on [HitBTC](https://api.hitbtc.com/). It includes all features the API provides using clear and readable C# objects including 
* Reading market info
* Placing and managing orders
* Reading balances

Additionally it adds some convenience features like:
* Access to the websocket, allowing for realtime updates
* Configurable rate limiting
* Autmatic logging

**If you think something is broken, something is missing or have any questions, please open an [Issue](https://github.com/intelligences/HitBTC.Net/issues)**

## CryptoExchange.Net
Implementation is build upon the CryptoExchange.Net library, make sure to also check out the documentation on that: [docs](https://github.com/JKorf/CryptoExchange.Net)

Other CryptoExchange.Net implementations:
<table>
<tr>
<td><a href="https://github.com/JKorf/Bittrex.Net"><img src="https://github.com/JKorf/Bittrex.Net/blob/master/Bittrex.Net/Icon/icon.png?raw=true"></a>
<br />
<a href="https://github.com/JKorf/Bittrex.Net">Bittrex</a>
</td>
<td><a href="https://github.com/JKorf/Bitfinex.Net"><img src="https://github.com/JKorf/Bitfinex.Net/blob/master/Bitfinex.Net/Icon/icon.png?raw=true"></a>
<br />
<a href="https://github.com/JKorf/Bitfinex.Net">Bitfinex</a>
</td>
<td><a href="https://github.com/JKorf/Binance.Net"><img src="https://github.com/JKorf/Binance.Net/blob/master/Binance.Net/Icon/icon.png?raw=true"></a>
<br />
<a href="https://github.com/JKorf/Binance.Net">Binance</a>
</td>
<td><a href="https://github.com/JKorf/CoinEx.Net"><img src="https://github.com/JKorf/CoinEx.Net/blob/master/CoinEx.Net/Icon/icon.png?raw=true"></a>
<br />
<a href="https://github.com/JKorf/CoinEx.Net">CoinEx</a>
</td>
<td><a href="https://github.com/JKorf/Huobi.Net"><img src="https://github.com/JKorf/Huobi.Net/blob/master/Huobi.Net/Icon/icon.png?raw=true"></a>
<br />
<a href="https://github.com/JKorf/Huobi.Net">Huobi</a>
</td>
<td><a href="https://github.com/JKorf/Kucoin.Net"><img src="https://github.com/JKorf/Kucoin.Net/blob/master/Kucoin.Net/Icon/icon.png?raw=true"></a>
<br />
<a href="https://github.com/JKorf/Kucoin.Net">Kucoin</a>
</td>
<td><a href="https://github.com/JKorf/Kraken.Net"><img src="https://github.com/JKorf/Kraken.Net/blob/master/Kraken.Net/Icon/icon.png?raw=true"></a>
<br />
<a href="https://github.com/JKorf/Kraken.Net">Kraken</a>
</td>
</tr>
</table>
Implementations from third parties:
<table>
	<tr>
		<td>
			<a href="https://github.com/Zaliro/Switcheo.Net">
				<img src="https://github.com/Zaliro/Switcheo.Net/blob/master/Resources/switcheo-coin.png?raw=true">
			</a>
			<br />
			<a href="https://github.com/Zaliro/Switcheo.Net">Switcheo</a>
		</td>
		<td>
			<a href="https://github.com/ridicoulous/LiquidQuoine.Net">
				<img src="https://github.com/ridicoulous/LiquidQuoine.Net/blob/master/Resources/icon.png?raw=true">
			</a>
			<br />
			<a href="https://github.com/ridicoulous/LiquidQuoine.Net">Liquid</a>
		</td>
		<td><a href="https://github.com/burakoner/OKEx.Net"><img src="https://raw.githubusercontent.com/burakoner/OKEx.Net/master/Okex.Net/Icon/icon.png"></a>
		<br />
		<a href="https://github.com/burakoner/OKEx.Net">OKEx</a>
		</td>
		</td>
		<td>
			<a href="https://github.com/ridicoulous/Bitmex.Net"><img src="https://github.com/ridicoulous/Bitmex.Net/blob/master/Bitmex.Net/Icon/icon.png"></a>
			<br />
			<a href="https://github.com/ridicoulous/Bitmex.Net">Bitmex</a>
		</td>
		<td>
			<a href="https://github.com/intelligences/HitBTC.Net"><img src="https://github.com/intelligences/HitBTC.Net/blob/master/src/HitBTC.Net/Icon/icon.png"></a>
			<br />
			<a href="https://github.com/intelligences/HitBTC.Net">HitBTC</a>
		</td>
	<td><a href="https://github.com/d-ugarov/Exante.Net"><img src="https://github.com/d-ugarov/Exante.Net/blob/master/Exante.Net/Icon/icon.png?raw=true"></a>
<br />
<a href="https://github.com/d-ugarov/Exante.Net">Exante</a>
</td>
	</tr>
	
</table>

## Installation
![Nuget version](https://img.shields.io/nuget/v/hitbtc_net.svg) ![Nuget downloads](https://img.shields.io/nuget/dt/HitBTC_Net.svg)

Available on [NuGet](https://www.nuget.org/packages/HitBTC.Net/):
```
PM> Install-Package HitBTC_Net
```
To get started with HitBTC_Net first you will need to get the library itself. The easiest way to do this is to install the package into your project using  [NuGet](https://www.nuget.org/packages/HitBTC_Net/). Using Visual Studio this can be done in two ways.

### Using the package manager
In Visual Studio right click on your solution and select 'Manage NuGet Packages for solution...'. A screen will appear which initially shows the currently installed packages. In the top bit select 'Browse'. This will let you download net package from the NuGet server. In the search box type 'HitBTC_Net' and hit enter. The HitBTC_Net package should come up in the results. After selecting the package you can then on the right hand side select in which projects in your solution the package should install. After you've selected all project you wish to install and use HitBTC_Net in hit 'Install' and the package will be downloaded and added to you projects.

### Using the package manager console
In Visual Studio in the top menu select 'Tools' -> 'NuGet Package Manager' -> 'Package Manager Console'. This should open up a command line interface. On top of the interface there is a dropdown menu where you can select the Default Project. This is the project that HitBTC_Net will be installed in. After selecting the correct project type  `Install-Package HitBTC_Net`  in the command line interface. This should install the latest version of the package in your project.

After doing either of above steps you should now be ready to actually start using HitBTC_Net.

## Getting started
To get started we have to add the HitBTC.Net namespace:  `using HitBTC.Net;`.

## Release notes
* Version 1.0.1.4 - 17 july 2020
	* Release version 1.0.1.4
	
## Examples
### Socket

```
var socketApi = new HitBTCSocketClient();
Console.WriteLine("Waiting...");

socketApi.SubscribeOrderBook("BTCUSD", (o) => { Console.WriteLine($"{o.Timestamp.ToShortTimeString()} > {o.Ask.First().Price} | {o.Bid.First().Price}"); });

while (Console.Read() == -1) ;

await socketApi.UnsubscribeAllAsync();
```
