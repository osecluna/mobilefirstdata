# Mobile First Data

This is a repository for the data that goes with the mobile first version of MobileFirst.

# NPM scripts

## Zip data
`npm run zipData` - Zips up the data before it can be imported in a BM.

# Product Types : 
1. Simple Product with no variant
2. Simple Product with single variant
3. Simple Product with multiple variants
4. product Set
5. product Bundles
6. variation group (not introduce yet as of May 2017)
7. product options (electronics) 


# Price Types :
1. List Price
2. Sale Price
3. Promotion Price
3. Price range
4. Tiered Price. (this is not working due to platform limitation) 
5. option price. 



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
|home-product-set-content |Home Product Set Content | Homepage |Content links to a product set and is assigned to the 'home-product-set' slot.|


# Slots
| ID                      | Rendering Template | Usage             |description|
|-------------------------|------|-------------------|-----------|
|home-categories          |slots/content/contentassetbody.isml| Homepage |This slot renders images that link to other category pages it uses the content asset 'home-categories'.|
|home-main                |slots/content/contentassetbody.isml| Homepage |Main image displayed on the homepage, used by the content asset 'home-main'.|
|home-product-set-content |slots/content/contentassetbody.isml| Homepage |This slot desiplays an image that links to a product set|

# Promotions
| ID                                                     | Qualifying Products | Coupon     | Campaign                    |
|--------------------------------------------------------|---------------------|------------|-----------------------------|
| mobile-first-order-coupon-promotion-1                  | 883360541815        | orderLevel | Mobile First Coupon Test    |
| mobile-first-shipping-coupon-promotion-1               | 740357377119        | shipping   | Mobile First Coupon Test    |
| mobile-first-product-coupon-promotion-1                | 682875719029        | product    | Mobile First Coupon Test    |
| mobile-first-order-no-coupon-promotion-1               | 883360543307        |            | Mobile First No Coupon Test |
| mobile-first-shipping-no-coupon-promotion-1            | 740357447164        |            | Mobile First No Coupon Test |
| mobile-first-order-approaching-discount-promotion-1    | 799927767720        |            | Mobile First No Coupon Test |
| mobile-first-shipping-approaching-discount-promotion-1 | 799927767720        |            | Mobile First No Coupon Test |