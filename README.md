Boxes
=====

Steve Woods - LaniLogic Technology Solutions Ltd
steve@lanilogic.com
May 2013

This is a very simple framework for setting up column-based layouts in CSS, which also allow
you to very easily over-ride with responsive values simply by specifying a new width percentage
for each column type.

Column declarations
-----------------------
Take care to make sure that all columns add up to 100%, i.e.

  <div class='col col25'></div>
  <div class='col col50'></div>
	<div class='col col25'></div>
	<br class='clearFix' />

3 Column Layouts example.
	Also notice that .col34 exists for using .col33 in a 3 column layout:
	33%+33%+33% = 99% so we make one 34% to equal 100%
	Other examples:
	34% + 66% = 100%

Add your own column permutations as you see fit :-)

For responsiveness, simply over-ride the .col class with your own desired percentage in your media-queries i.e.;
	.col { width: 100% !important; }

	or even specific columns, such as:
	.col33 { width: 100%; } 
	to convert a 3 column section into a single column that will then stack 
	(Don't forget to add the same override to .col34 if you do this)

Enjoy!

*/
