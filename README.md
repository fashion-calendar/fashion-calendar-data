# Fashion Calendar Dataset and Code
## Dataset for the Fashion Calendar Research Database

categories.json is all categories listed used in the database.  

names.json is all names in the database, including reference to their respective categories by their _id, 'category_id'.  

events.json is all the listed event, including reference to the respective names by their _id, 'name_id'.  

fashion-calendar.events.json is the previous 3 datasets merged together starting at the event level, and then nested with names and categories.

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



All code is licensed under the [MIT License](https://opensource.org/licenses/MIT).

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
