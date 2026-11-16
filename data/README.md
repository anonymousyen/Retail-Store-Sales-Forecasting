# Data

The dataset used in this project is the **Rossmann Store Sales** dataset from Kaggle.

**Download it here:** https://www.kaggle.com/competitions/rossmann-store-sales/data

Place `train.csv` in this folder before running any notebook. The file is excluded from version control (it's ~70 MB).

## Columns

| Column | Description |
|--------|-------------|
| `Store` | Store ID (1–1115) |
| `DayOfWeek` | 1 = Monday, 7 = Sunday |
| `Date` | Transaction date |
| `Sales` | Daily sales — this is what we're predicting |
| `Customers` | Number of customers that day |
| `Open` | 0 = closed, 1 = open |
| `Promo` | 1 if the store had a promo running |
| `StateHoliday` | `0` none, `a` public holiday, `b` Easter, `c` Christmas |
| `SchoolHoliday` | 1 if schools were closed |
| `StoreType` | Store category: `a`, `b`, `c`, `d` |
| `Assortment` | Product range: `a` basic, `b` extra, `c` extended |
| `CompetitionDistance` | Distance (m) to nearest competitor store |
| `CompetitionOpenSinceMonth` | Month the nearest competitor opened |
| `CompetitionOpenSinceYear` | Year the nearest competitor opened |
| `Promo2` | 1 if the store runs a recurring promotion |
| `Promo2SinceWeek` | Week Promo2 started |
| `Promo2SinceYear` | Year Promo2 started |
| `PromoInterval` | Months Promo2 restarts (e.g. `Jan,Apr,Jul,Oct`) |
