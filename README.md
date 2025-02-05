# Module-2-Workflow-Orchestration


### Q1. Within the execution for Yellow Taxi data for the year 2020 and month 12: what is the uncompressed file size (i.e. the output file yellow_tripdata_2020-12.csv of the extract task)?
Answer: 128.3 MB
### Q2. What is the rendered value of the variable file when the inputs taxi is set to green, year is set to 2020, and month is set to 04 during execution?
Answer: green_tripdata_2020-04.csv
### Q3. How many rows are there for the Yellow Taxi data for all CSV files in the year 2020?
Answer: 24648499
    SELECT COUNT(*) AS count
    FROM public.yellow_tripdata
    WHERE filename LIKE 'yellow_tripdata_2020-%.csv'
### Q4. How many rows are there for the Green Taxi data for all CSV files in the year 2020?
Answer:1734051
    SELECT COUNT(*) AS count
    FROM public.green_tripdata
    WHERE filename LIKE 'green_tripdata_2020-%.csv'
### Q5. How many rows are there for the Yellow Taxi data for the March 2021 CSV file?
Answer: 1925152
    SELECT COUNT(*) AS count
    FROM public.yellow_tripdata
    WHERE filename = 'yellow_tripdata_2021-03.csv'
### Q6. How would you configure the timezone to New York in a Schedule trigger?
Answer: Add a timezone property set to America/New_York in the Schedule trigger configuration
