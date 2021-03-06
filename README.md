# Web map that displays a WMS layer

(1) Install Geoserver from http://geoserver.org/release/stable.

![1](img/1.png)

(2) Then open http://localhost:8080/geoserver/web/ and login with your username and password, given while you’re installing the Geoserver process in Point 1. The default username is `admin` and the password is `geoserver`.

![2](img/2.png)

(3) On your Left, `Select Data` → `Workspaces`. 

![3](img/3.png)

(4) Select `Add new workspace`.

![4](img/4.png)

(5) Give a `name`.

(6) Then for Namespace URI give as `http://geoserver.org/name/`

(7) Then `submit` it.

![5 6 7](img/5_6_7.png)

(8) Now, Your Workspace is created.

(9) Then Go to `Data` → `Stores`.

(10) Then click `Add new store`.

![9 10](img/9_10.png)

(11) Select the Vector Data `Souces` → `shapefile`.

![11](img/11.png)

(12) Then select your Workspace `name` created in Point 6.

(13) Give a `Data Source Name`.

(14) `Browse` and locate the `Shapefile`.

(15) `Submit` it.

![12 13 14 15](img/12_13_14_15.png)

(16) Click on `Publish`.

![16](img/16.png)

(17) Scroll Down, and find Bounding Boxes, then click on `compute from data`.

(18) Then again click on `Compute on native bounds`.

![17 18](img/17_18.png)

(19) Then `save` it.

![19](img/19.png)

(20) Now, Go to `Data` → `Layer Preview`.

![20](img/20.png)

(21) Search your Created Layer and select the Openlayer.

![21](img/21.png)

(22) A pop-up tab opens and shows the Layer.

![22](img/22.PNG)

### CONTINUE WITH CQL

# Using Common Query Language (CQL) in WMS Layer

Get the new ShapeFile from https://download.geofabrik.de/asia/sri-lanka.html

(1) Select `three dot`on the Openlayer Layer Preview and it looks like this:
    
![1](CQL/1st.PNG)

(2) And then using the value of `code=5141`. The `code=5141` represents only the `small_roads`.

DESCRIPTION - `4 digit code (between 1000 and 9999) defining the feature class. The first one or
two digits define the layer, the last two or three digits the class inside a layer.` And it looks like:
    
![2](CQL/2nd.PNG)
    
(3) Then Finally using the value of `fclass='public_building'`. The `fclass='public_building'` represents only `An unspecified public building`.

DESCRIPTION - `Class name of this feature. This does not add any information that is not already
in the “code” field but it is better readable.` And it looks like:
    
![3](CQL/3rd.PNG)

```That's it Thanks!```
