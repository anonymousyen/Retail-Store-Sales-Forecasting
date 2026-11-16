# Data

The raw dataset is the **Rossmann Store Sales** dataset originally hosted on Kaggle.

> Download link: https://www.kaggle.com/competitions/rossmann-store-sales/data

## Files expected here

| File | Description |
|------|-------------|
| `train.csv` | Historical sales data (1 017 209 rows × 18 columns) |
| `test.csv` | Holdout set used for Kaggle submission |
| `store.csv` | Supplemental store metadata |
| `sample_submission.csv` | Kaggle submission template |

> [!IMPORTANT]
> These files are excluded from version control via `.gitignore` because of their size.  
> Place them in this folder before running any notebook.

## Column reference (`train.csv`)

| Column | Type | Description |
|--------|------|-------------|
| `Store` | int | Unique store ID (1 – 1 115) |
| `DayOfWeek` | int | 1 = Monday … 7 = Sunday |
| `Date` | date | Transaction date |
| `Sales` | int | Daily turnover (target) |
| `Customers` | int | Number of customers that day |
| `Open` | int | 0 = closed, 1 = open |
| `Promo` | int | 1 if the store is running a promo |
| `StateHoliday` | str | `0` = none, `a` = public, `b` = Easter, `c` = Christmas |
| `SchoolHoliday` | int | 1 if public schools are closed |
| `StoreType` | str | Store model: `a`, `b`, `c`, `d` |
| `Assortment` | str | Assortment level: `a` = basic, `b` = extra, `c` = extended |
| `CompetitionDistance` | float | Distance (m) to nearest competitor |
| `CompetitionOpenSinceMonth` | float | Month nearest competitor opened |
| `CompetitionOpenSinceYear` | float | Year nearest competitor opened |
| `Promo2` | int | 1 if the store participates in a recurring promo |
| `Promo2SinceWeek` | float | Week Promo2 started |
| `Promo2SinceYear` | float | Year Promo2 started |
| `PromoInterval` | str | Months Promo2 restarts (e.g. `Jan,Apr,Jul,Oct`) |
