Inflector
=========

Inflector to pluralize and singularize English nouns.

This Inflector is a port of Ruby on Rails Inflector.

It can be really helpful for developers that want to
create frameworks based on naming conventions rather than
configurations.

It was ported to PHP for the Akelos Framework, a
multilingual Ruby on Rails like framework for PHP.

* author: Bermi Ferrer Martinez
* copyright: Copyright (c) 2002-2006, Akelos Media, S.L. http://www.akelos.org
* licence: GNU Lesser General Public License

Usage Examples
--------------

``` php

<?php

/* Singular to plural / Plural to singular */

echo Inflector::pluralize('search'); // outputs searches
echo Inflector::singularize('cases'); // outputs case
echo Inflector::pluralize('query'); // outputs queries
echo Inflector::singularize('queries'); // outputs query
echo Inflector::pluralize('ability'); // outputs abilities
echo Inflector::singularize('abilities'); // outputs ability
echo Inflector::pluralize('analysis'); // outputs analyses
echo Inflector::singularize('analyses'); // outputs analysis
echo Inflector::pluralize('information'); // outputs information
echo Inflector::singularize('information'); // outputs information
echo Inflector::pluralize('mouse'); // outputs mice
echo Inflector::singularize('mice'); // outputs mouse

/* CamelCase to underscore / underscore to CamelCase */

echo Inflector::underscore('SpecialGuest'); // outputs special_guest
echo Inflector::camelize('special_guest'); // outputs SpecialGuest
echo Inflector::underscore('FreeBSD'); // outputs free_bsd
echo Inflector::camelize('free_bsd'); // outputs FreeBsd
echo Inflector::underscore('HTML'); // outputs html
echo Inflector::camelize('html'); // outputs Html

/* Underscore to "human-text" / "Human-text" to Underscore */

echo Inflector::humanize('employee_salary'); // outputs Employee salary
echo Inflector::underscore('Employee salary'); // outputs employee_salary

/* Examples of titleize() */

echo Inflector::titleize('ActiveRecord'); // outputs Active Record
echo Inflector::titleize('action web service'); // outputs Action Web Service

/* Examples of ordinalize() */

echo Inflector::ordinalize(1); // outputs 1st
echo Inflector::ordinalize(2); // outputs 2nd
echo Inflector::ordinalize(3); // outputs 3rd
echo Inflector::ordinalize(4); // outputs 4th
echo Inflector::ordinalize(5); // outputs 5th
echo Inflector::ordinalize(20); // outputs 20th
echo Inflector::ordinalize(21); // outputs 21st

```

