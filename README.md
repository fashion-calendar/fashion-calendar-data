# Fashion Calendar Dataset and Code
## Summary
This repository stores data and code for the [Fashion Calendar Research Database](https://fashioncalendar.fitnyc.edu/), a project of the Fashion Institute of Technology's Gladys Marcus Library and the FIT History of Art Department. From 1941 to 2014, Ruth Finley published the *Fashion Calendar*, an independent, weekly periodical that served as the official scheduling clearinghouse for the American fashion industry. In 2020, FIT was awarded a Digitizing Hidden Collections grant for “The Ruth Finley Collection: Digitizing 70 Years of the Fashion Calendar,” from the Council on Library and Information Resources (CLIR) to digitize this important resource. Information about the events listed in the *Fashion Calendar*—the who, what, when, where—was extracted and parsed from each issue. Names and entities in the listings (i.e. designers and brands) were categorized to highlight gender, race, social class, sexual identity, nationality, etc. The [Fashion Calendar Research Database](https://fashioncalendar.fitnyc.edu/) makes the data over 200,000 events searchable, graphable and mappable, allowing users to discover rich patterns and threads woven into the history of fashion and the creative industries.

Both the underlying dataset for the project and code used to extract the data from the digitized issues are available in this repository. Please visit the [Fashion Calendar Research Database](https://fashioncalendar.fitnyc.edu/) for more information and context on this project.

Principal Investigator: Natalie Nudell, History of Art, FIT  
Co-Prinicipal Investigator: Joseph Anderson, FIT Library  
contact: [fashioncalendar@fitnyc.edu](mailto:fashioncalendar@fitnyc.edu)

## Rights and Reuse
All data and code are copyrighted and have been made available by the Fashion Institute of Technology under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/). This means you are free to share and adapt this material as long as you provide attribution, include a link to the license, and indicate if you have made any changes. When providing an attribution for this material, we request you include the credit, “Courtesy of the Fashion Institute of Technology-SUNY, Gladys Marcus Library unit of Special Collections and FIT Archive under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).” For example, to cite this dataset:

"Fashion Calendar 1941-2014 Dataset," [https://github.com/fashion-calendar/fashion-calendar-data](https://github.com/fashion-calendar/fashion-calendar-data). Courtesy of the Fashion Institute of Technology-SUNY, Gladys Marcus Library unit of Special Collections and FIT Archive under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

For more information, see our page on [Rights and Reuse](https://fashioncalendar.fitnyc.edu/page/rights) on the Fashion Calendar Research Database.

## Dataset for the Fashion Calendar 1941-2014

The dataset for this project is broken into 3 parts: "events", "names" and "categories". The "events" subset is the foundation of the dataset. Names listed in the "events" subset are linked to name entities listed in the "names" subset, which are then linked to category entities in the "categories" subset. Where possible names and categories are based and linked to wikidata entities based on the "_id" field. If the "_id" begins with a Q then that is the corresponding wikidata identifier for the entity. Because many names listed in the Fashion Calendar did not have corresponding wikidata entries, many are prefixed with FC, which indicates it identified by the project's own system.

categories-fc.json is all categories listed used in the database.  

names-fc.json is all names in the database, including reference to their respective categories by their _id, 'category_id'.  

events-fc.json is all the listed events, including reference to the respective names by their _id, 'name_id'.  

## Code used for the Fashion Calendar Research Database

fourcolumnsreduced.py and FourColumnsReduced.ipynb is python code used to extract and parse data from digitized copies of the Fashion Calendar.

## License

All data is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[![CC BY 4.0][cc-by-shield]][cc-by]


[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
