# Bybit NinjaTrader Adapter

[NinjaTrader](https://www.ninjatrader.com)  is a desktop application which allows trading. It also supports addons to allow third parties integrate their market data into the application.

[Bybit](https://www.bybit.com) [NinjaTrader](https://www.ninjatrader.com) Adapter provides data from Bybit platform. Please note that only live data is provided, it can be used for analyzis and sim trading. Order routing is not supported and is against terms and conditions of [NinjaTrader](https://www.ninjatrader.com).

Source code is **NOT** provided due to NinjaTrader Terms & Conditions. You can download the installer **BybitAdapterInstallerV1_2.msi** using this repository to perform an installation.

## Prerequisites

First you need to download and install [NinjaTrader](https://www.ninjatrader.com). You don't need a paid account or a license to performa data analysis, run strategies or execute sim trades and display indicators. Please download and install NinjaTrader before proceeding further with this manual.

## Adapter Installation

0. Make sure NinjaTrader is NOT running.
1. Download BybitAdapterInstallerV1_2.msi from this repository and run the installer.
2. Start NinjaTrader
3. Go to Connections -> configure

![image](https://user-images.githubusercontent.com/23218905/118494541-e0ca7f80-b6e7-11eb-8263-cb0dafa1bf11.png)

4. Find Bybit in the list and click ADD.

![image](https://user-images.githubusercontent.com/23218905/118495698-102dbc00-b6e9-11eb-9a78-260b8f38f47a.png)

5. After you clicked add the connection will get added to the list of configured connections.

![image](https://user-images.githubusercontent.com/23218905/118496212-88947d00-b6e9-11eb-8022-d10a99da1abf.png)

7. You are free to give it any name you like. Please check that you have the correct version. The connection does not require any credentials. You may choose to connect on start up of NinjaTrader (use the available check box to configure this).
8. Choose an applicable server address to your location.
9. After you click OK the connection will become available in the list of available connections.

![image](https://user-images.githubusercontent.com/23218905/118496351-abbf2c80-b6e9-11eb-8753-26a847e420dd.png)

10. Click on the connection name to connect.
11. You will see a green light in the bottom left hand corner in the NinjaTrader control center after a successfull connection.

![image](https://user-images.githubusercontent.com/23218905/118496601-e3c66f80-b6e9-11eb-8aec-6024d64e53a5.png)


## Updates

1. Updating the adapter requires you to first uninstall the old version. Please view the uninstalling information in this manual and then proceed with the installing steps again.

## Uninstalling

1. Go to Windows Control Panel -> Programs & Features and uninstall BybitAdapter

![image](https://user-images.githubusercontent.com/23218905/118495170-909fed00-b6e8-11eb-963d-f5faa9062acc.png)

## Creating an Instrument List

1. After a connection you should be able to see a list of available symbols insde  **New -> BYBIT CONNECTOR** window. This window is only for reference.

![image](https://user-images.githubusercontent.com/23218905/118496919-33a53680-b6ea-11eb-81a0-fca5850d1bd4.png)

2. To create an instrument list that you can work with go to Tools -> Instrument Lists.
3. In the left hand side of the window click add to create a list with a new name eg. MyBybitList

![image](https://user-images.githubusercontent.com/23218905/118497213-7a932c00-b6ea-11eb-854a-6e1c3212fe11.png)

4. To add an instrument click ADD on the right hand side whilst having the left hand side newly created list name selected. Search for the required symbol. All Bybit symbols will be post fixed with a _BYBIT eg. BTCUSDT_BYBIT

![image](https://user-images.githubusercontent.com/23218905/118497584-d067d400-b6ea-11eb-8d70-3fe9322b6b0d.png)

5. Add the symbol from the search to the list by double clicking it.
6. Now this symbol will become available for you to work with inside your custom instrument list when opening a chart.
7. Don't forget to click OK when leaving the instrument list window!!! You might loose your changes if you don't!
8. To open a chart got to New -> Chart and find the symbol in the list.

![image](https://user-images.githubusercontent.com/23218905/118497980-2b99c680-b6eb-11eb-9fbf-f93670088d13.png)

## Important Notes

- NinjaTrader accepts only min, day and tick data from Bybit. This means that the adapter feeds NinjaTrader with minute data from Bybit API and NinjaTrader builds all intraday bars using 1 min bars. Same is true for weekly, monthly and yearly bars that use dayily feed from Bybit API via the adapter. This means that you can expect quite similar to Bybit trading terminal bar plots for 1 min and 1 day charts but other types of charts can and probably will differ slightly.

- If you experience connection issues, go to your browser and enter the website credentials you are logging in with. Bybit.com , .us or other that you selected in the configuration window. If your browser does not open the page that means Bybit is blocked in your country. In this case you will need a VPN.










