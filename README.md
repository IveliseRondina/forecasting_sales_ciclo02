<h1 align="center"> Rossmann Sales Forcasting </h1>

![images](https://user-images.githubusercontent.com/103456938/221711294-ceb13280-5d48-4e58-9c1f-c93994ee9a93.png)

**PS.:** This project has just educational purposes.

## 1.0 - Bussiness Problems

### 1.1 - About Rossmann
Rossmann is one of Europe's largest drugstore chains, with around 56.200 employees and over 4.000 stores.
The company was founded in 1972 by Dirk Rossmann based in Burgwedel near Hanover in Germany. The product range includes up to 21.700 items and may vary depending on store size and location.

### 1.2 - The bussiness problem
Rossmann's CFO decided to renovate the stores, and to plan how much to spend on each renovation, he asked for a forecast of each store's revenue over the next six weeks. To solve this problem, we will use sales data from recent years.

### 1.3 - About the data
| Atributo | Descrição |
| :----- | :----- |
| ID | an Id that represents a (Store, Date) duple within the test set |
| Store | a unique Id for each store |
| Sales | the turnover for any given day (this is what you are predicting) |
| Customers | the number of customers on a given day |
| Open | an indicator for whether the store was open: 0 = closed, 1 = open |
| State Holiday | indicates a state holiday a = public holiday, b = Easter holiday, c = Christmas, 0 = None |
| School Holiday | indicates if the (Store, Date) was affected by the closure of public schools |
| Store Type | differentiates between 4 different store models: a, b, c, d |
| Assortment | describes an assortment level: a = basic, b = extra, c = extended |
| Competition Distance | distance in meters to the nearest competitor store |
| Competition Open Since [Month/Year] | gives the approximate year and month of the time the nearest competitor was opened |
| Promo | indicates whether a store is running a promo on that day |
| Promo2 | Promo2 is a continuing and consecutive promotion for some stores: 0 = store is not participating, 1 = store is participating |
| Promo2 Since [Year/Week] | describes the year and calendar week when the store started participating in Promo2 |
| Promo Interval | describes the consecutive intervals Promo2 is started, naming the months the promotion is started anew. E.g. "Feb,May,Aug,Nov" means each round starts in February, May, August, November of any given year for that store |

Data source: [Kaggle](https://www.kaggle.com/competitions/rossmann-store-sales/data)
![kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=Kaggle&logoColor=white)

## 2.0 - Business Assumptions
* In the CompetitionDistance column, the NA values have been changed to 200.000 meters, meaning that there is no competitor near.
* For NA values in Competition Open Since[Month/Year], we use the same data as in the Date column.
* In the Promo2Since[Year/Week] column, the NA values were also replaced by the value of the Date column.
* 
