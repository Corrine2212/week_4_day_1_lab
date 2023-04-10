**ANSWERS:**

1.  Return ALL the data in the 'movies' table.
--SELECT * FROM movies;


2.  Return ONLY the name column from the 'people' table
--SELECT name FROM people;


3.  Oops! Someone spelled Krusty The Clown's name wrong! Change it to reflect the proper spelling (Crusty should be Krusty).
--UPDATE people SET name = 'Krusty the Clown' WHERE name = 'Crusty the Clown';

4.  Return ONLY Homer Simpson's name from the 'people' table.
--SELECT name FROM people WHERE name = 'Homer Simpson';
					--OR where id = 1;


5.  The cinema is showing 'Batman Begins', but Batman is DC, not Marvel! Delete the entry from the 'movies' table.
--DELETE FROM movies WHERE title = 'Batman Begins';



6.  We forgot one of the main characters! Add Bart Simpson to the 'people' table
--INSERT INTO people (name) VALUES('Bart Simpson');


7.  Eric Cartman has decided to hijack our movie evening, Remove him from the table of people.
--DELETE FROM people WHERE name = 'Eric Cartman';

8.  The cinema has just heard that they will be holding an exclusive midnight showing of 'Avengers: Infinity War'!! Create a new entry in the 'movies' table to reflect this.
--INSERT INTO movies(title, year, show_time) VALUES ('Avengers: Infinity War', 2018, '00:00');

9.  The cinema would like to make the Iron Man movies a triple billing. Find out the show time of "Iron Man 2" and set the show time of "Iron Man 3" to start two hours later.
--SELECT show_time FROM movies WHERE title = 'Iron Man 2';
--UPDATE movies SET (show_time) = '20.45' WHERE title = 'Iron Man 3';

EXTENSION: Research how to delete multiple entries from your table in a single command.
--DELETE FROM movies WHERE year BETWEEN '2008' AND '2011';
--DELETE FROM movies WHERE title LIKE ‘Iron Man%’;







