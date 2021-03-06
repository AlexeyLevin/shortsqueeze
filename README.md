![GitHub Workflow Status](https://img.shields.io/github/workflow/status/samgozman/shortsqueeze/Shortsqueeze%20Node.js) 
[![npm](https://img.shields.io/npm/v/shortsqueeze)](https://www.npmjs.com/package/shortsqueeze)
![npm bundle size](https://img.shields.io/bundlephobia/min/shortsqueeze)
![NPM](https://img.shields.io/npm/l/shortsqueeze)

# shortsqueeze

Get detailed short stocks data from shortsqueeze.com

> *Warning! This is unofficial API.*

> 💎🙌 to the moon 🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀

## Installation
Install package from NPM

```
npm install shortsqueeze
```

## Features
Get free stock shorts data from shortsqueeze.com such as: 

* Short intrest days to cover
* Short percent float
* Short % Increase / Decrease
* Short interest shares short
* Trading volume today vs Avg
* Market cap
* Current price (20 min delay)
* **AND MANY OTHERS**

## Usage
Use **shortsqueeze** in async functions

```javascript
const shortsqueeze = require('shortsqueeze')

const main = async () => {
	const stock = await shortsqueeze('SPCE')
	console.log(stock)
}

main()
```
### Returns
> await shortsqueeze('SPCE')

```javascript
{
  shortInterestRatioDaysToCover: 1.1,
  shortPercentOfFloat: 10.12,
  shortPercentIncreaseDecrease: -45,
  shortInterestCurrentSharesShort: 21130000,
  sharesFloat: 208790000,
  shortInterestPriorSharesShort: 38600000,
  percentFrom52WkHigh: -5.4,
  percentFrom50DayMa: 74.66,
  percentFrom200DayMa: 162.11,
  percentFrom52WkLow: 555.74,
  n52WeekPerformance: 148.91,
  tradingVolumeTodayVsAvg: 108.18,
  tradingVolumeToday: 21387935,
  tradingVolumeAverage: 19770000,
  marketCap: null,
  percentOwnedByInsiders: 40,
  percentOwnedByInstitutions: 29.72,
  price: 54.53,
  name: 'Virgin Galactic Holdings Inc',
  ticker: 'SPCE'
}
```
