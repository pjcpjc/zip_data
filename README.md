Munged it from 
[here](https://data.opendatasoft.com/explore/dataset/georef-united-states-of-america-zc-point%40public/table/?flg=en-us)

Only annoying part of the munging was the json I downloaded truncated the 
leading zeros, which is odd since it was a json file with the zip serialized
as text. I fixed it just by prepending "0" to the zips with length 
four, while double checking that they were in the states that have 
such zips.

* `conus.json` - has the zip code with the lat and lon.
* `conus_zips.json` shorted file with just the zips.