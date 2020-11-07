# loadmore-with-ajax
Here's the code that will help you load more products on your website without changing url such as url/page/1.

The website that are using it are 
* [bettergiftflowers.com](https://www.bettergiftflowers.com)
* [flipkart.com](https://www.flipkart.com)

*
CALLBACK FUNCTIONS
The following functions are available to be dispatched by Ajax Load More.

Complete – The almComplete() function is triggered after every successful ajax call made by Ajax Load More.

almComplete = function(alm){
    // Your on complete code goes here
};
Destroyed – The almDestroyed() function is dispatched after the destroy_after shortcode parameter is triggered.

almDestroyed = function(alm){
    console.log('"Ajax Load More functionality has been destroyed!');
};
Done – The almDone() function is triggered after all posts have been loaded.

almDone = function(alm){
    console.log('All posts have been loaded!');
};
Empty – The almEmpty() function is triggered if there are zero results returned in the initial query.

almEmpty = function(alm){
   console.log('Sorry, but we could not locate any posts that matched your criteria.');
};
Filter Complete – The almFilterComplete() function is triggered after a successful call to the public function almFilter().

almFilterComplete = function(){
    console.log('Ajax Load More filter has completed!');
};
URL Update – The almUrlUpdate() function is triggered after a successful URL update (pushState) from the Single Post or the Search Engine Optimization add-on

almUrlUpdate = function(permalink, type){
    console.log("URL updated to " + permalink + '- dispatched from the '+ type + ' add-on.');
};
