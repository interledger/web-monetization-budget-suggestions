# Web Monetization Budget Suggestions

This repository contains recommended budget for Web Monetization in various currencies.

For each currency, we have a suggested monthly budget and hourly rate of pay.
Each amount has a _`default`_ value which is what we may show to users.
There is also a _`max`_ value where we may warn users to prevent them from overpaying accidentally.

## Motivation

For some time, we've been using a default USD 5 monthly budget for web monetization. However, this doesn't translate well to other currencies.

Simple currency conversion doesn't reflect local purchasing power, which means the value isn't consistent globally. To ensure fairness and relevance, we try to provide a reasonable monthly web monetization budget in different currencies.

Also, a currency conversion requires reliance on an up-to-date exchange rate, which may not be viable for all Web Monetization implementors.

## How this data was generated?

- For the default monthly budget amount, we used an estimated Purchasing Power Parity (PPP) value to get a rough equivalent of 5 USD.
- The values were then made prettier, rounding off to nearer whole numbers.
- For the max monthly budget recommendation, we used the default value and kept it 2-3x amount keeping the values _reasonable_. We also compared direct currency conversion rates to stay within reasonable bounds.
- For the hourly rate of pay, we followed similar approach, but divided the default value by approximately 8. The number 8 comes from the default USD budget settings ($5 monthly budget, $0.60 hourly rate). Then values were modified to keep them prettier.

We also used an [active survey](https://forms.gle/VMNe1uDNHD6ngEYo6) to help us improve the data based on real-user responses.

## How will this data be updated?

The provided data is based on estimations and should be considered preliminary.

We encourage you to submit a pull request or initiate a discussion if you identify any inaccuracies, outdated or missing information. Please include detailed reasoning and supporting evidence for any proposed revisions.

There aren't any automated processes to update the data as of now, so we hope to get valuable feedback from the community.

## Data

The [data.json](v1/data.json) contains the data that you may use. This file is sorted alphabetically by the currency code.

There's also a [JSON Schema](v1/schema.json) to keep data structure consistent and serve as a documentation for the file structure.
