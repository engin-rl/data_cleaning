# data_cleaning
this is an SQL data cleaning project using MySQL
-- steps
-- 1. remove duplicates
-- 2. standardize the data
-- 3. null values or blank values
-- 4. remove any columns and rows that are not necessary

# sample data

| Company        | Location      | Industry       | Total Laid Off | Percentage Laid Off | Date     | Stage      | Country        | Funds Raised (Millions) |
|--------------|-------------|--------------|---------------|------------------|----------|-----------|--------------|----------------------|
| Atlassian    | Sydney      | Other        | 500           | 0.05             | 3/6/2023 | Post-IPO  | Australia     | 210                  |
| SiriusXM     | New York City | Media       | 475           | 0.08             | 3/6/2023 | Post-IPO  | United States | 525                  |
| Alerzo      | Ibadan       | Retail       | 400           | NULL             | 3/6/2023 | Series B  | Nigeria       | 16                   |
| UpGrad       | Mumbai       | Education    | 120           | NULL             | 3/6/2023 | Unknown   | India         | 631                  |
| Loft        | Sao Paulo    | Real Estate  | 340           | 0.15             | 3/3/2023 | Unknown   | Brazil        | 788                  |
| Embark Trucks | SF Bay Area | Transportation | 230         | 0.7              | 3/3/2023 | Post-IPO  | United States | 317                  |
| Lendi       | Sydney       | Real Estate  | 100           | NULL             | 3/3/2023 | Unknown   | Australia     | 59                   |
| UserTesting | SF Bay Area  | Marketing    | 63            | NULL             | 3/3/2023 | Acquired  | United States | 152                  |
| Airbnb      | SF Bay Area  |              | 30            | NULL             | 3/3/2023 | Post-IPO  | United States | 6400                 |



# clean data
| Company         | Location        | Industry    | Total Laid Off | Percentage Laid Off | Date       | Stage     | Country        | Funds Raised (Millions) |
|----------------|----------------|------------|---------------|------------------|------------|-----------|--------------|----------------------|
| Included Health | SF Bay Area     | Healthcare | 0             | 0.06             | 2022-07-25 | Series E  | United States | 272                  |
| &Open         | Dublin          | Marketing  | 9             | 0.09             | 2022-11-17 | Series A  | Ireland        | 35                   |
| #Paid         | Toronto         | Marketing  | 19            | 0.17             | 2023-01-27 | Series B  | Canada         | 21                   |
| 100 Thieves   | Los Angeles     | Consumer   | 12            | NULL             | 2022-07-13 | Series C  | United States | 120                  |
| 10X Genomics  | SF Bay Area     | Healthcare | 100           | 0.08             | 2022-08-04 | Post-IPO  | United States | 242                  |
| 1stdibs       | New York City   | Retail     | 70            | 0.17             | 2020-04-02 | Series D  | United States | 253                  |
| 2TM          | Sao Paulo       | Crypto     | 90            | 0.12             | 2022-06-01 | Unknown   | Brazil        | 250                  |
| 2TM          | Sao Paulo       | Crypto     | 100           | 0.15             | 2022-09-01 | Unknown   | Brazil        | 250                  |
| 2U           | Washington D.C. | Education  | 0             | 0.2              | 2022-07-28 | Post-IPO  | United States | 426                  |

