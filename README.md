# top-pot
January 6 Assignment for calculating donut demand estimates at top pot locations

The purpose of this program is to produce estimates for the hourly and daily totals of how many donuts may be needed to meet sales demands at five different Top Pot Donut store locations.  The estimates are calculated by running several pieces of numerical data, which have been tabulated at each store, through algorithms.

One important piece of data is the range of potential customers passing by each store for any given hour.  A piece of code found at the URL below was very useful for selecting a random element from within this range to determine an estimate of how many customers may enter a store.
http://stackoverflow.com/questions/1527803/generating-random-numbers-in-javascript-in-a-specific-range

That element is then used in conjunction with the average percentage of customers who enter a store and the average number of donuts purchased by each customer to determine demand for each one hour time slot.  These estimates are then accumulated to determine the estimate for total daily demand at each store.

All of this information is applied to a constructor function to create objects representing the data sets for each store.

I worked directly with Keri Brady to find solutions for applying the calculations correctly for one test store initially.Her use of the algorithm found on Stackoverflow.com was the most important piece to move the project forward when we were both feeling really stuck.  I then worked through ideas to apply 'for loops' and arrays to several sections of the program to eliminate repetitive code.  Brook helped provide guidance when my introduction of arrays presented problems that I could not figure out. Stephanie worked through the final versions with me and helped me understand how moving more of my functions/methods into my constructor function would eliminate more unneccessary lines of code and make my objects more comprehensive with respect to data for each store as a set.

The console output results from one run of my program are pasted below:

 -------------------------------------
donuts.html:44 Downtown needs 148 donuts between 7 and 8 a.m.
donuts.html:44 Downtown needs 122 donuts between 8 and 9 a.m.
donuts.html:44 Downtown needs 172 donuts between 9 and 10 a.m.
donuts.html:44 Downtown needs 209 donuts between 10 and 11 a.m.
donuts.html:44 Downtown needs 150 donuts between 11 a.m. and 12 p.m.
donuts.html:44 Downtown needs 181 donuts between 12 and 1 p.m.
donuts.html:44 Downtown needs 187 donuts between 1 and 2 p.m.
donuts.html:44 Downtown needs 83 donuts between 2 and 3 p.m.
donuts.html:44 Downtown needs 190 donuts between 3 and 4 p.m.
donuts.html:44 Downtown needs 116 donuts between 4 and 5 p.m.
donuts.html:44 Downtown needs 169 donuts between 5 and 6 p.m.
donuts.html:47 Downtown needs 1761 donuts per day
donuts.html:42 -------------------------------------
donuts.html:44 Capitol Hill needs 16 donuts between 7 and 8 a.m.
donuts.html:44 Capitol Hill needs 30 donuts between 8 and 9 a.m.
donuts.html:44 Capitol Hill needs 19 donuts between 9 and 10 a.m.
donuts.html:44 Capitol Hill needs 40 donuts between 10 and 11 a.m.
donuts.html:44 Capitol Hill needs 44 donuts between 11 a.m. and 12 p.m.
donuts.html:44 Capitol Hill needs 15 donuts between 12 and 1 p.m.
donuts.html:44 Capitol Hill needs 29 donuts between 1 and 2 p.m.
donuts.html:44 Capitol Hill needs 39 donuts between 2 and 3 p.m.
donuts.html:44 Capitol Hill needs 24 donuts between 3 and 4 p.m.
donuts.html:44 Capitol Hill needs 17 donuts between 4 and 5 p.m.
donuts.html:44 Capitol Hill needs 28 donuts between 5 and 6 p.m.
donuts.html:47 Capitol Hill needs 239 donuts per day
donuts.html:42 -------------------------------------
donuts.html:44 South Lake Union needs 190 donuts between 7 and 8 a.m.
donuts.html:44 South Lake Union needs 221 donuts between 8 and 9 a.m.
donuts.html:44 South Lake Union needs 193 donuts between 9 and 10 a.m.
donuts.html:44 South Lake Union needs 233 donuts between 10 and 11 a.m.
donuts.html:44 South Lake Union needs 206 donuts between 11 a.m. and 12 p.m.
donuts.html:44 South Lake Union needs 189 donuts between 12 and 1 p.m.
donuts.html:44 South Lake Union needs 242 donuts between 1 and 2 p.m.
donuts.html:44 South Lake Union needs 181 donuts between 2 and 3 p.m.
donuts.html:44 South Lake Union needs 232 donuts between 3 and 4 p.m.
donuts.html:44 South Lake Union needs 187 donuts between 4 and 5 p.m.
donuts.html:44 South Lake Union needs 242 donuts between 5 and 6 p.m.
donuts.html:47 South Lake Union needs 2287 donuts per day
donuts.html:42 -------------------------------------
donuts.html:44 Wedgewood needs 34 donuts between 7 and 8 a.m.
donuts.html:44 Wedgewood needs 22 donuts between 8 and 9 a.m.
donuts.html:44 Wedgewood needs 43 donuts between 9 and 10 a.m.
donuts.html:44 Wedgewood needs 55 donuts between 10 and 11 a.m.
donuts.html:44 Wedgewood needs 54 donuts between 11 a.m. and 12 p.m.
donuts.html:44 Wedgewood needs 43 donuts between 12 and 1 p.m.
donuts.html:44 Wedgewood needs 34 donuts between 1 and 2 p.m.
donuts.html:44 Wedgewood needs 41 donuts between 2 and 3 p.m.
donuts.html:44 Wedgewood needs 45 donuts between 3 and 4 p.m.
donuts.html:44 Wedgewood needs 33 donuts between 4 and 5 p.m.
donuts.html:44 Wedgewood needs 49 donuts between 5 and 6 p.m.
donuts.html:47 Wedgewood needs 445 donuts per day
donuts.html:42 -------------------------------------
donuts.html:44 Ballard needs 60 donuts between 7 and 8 a.m.
donuts.html:44 Ballard needs 74 donuts between 8 and 9 a.m.
donuts.html:44 Ballard needs 28 donuts between 9 and 10 a.m.
donuts.html:44 Ballard needs 54 donuts between 10 and 11 a.m.
donuts.html:44 Ballard needs 45 donuts between 11 a.m. and 12 p.m.
donuts.html:44 Ballard needs 29 donuts between 12 and 1 p.m.
donuts.html:44 Ballard needs 74 donuts between 1 and 2 p.m.
donuts.html:44 Ballard needs 69 donuts between 2 and 3 p.m.
donuts.html:44 Ballard needs 37 donuts between 3 and 4 p.m.
donuts.html:44 Ballard needs 39 donuts between 4 and 5 p.m.
donuts.html:44 Ballard needs 61 donuts between 5 and 6 p.m.
donuts.html:47 Ballard needs 544 donuts per day

