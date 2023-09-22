# Binance Order List
**An application to retrieve a list of all orders executed on a [Binance](https://www.binance.com) account and export them to an Excel spreadsheet.**

By configuring the API Key for a Binance account, you can obtain a comprehensive list of all account orders, including active, canceled, or filled orders. This can be done for a single trading pair (symbol) or a group of trading pairs, with the option to refine the search by date, order status, or order side.

## Dependencies
- [Binance.Net](https://github.com/JKorf/Binance.Net)
- [ClosedXML](https://github.com/ClosedXML/ClosedXML)

## Configuration
To get started, create a [Binance API Key](https://www.binance.com/en/support/faq/360002502072) with read-only permissions. Follow these steps:
- Enter the generated Binance `API Key` and `Secret Key` in the respective text boxes.
- Optionally, you can save the entered credentials for future use by clicking the `Save User` button and assigning it a name. Please note that the Secret Key is stored as plain text, without encryption, so be careful.
- Specify the trading symbol (pair) or a list of symbols (comma-separated) that you wish to search, such as `BTCUSDT` or `ETHUSDT, DOGEEUR, ADABTC, LTCETH`.
- **Options:**
  - **Start Date:** Set the start date for your search. Orders older than the specified date will be excluded.
  - **End Date:** Set the end date for your search. Orders newer than the specified date will be excluded.
  - **Order Status:** Select the order status you wish to filter by. Choose `All` to retrieve orders from all status types.
  - **Order Side:** Choose the order side you want to filter by. Select `All` to include orders from both sides, `buy` and `sell.`

## Usage
Once the configuration is complete, simply click the `Search` button. If data matching the specified parameters is found, a window containing the data will appear. You can then export this data to an Excel spreadsheet by clicking the `Export to Excel` button.

## Changelog
- **v1.1.2 - 05/06/2021**
  - Bug fixes.

- **v1.1.1 - 01/05/2021**
  - Removed trailing zeros from the `Quantity` if it exceeds 1.

- **v1.1.0 - 25/04/2021**
  - Added an `Update Time` column to the search result grid view, displaying the date and time of the order's last update.
  - Prices are now rounded to two decimal places for USDT, USD, and EUR, or as specified in the `LimitTwoDecimalsCurrencies` constant.
  - For partially filled orders, the percentage filled is now included, along with the filled quantity when exporting to Excel.

<br>

------------
## :heart:Donations
**Donations are always greatly appreciated. Thank you for your support!**

<a href="https://www.buymeacoffee.com/devilquest" target="_blank"><img src="https://i.imgur.com/RHHFQWs.png" alt="Buy Me A Dinosaur"></a>