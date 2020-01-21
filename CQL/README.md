# Using Common Query Language (CQL) in WMS Layer

Get the new ShapeFile from https://download.geofabrik.de/asia/sri-lanka.html

(1) Select `three dot`on the Openlayer Layer Preview and it looks like this:
    
![1](1st.PNG)

(2) And then using the value of `code=5141`. The `code=5141` represents only the `small_roads`. 

DESCRIPTION - `4 digit code (between 1000 and 9999) defining the feature class. The first one or
two digits define the layer, the last two or three digits the class inside a layer.` And it looks like:
    
![2](2nd.PNG)
    
(3) Then Finally using the value of `fclass='public_building'`. The `fclass='public_building'` represents only `An unspecified public building`.

DESCRIPTION - `Class name of this feature. This does not add any information that is not already
in the “code” field but it is better readable.` And it looks like:
    
![3](3rd.PNG)

```That's it Thanks!```
