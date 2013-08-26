# Manual

This script is pretty straightforward. Use this syntax in Drafts, then trigger the action:

    [POSTALCODE], [COUNTRY ABBREVIATION]
	
This is not case-sensitive.
	
For example, if you want to know the postal codes of Beverky Hills:

    90210, US
	
For now, the API doesn't support empty country fields. This can be a hassle. You can find the country codes [here](http://www.zippopotam.us/#where), but the state codes can be a little hard to find.

# Result

A markdown list of all city with that postal code in the given country.

# Remarks

This script utilizes the awesome API of [Zippopotamus](http://www.zippopotam.us/).
