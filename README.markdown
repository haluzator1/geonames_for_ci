# GeoNames CI Library 1.0 -
GeoNames Library is a library for CodeIgniter to the various webservices offered by the GeoNames project.

## Information about GeoNames (source: Wikipedia) --
GeoNames is a geographical database available and accessible through various Web services, under a Creative Commons attribution license.

The GeoNames database contains over 10,000,000 geographical names corresponding to over 7,500,000 unique features. All features are categorized into one out of nine feature classes and further subcategorized into one out of 645 feature codes. Beyond names of places in various languages, data stored include latitude, longitude, elevation, population, administrative subdivision and postal codes. 

## Install
1. Set GeoNames username in your config file (application/config/geonames.php).
2. Login to your GeoNames account, go to "manage account" page (http://www.geonames.org/manageaccount) and enable account to use the free web services.
3. Enjoy it.

-- Use --
		<?php
		$this->load->library('geonames');

		$results = $this->geonames->countryInfo(array('country'=>'SK','lang'=>'en'));
		echo $results['geonames'][0]->countryName;
		?>