# Roundcube plugin - Smart Autocomplete

Find your recipients faster by optimizing autocomplete results order.

This plugin performs statistical analysis of accepted autocomplete suggestions and
prioritizes frequently contacted addresses. It goes one step further and correlates
selected suggestion with original search string.



## Example of what you can teach Roundcube by using this plugin

Say you have two contacts with quite similar names:

- friend no.1 is 'Leslie Rosenberg',
- friend no.2 is 'Leslie Rosemann'.

The first one you know since childhood and you call each other by first names, 'Leslie'.
The second contact is your business consultant and you refer to her usually by surname, 'Rosemann'.

If you start typing 'les' and select 'Leslie RoseNBERG' from autocomplete suggestions, and
go on and start typing 'ros' and select 'Leslie RoseMANN', you have just trained RC to
display correct contact as first autocomplete suggestion for both occasions.




## Requirements

Whichever RC release has this PR merged: https://github.com/roundcube/roundcubemail/pull/5203

Expected to be merged in v1.1.5 and v1.2.0.



## TODO

- DONE configurable max length of email address - long email addresses are probably
    autogenerated (mailing list Return-Path:, for example)
- setting button to remove all learned autocomplete data, so user can start teaching
    RC from scratch at any time
- check automatic addressbook (autocomplete only works for addresses in address book?)
- implement minimun search string length?
- searchstring sanitization before using it in queries