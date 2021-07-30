# 03-United-nations

### Author details
##### #24 Andrea Zappa
***

<h4>Requirements</h4>

- Make a ```<ul>``` list of countries:

1. Each list item should contain: the flag, the name and the population number
The name should be left aligned and the population should be right aligned
2. Countries with large populations should be highlighted in some way
3. The flags area should have a background color
4. If the flag is not rectangular (e.g. Switzerland) the flag should be centered in the flag area
5. Include at least one country with an irregularly sized flag (e.g Switzerland)
6. The list should contain at least 50 countries and should be scrollable
- Include a header above the list
7. It should contain the following titles: 'Flag', 'Country', 'Population'
8. It should be spaced and aligned properly
9. It should remain in place when the list is scrolled
 Not to be confused with the ```<header>``` tag

<h4>My solution</h4>

1. I've created an unordered list which contains a list elements within. 
The flag area, name of contry and population number are just an inline-blocked ```span``` elements that have been inserted into the ```li``` list item.
In stylesheet the three elements above described have been placed ```position:relative``` to each other;
the country name has a negative value because of its position in the html flow, so to be positioned left we must set negative values.
The same technique has been applied for the flag-area and population fields.
2. TO-DO
3. I choose a background color to cover the entire flag-area field.
4. In HTML some of the flags images have been tagged with a ```.irregular-flag``` class which apply a 25% margin to the four directions. The result match the requirement.
5. Done.
6. Done. The entire ```flags-list``` is set with ```overflow-y: scroll``` .
7. In HTML a ```div#header``` has been placed on top of the list and styled with ```position:fixed``` and a ```z-index``` because without that the list overlaps the header when scrolling.
8. Done, ```width``` has been set manually as precise as possible.
9. go to #7