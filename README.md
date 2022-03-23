### Differences in Households Ordering Free COVID-19 Tests

Policy makers should understand people’s attitudes towards opt-in nudges to smoothly promote and implement the policies.

While governments across several countries shipped COVID-19 tests to households such as the [UK](https://www.washingtonpost.com/world/2022/01/20/rapid-tests-covid/), only in late January of 2022 did the Biden administration decide to allow households to order 2 free rapid tests. The website was run by the [USPS](https://special.usps.com/testkits) and although it was a very easy-to-use website, it still required someone in each household to opt-in. (Note: as of March of 2022, the government now allows us to complete 2 orders of 2 COVID-tests).

My hypothesis was that the more advantaged population - people with higher incomes - would more readily take advantage of this opt-in intervention because they had more time, better access to internet, and more knowledge about this intervention.

I decided to test whether this hypothesis was true by getting a random sample of 1000 addresses, and completing orders for these households. From a legal standpoint, I could not find anything on the website that prohibited this behavior. From an ethical standpoint, the most harm I could do to someone from this was that someone would go online to order a test, and be confused why it had already been ordered. To minimize this harm, I waited one month from USPS launch to conduct this experiment, with the assumption that most people would have ordered the tests by that point. The benefit of this experiment was direct - households would receive a COVID-19 test that they could use or give to a friend. 

My first experiment was conducted in Portland because I live there, and thus knew about the fantastic database of addresses at [Portland Maps](https://www.portlandmaps.com/). 

To read the code: [click on my Jupyter notebook](https://github.com/jaedowning/covid-tests/blob/main/COVID_Tests.ipynb). This contains all the steps used to prepare the addresses, order the tests, geocode and append Census data, and conduct analyses to test hypotheses. 

This project requires:

- Python
- R
- [Pandas](https://pandas.pydata.org/) for data manipulation
- [GeoPy](https://pandas.pydata.org/) for geocoding
- [Selenium](https://www.selenium.dev/) for ordering the tests using an automated browser
- [TidyCensus](https://cran.r-project.org/web/packages/tidycensus/index.html) for pulling in Census data
