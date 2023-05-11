# LibreOfficeBaseNotes
my notes on using libreoffice base

## Forms

The wizard is your friend, when modifying a form, on the left hand side make sure wizard is on, when adding a dropdown or something

### Dropdown

to have a dropdown menu that is populated with something different than it uses in the relationship use a listbox. If you want custom text to appear that isn't in the table, then create a view - the listbox wizard won't let you use a computed field but you can then edit the sql by hand afterwards.

## Queries

If you want to do a `union` you need to open the query in the SQL editor and on the toolbar at the top, on the right choose "Run SQL Command Directly"

### Time Deltas

To get a delta for dates you do something like this

  SELECT * FROM "WORKOUT" WHERE DATEDIFF( 'mm', "DATE", CURDATE( ) ) < 1
 
notice the single quotes on mm
