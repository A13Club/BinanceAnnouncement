# Important Updates on Funding Rate Formula and Mark Price Calculation of Futures Contracts (2025-09-18)

This is a general announcement. Products and services referred to here may not be available in your region.

Fellow Binancians,

Binance constantly reviews its product and service offerings to ensure the best user experience for all users. Effective from 2025-09-18 08:01 (UTC), the funding rate formula will be updated as follows:

Before the UpdateAfter the UpdateFunding Rate (F) = Average Premium Index (P) + clamp (interest rate - Premium Index (P), 0.05%, -0.05%)Funding Rate (F) = [Average Premium Index (P) + clamp (interest rate - Premium Index (P), 0.05%, -0.05%)] / (8/N)Where N = Funding Rate Settlement FrequencyExample: PUMPUSDT’s funding rate settlement frequency is every 4 hours. PUMPUSDT’s funding rate formula will be as follows:Funding Rate (F) = [Average Premium Index (P) + clamp (interest rate - Premium Index (P), 0.05%, -0.05%)] / (8/4)= [Average Premium Index (P) + clamp (interest rate - Premium Index (P), 0.05%, -0.05%)] / 2

In addition, effective from 2025-09-18 08:01 (UTC), Binance Futures will make adjustments to mark price calculations by updating the basis of Price 2 from 1-minute basis to 30 seconds basis, with details as follows:

Futures ContractsBefore the AdjustmentAfter the AdjustmentUSDⓈ-M and COIN-M Perpetual ContractsMark Price = Median (Price 1, Price 2, Contract Price) Where Price 2 = Price Index + Moving Average (1-Minute Basis) Note: The Moving Average (1-Minute Basis) is calculated as the average of 60 data points over a 1-minute period.The basis is calculated every second by taking the average of the bid and ask prices and then subtracting the Price Index.Mark Price = Median (Price 1, Price 2, Contract Price) Where Price 2 = Price Index + Moving Average (30 Seconds Basis) Note: The Moving Average (1-Minute Basis) is calculated as the average of 30 data points over a 30 seconds period. The basis is calculated every second by taking the average of the bid and ask prices and then subtracting the Price Index.USDⓈ-M and COIN-M Delivery ContractsMark Price = Price Index + Moving Average (1-Minute Basis)Note: Moving Average (1-Minute Basis) = Moving Average ((Bid1 + Ask1) / 2 - Price Index), calculated each second minute in a 1-minute interval. The basis is calculated every second by taking the average of the bid and ask prices and then subtracting the Price Index.Mark Price = Price Index + Moving Average (1-Minute Basis)Note: Moving Average (1-Minute Basis) = Moving Average ((Bid1 + Ask1) / 2 - Price Index), calculated each second minute in a 30 seconds interval. The basis is calculated every second by taking the average of the bid and ask prices and then subtracting the Price Index.

Notes

Users may visit the Real-Time Funding Rate and Funding Rate History pages to view the latest funding interval and historical funding rates. API users may query USDⓈ-M futures funding rate information via the newly added endpoint: GET /fapi/v1/fundingInfo. There may be discrepancies between this original content in English and any translated versions. Please refer to the original English version for the most accurate information, in case any discrepancies arise.

For More Information:

Introduction to Binance Futures Funding RatesWhat Are Mark Price and Price Index in USDⓈ-Margined FuturesMark Price and Price Index of COIN-Margined Contracts

Thank you for your support!

Binance Team

2025-09-16