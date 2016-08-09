# Mobile First SiteGenesis Data

This is a repository for the data that goes with the mobile first version of SiteGenesis.


# Install/Import
To use this data with in a sandbox

1. The directory 'demo\_data\_no\_hires\_images' needs to compressed into a zip file of the same name.
		e.g 'demo\_data\_no\_hires\_images.zip'.


2. The zip file needs to be uploaded to the instance's BM.  In the BM go to Administration >  Site Development >  Site Import & Export.  Then upload the zip file from step#1.

3. Import the zip file from within the BM.

4. (optional steps)
	a. Check the cartridge path for the sites.
	b. Run the search index.


## Content Assets
Here is a list of the content assets used from the shared content library.


| ID                      | Name | Usage             |description|
|-------------------------|------|-------------------|-----------|
|home-categories          |Home Categories| Homepage |Images that link to category pages, this is used by the content slot 'home-categories'.|
|home-main                |Home Main| Homepage |Main image displayed on the homepage, used by the content slot 'home-main'.|
|home-product-set-content |Home Product Set Content | Homepage |Content shown on the homepage that will reveal product tiles of products assigned to the 'home-product-set' slot.|
|home-product-tile-content|Home page product tiles|Homepage| Content that is embeded within the product tiles, this content asset is used in the rendering template 'slots/product/homepage-product-slot.isml' for the slot 'home-products'|



# Slots
| ID                      | Rendering Template | Usage             |description|
|-------------------------|------|-------------------|-----------|
|home-categories          |slots/content/contentassetbody.isml| Homepage |This slot renders images that link to other category pages it uses the content asset 'home-categories'.|
|home-main                |slots/content/contentassetbody.isml| Homepage |Main image displayed on the homepage, used by the content asset 'home-main'.|
|home-product-set-content |slots/product/homepage-product-set-slot.isml| Homepage |This slot desiplays a product set and when clicked reveals product tiles belonging to the set.  Products used include 740357377041, 013742335422, 701642819431, 701644059262|
|home-products|slots/product/homepage-product-slot.isml|Homepage| This slot shows product tiles on the homepage, and uses the rendering template products used are 701644179922, 701644329402, 701644391751, 701642991014, 750518699578|

