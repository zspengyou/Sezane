## what
This is for adding item to basket for Sezane. 

## how to install
1. install [tampermonkey](https://www.tampermonkey.net/) script to your chrome browser
2. install this script


## how does it works

1. this script will start when the page finished loading
2. it will run `mainFunction` every 5 second (`5*1000`)
3. it will check the availability based on CSS, 
31. if it is available, then click the `addToBasketBtn` button and set `addItemToBusketSuccess` to 1, then it will stop executing the script `clearInterval(timerId);`
31. if it is not available, then wait for 5 second (`5000`) and refresh the page, then start from step1

## customization 

### alarm sound 
https://notificationsounds.com
pick the sound you like, then update the url

### product page
update the `@match        https://www.sezane.com/us/product/collection-ete-all/ilonie-blouse?cou_Id=3041` to the page that you are interested in

### product size
update `MainContentPlaceHolder_rptTaille_liTaille_1` to be the product size you want 

### target CSS
update the `targetSizeCss` variable `product-page__size__item product-page__size__item--active` to be the CSS on the page. 

## todo 
update the CSS, split it, then check `product-page__size__item--active`


