# Final project.
## Project_11. E-Commerce: Product Range Analysis.

**Task:**

**Analyze the store's product range.**

- Carry out exploratory data analysis
- Analyze the product range
- Formulate and test statistical hypotheses

### Data description
The dataset contains the transaction history of an online store that sells household goods.

The file `ecommerce_dataset_us.csv` contains the following columns:

`InvoiceNo` — order identifier

`StockCode` — item identifier

`Description` — item name

`Quantity`

`InvoiceDate` — order date

`UnitPrice` — price per item


**Dashboards:** https://public.tableau.com/app/profile/olga6173/viz/ProductRangeAnalysis/Dashboard1?publish=yes 
<br>
**Presentation:** https://disk.yandex.ru/i/bi2aa6rBmrCK1Q


# Project description
# SQL

The coronavirus took the entire world by surprise, changing everyone's daily routine. City dwellers no longer spent their free time outside, going to cafes and malls; more people were at home, reading books. That attracted the attention of startups that rushed to develop new apps for book lovers. 

You've been given a database of one of the services competing in this market. It contains data on books, publishers, authors, and customer ratings and reviews of books. This information will be used to generate a value proposition for a new product. 
![SQL tables](https://user-images.githubusercontent.com/99878046/169647358-b3247a9f-6169-4d94-aa5c-0dbe1a730258.png)

# Project description
## A/B Testing

### Task statement

You've received an analytical task from an international online store. Your predecessor failed to complete it: they launched an A/B test and then quit (to start a watermelon farm in Brazil). They left only the technical specifications and the test results. 

### Technical description

- Test name: `recommender_system_test`
- Groups: А (control), B (new payment funnel)
- Launch date: 2020-12-07
- The date when they stopped taking up new users: 2020-12-21
- End date: 2021-01-01
- Audience: 15% of the new users from the EU region
- Purpose of the test: testing changes related to the introduction of an improved recommendation system
- Expected result: within 14 days of signing up, users will show better conversion into product page views (the `product_page` event), product card views (`product_card`) and purchases (`purchase`). At each of the stage of the funnel `product_page → product_card → purchase`, there will be at least a 10% increase.
- Expected number of test participants: 6000

# Data description
- `ab_project_marketing_events_us.csv` — the calendar of marketing events for 2020
- `final_ab_new_users_upd.csv` — all users who signed up in the online store from December 7 to 21, 2020
- `final_ab_events_upd.csv` — all events of the new users within the period from December 7, 2020 to January 1, 2021
- `final_ab_participants_upd.csv` — table containing test participants

Structure of `ab_project_marketing_events_us.csv`:

- `name` — the name of the marketing event
- `regions` — regions where the ad campaign will be held
- `start_dt` — campaign start date
- `finish_dt` — campaign end date

Structure of `final_ab_new_users_upd.csv`:

- `user_id`
- `first_date` — sign-up date
- `region`
- `device` — device used to sign up

Structure of `final_ab_events_upd.csv`:

- `user_id`
- `event_dt` — event date and time
- `event_name` — event type name
- `details` — additional data on the event (for instance, the order total in USD for `purchase` events)

Structure of `final_ab_participants_upd.csv`:

- `user_id`
- `ab_test` — test name
- `group` — the test group the user belonged to

