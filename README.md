# ncxa
TOD0:
*Change to mapbox: Check if several files can be loaded
* Load geojson directly in Google Maps: https://developers.google.com/maps/tutorials/data/importing_data 
* Coordinate to distance calculations:
  http://www.movable-type.co.uk/scripts/latlong.html
  Formula	
  x = Δλ ⋅ cos φm
  y = Δφ
  d = R ⋅ √x² + y²
  JavaScript:	
  var x = (λ2-λ1) * Math.cos((φ1+φ2)/2);
  var y = (φ2-φ1);
  var d = Math.sqrt(x*x + y*y) * R;


(1) Static url: http://geojson.io/#id=github:rescolo/ncxa/blob/master/NCXA.geojson&map=10/6.3467/-75.1808

TODO:
* cp kml track into kml dir
* cd into kml and run
* Fix the file names with
  $ ./000_fix_names.sh N-1
  where N is the N_* name of the last file withour intial zeroes. 

  $ ./000_generate_full_kml.sh N  #change icon into last position for each track
  which generates the file map_all.kml in the main dir
* upload to (1)
* Save kml and upload to "My maps": https://www.google.com/maps/d/u/0/edit?mid=z2NCe4lIOjVA.kgQgTDLLMHfw
* Save as geojson
* copy saved file into local git repo
* Fix index.php and commit and push with
  $ ./fix_index.php.sh "COMMIT MESSAGE share:HASH" # with the share HASH
* pull from /var/www/ncxa






