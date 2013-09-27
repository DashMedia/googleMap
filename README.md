googleMap
=========

Static Google Map Output Modifier for MODX


googleMap Output Modifier

##DESCRIPTION
This output modifier accepts an address and returns a url for the static map image

###PARAMETERS
`w` - width, `h` - height, `z` - zoom level, `key` - Google Maps API v3 Key, `sensor` - (1 or 0), `marker` - (1 or 0)
###OUTPUT MODIFIER USAGE:
```
<img [[*tvAddress:googleMap=`w=425,h=300,z=16,key=xxxxxxxxxxx,sensor=0,marker=1`]] />
```

key is the only *REQUIRED* variable, unless you set up a system setting named `google_api_key`
then the snippet will use that value whenever `key` is not passed
###SNIPPET USAGE:
```
<img [[!googleMap? &address=`[[*tvAddress]]` &w=`425` &h=`300` &z=`16` &marker=`1` &sensor=`0`]] />
```

AUTHOR: Jason Carney, DashMedia.com.au
