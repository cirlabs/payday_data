# payday_data
Exported salaries from Payday, the now-deprecated salary app from California Watch/Reveal/The Center for Investigative Reporting

The California State Controller’s Office has collected and published compensation data on as many as 700,000 city and county employees annually from 2009 through 2013. The Center for Investigative Reporting built Payday California to provide additional information and more context for public employee pay.  

For calendar years 2008 through 2012, Payday California also includes additional employee compensation records that CIR requested from the 10 most populous counties and 10 most populous cities in California. The state controller’s data currently includes 2009 through 2013; as of late April 2015, its 2013 data is missing Yuba County and the cities of Glendale and Solana Beach.  

The data we obtained from cities and counties differs from the state’s in two additional ways: 1) We include employees’ names; the State Controller's Office does not. 2) We asked for employees’ gross pay prior to deductions.The State Controller’s Office requests employees’ total wages subject to Medicare taxes, which tend to be lower than gross wages.  

Other differences, such as the number of employees or the amount of pay, could be due to errors or different reporting methods.

### How we obtained the data

Most cities and counties provided the data to CIR for free. Some said they would provide data only by charging programming fees. CIR negotiated these charges whenever possible and paid nominal fees when they were legally supported and appeared to be reasonable. We declined to pay programming fees for some records from Orange County, the city of San Diego and the city of Long Beach because they seemed excessive, leaving those data sets incomplete. In total, CIR paid about $4,800 for records.  

If cities and counties could not provide the data as requested for free or for nominal fees, CIR accepted records in the format they were submitted to the State Controller’s Office with the addition of employee names. Because of these variations, only the state controller’s records can be used to compare communities and years.

### Copyright and license

This repository and the included data are licensed under the Open Database License (ODbL) by Reveal from The Center for Investigative Reporting.

You are free to copy, distribute, transmit and adapt the spreadsheet, so long as you:

- Do not change the data in any way that introduces errors
- Credit Reveal as specified below, including linking back to Reveal as specified below.
- Inform Reveal that you are using the data in your work by emailing Matt Thompson at mthompson@revealnews.org.
- Share the spreadsheets under the same license.

If you alter or build upon our data, you may distribute the result only under the same license. The [full legal code](https://opendatacommons.org/licenses/odbl/1.0/) explains your rights and responsibilities.

### How to credit Reveal

We require that you use the credit “Reveal from The Center for Investigative Reporting." The credit must link to https://www.revealnews.org/ unless the credit is appearing in printed media.

You must also make it clear to anyone who requests access to the data that it is available under the Open Database License. You can [link directly to the license](https://opendatacommons.org/licenses/odbl/1.0/).

## Data documentation

There are two types of salary data, detailed data (file names that include _D_ ), which include employee names, and controller data, which is data obtained from the California State Controller that does not include employee names. The detailed data with names was obtained using California Public Records Act requests to individual cities and counties.

### Field descriptions

|Column name|Format|Description|
|---|---|---|
|year|Integer|Year of salary data|
|data_type|String|Choices: D (detailed) or C (controller)|
|entity_name|String|Name of city or county|
|entity_type|String|Type of jurisdiction. Choices: CITY or COUNTY|
|department|String|Name of top-level department|
|subdepartment|String|Name of sub-department or office|
|position|String|Position title|
|employee_id|String|Usually a numerical ID, often not present|
|orig_name|String|If names were not separated when delivered, the raw name string received in the public records request. Blank in controller data.|
|last_name|String|Blank in controller data.|
|first_name|String|Blank in controller data.|
|middle_name|String|Blank in controller data.|
|name_suffix|String|Blank in controller data.|
|base_pay|Float|May be 0 or null. See "How total pay was calculated" below.|
|total_pay|Float|May be 0 or null. See "How total pay was calculated" below.|
|overtime_pay|Float|May be 0 or null. See "How total pay was calculated" below.
|health_pay|Float|May be 0 or null. See "How total pay was calculated" below.
|retirement_pay|Float|May be 0 or null. See "How total pay was calculated" below.
|deferred_pay|Float|May be 0 or null. See "How total pay was calculated" below.
|misc_pay|Float|May be 0 or null. See "How total pay was calculated" below.

### Why are there names for some records and not for others?

Government employee names and compensation are public record in California. However, employee names are not included in the state controller's data because the agency does not request them from local governments.  

Employee names are included in the data 2008-2012 data CIR requested from the 10 most populous counties and 10 most populous cities. Some cities and counties redacted names for some employees whom they said are protected by law.

### Standardized position titles

CIR identified several top officials across the state to track trends and allow for comparisons. These positions are: city council member, mayor, city manager, police chief, city fire chief, county supervisor, county executive or administrative officer (CEO/CAO), sheriff and district attorney. In records from the state controller, Payday California displays these positions with a standardized title when the official’s title differs in the controller’s database.

### How total pay was calculated

An employee’s total pay is either gross pay prior to deductions or wages subject to Medicare taxes, which tend to be lower than gross wages. Total pay is composed of base pay (usually an employee’s salary), miscellaneous pay (other taxable pay such as car allowances and bonuses, as well as one-time payouts such as unused vacation time) and overtime pay. Payday California displays these types of pay as they were reported to CIR and the controller. In 2009 and 2010, the controller requested only total pay, not separate categories.

### Original site credits

Web development: Michael Corey  

Data analysis and reporting: Joanna Lin  

Research: Emmanuel Martinez and Coulter Jones  

Design: Dave Stanton and Michael Corey  

Copy editing: Sheela Kamath and Nikki Frick  
