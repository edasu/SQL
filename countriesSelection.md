```sql
CREATE PROCEDURE solution()
BEGIN
	SELECT name, continent, population
    FROM countries
    WHERE continent = "Africa"
    ORDER BY name ASC;
END
```

Given a list of countries, your friend should identify all the countries that are in Africa. To help her, you have decided to write a function that will find all such countries from any set of countries. The countries table in which the countries are stored has the following structure:

name: the name of the country;
continent: the continent on which the country is situated;
population: the country's population.
Your task is to return a new table that has the same columns, but that only contains the countries from Africa. The countries should be sorted alphabetically by their names.