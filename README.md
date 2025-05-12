# cs546-lab6--a-restaurant-api-solved
**TO GET THIS SOLUTION VISIT:** [CS546 Lab6 -A Restaurant API Solved](https://www.ankitcodinghub.com/product/cs546-lab6-a-restaurant-api-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;91590&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS546 Lab6 -A Restaurant API Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="section">
<table>
<tbody>
<tr>
<td></td>
</tr>
<tr>
<td></td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
CS-546 Lab 6

A Restaurant API

For this lab, you will create a simple server that provides an API for someone to Create, Read, Update, and Delete restaurants and also restaurant reviews.

We will be practicing:

Seperating concerns into different modules: Database connection in one module Collections defined in another

Data manipulation in another

Practicing the usage of async / await for asynchronous code Continuing our exercises of linking these modules together as needed Developing a simple (9 route) API server

Packages you will use:

You will use the mongodb (https://mongodb.github.io/node-mongodb-native/) package to hook into MongoDB

You may use the lecture 4 code (https://github.com/stevens-cs546-cs554/CS- 546/tree/master/lecture_04/code) and the lecture 5 code (https://github.com/stevens-cs546-cs554/CS- 546/tree/master/lecture_05/code) and lecture 6 code (https://github.com/stevens-cs546-cs554/CS- 546/tree/master/lecture_06/code) as a guide.

You can read up on express (http://expressjs.com/) on its home page. Specifically, you may find the API Guide section on requests (http://expressjs.com/en/4x/api.html#req) useful.

You must save all dependencies you use to your package.json file

Folder Structure

</div>
</div>
</td>
</tr>
</tbody>
</table>
<div class="layoutArea">
<div class="column">
https://sit.instructure.com/courses/50148/assignments/273386

</div>
<div class="column">
1/12

</div>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
12/14/21, 11:46 PM Lab 6

You will use the following folder structure for the data module. You may need other files to handle the connection to the database as well.

<pre>  ./
  ../data/
  ../data/restaurants.js
  ../data/index.js
  ../data/reviews.js
  ../routes/
  ../routes/restaurants.js
  ../routes/index.js
  ../routes/reviews.js
  ../app.js
  ../package.json
</pre>
I also recommend having your database settings centralized in files, such as:

<pre>  ./
  ../config/
  ../config/mongoConnection.js
  ../config/mongoCollections.js
</pre>
Database Structure

You will use a database with the following structure:

The database will be called FirstName_LastName_lab6

The collection you use to store restaurants will be called restaurants you will store a sub-document of reviews

restaurants

The schema for restaurants is now as followed:

<pre>  {
      _id: ObjectId,
</pre>
<pre>      name: string,
      location: string,
      phoneNumber: string (xxx-xxx-xxxx format),
      website: string (must contain full url http://www.patrickseats.com),
      priceRange: string (from $ to $$$$),
      cuisines: [strings],
      overallRating: number (from 0 to 5 this will be a computed average from all the reviews posted f
</pre>
<pre>  or a restaurant,
      the initial value of this field will be 0 when a restaurant is created),
      serviceOptions: {dineIn: Boolean, takeOut: Boolean, delivery: Boolean},
      reviews: [] (an array of review objects, you will initialize this field to be an empty array whe
</pre>
<pre>  n a restaurant is created)
  }
</pre>
The **_id** field will be automatically generated by MongoDB, so you do not need to provide it.

The _id field will be automatically generated by MongoDB when a restaurant is inserted, so you do not need to provide it when a restaurant is created.

</div>
</div>
<div class="layoutArea">
<div class="column">
https://sit.instructure.com/courses/50148/assignments/273386 2/12

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="section">
<div class="layoutArea">
<div class="column">
12/14/21, 11:46 PM Lab 6

</div>
</div>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
An example of how The Saffron Lounge would be stored in the DB when it’s first created:

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
<pre>{
    _id: ObjectId("507f1f77bcf86cd799439011"),
    name: "The Saffron Lounge",
    location: "New York City, New York",
    phoneNumber: "123-456-7890",
    website: "http://www.saffronlounge.com",
    priceRange: "$$$$",
    cuisines: ["Cuban", "Italian" ],
    overallRating: 0
    serviceOptions: {dineIn: true, takeOut: true, delivery: false},
    reviews: []
</pre>
}

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
The Restaurant Review Sub-document (stored within the restaurants document)

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
<pre>{
  _id: ObjectId,
  title: string,
  reviewer: string,
  rating: number (from 1 to 5),
  dateOfReview: string (must be a valid date string),
  review: string
</pre>
}

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
For example a review:

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
<pre>{
  _id: ObjectId("603d992b919a503b9afb856e"),
  title: "This place was great!",
  reviewer: "scaredycat",
  rating: 5,
  dateOfReview: "10/13/2021",
  review: "This place was great! the staff is top notch and the food was delicious!  They really kno
</pre>
<pre>w how to treat their customers"
}
</pre>
</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
NOTE: When a review is added, you must calculate/re-calculate the average of all reviews and update the overallRating field in the main document to be the average of all the review ratings.

data/restaurants.js

In restaurants, you will create and export 5 methods. Create, Read (one for getting all and also one getting by id), Update, and Delete. You must do FULL error handling and input checking for ALL functions as you have in previous labs, checking if input is supplied, correct type, range etc. and throwing errors when you encounter bad input. You can use the functions you used for lab 4 however, you will need to create an update function. rename from lab 4 will not be used.

</div>
</div>
<div class="layoutArea">
<div class="column">
As a reminder, you will keep the same function names you used in lab 4:

</div>
</div>
</td>
</tr>
</tbody>
</table>
<div class="layoutArea">
<div class="column">
https://sit.instructure.com/courses/50148/assignments/273386

</div>
<div class="column">
3/12

</div>
</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
12/14/21, 11:46 PM Lab 6

<pre> create(name, location, phoneNumber, website, priceRange, cuisines, serviceOptions) Note: notice we no
longer pass overallRating into the function since that will be a computed field
getAll()
get(id)
</pre>
<pre>remove(id)
update (id, name, location, phoneNumber, website, priceRange, cuisines, serviceOptions)  Note: this is
the new function you will create
</pre>
For the functions you did in lab 4, all the same input requirements apply in this lab, for new update function, those requirements are stated below.

NOTE: For create: We no longer will need to pass in overallRating like we did in lab 4 since that will now be a computed average field of all ratings. When a restaurant is created, in your DB function, you will initialize the reviews array to be an empty array (since there can’t be reviews of a restaurant until the restaurant is in the system). You will also initialize overallRating to be 0 when a restaurant is created.

async update(id, name, location, phoneNumber, website,

priceRange, cuisines, serviceOptions)

This function will update all the data of the restaurant currently in the database.

If id, name, location, phoneNumber, website, priceRange, cuisines, serviceOptions are not provided at all, the method should throw. (All fields need to have valid values);

If id, name, location, phoneNumber, website, priceRange are not strings or are empty strings, the method should throw.

If phoneNumber does not follow this format: xxx-xxx-xxxx, the method will throw.

If website does not contain http://www. and end in a .com , and have at least 5 characters in-between

the http://www. and .com this method will throw.

If priceRange is not between ‘ $ ‘ to ‘ $$$$ ‘, this method will throw.

If cuisines is not an array and if it does not have at least one element in it that is a valid string , or are empty strings the method should throw.

If serviceOptions is not an object , the method should throw.

If serviceOptions.dineIn, serviceOptions.takeOut, serviceOptions.delivery are not in the object, the

method should throw.

If serviceOptions.dineIn, serviceOptions.takeOut, serviceOptions.delivery is not a boolean, the method should throw.

</div>
</div>
<div class="layoutArea">
<div class="column">
https://sit.instructure.com/courses/50148/assignments/273386 4/12

</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
12/14/21, 11:46 PM Lab 6

If the update succeeds, return the entire restaurant object as it is after it is updated.

data/reviews.js

In reviews.js, you will create and export 4 methods. Create, Read (one for getting all and also one getting by id), and Delete. You must do FULL error handling and input checking for ALL functions as you have in previous labs, checking if input is supplied, correct type, range etc. and throwing errors when you encounter bad input.

Function Names:

<pre> create(restaurantId, title, reviewer, rating, dateOfReview, review)
getAll(restaurantId)
get(reviewId)
remove(reviewId)
</pre>
async create(restaurantId, title, reviewer, rating, dateOfReview, review);

This async function will return to the newly created restaurant object, with all of the properties listed above.

If restaurantId, title, reviewer, rating, dateOfReview, review are not provided at all, the method should throw. (All fields need to have valid values);

If restaurantId, title, reviewer, dateOfReview, review are not strings or are empty strings, the method should throw.

If the restaurantId provided is not a valid ObjectId , the method should throw

If the restaurant doesn’t exists with that restaurantId , the method should throw

If rating is not a number that’s value is 1-5, the method will throw.

If dateOfReview is not a valid date string, the method will throw.

if dateOfReview is prior or after the current day’s date, the method should throw. (you can’t leave a review yesterday or before yesterday, and you can’t leave a review in the future)

Note: FOR ALL INPUTS: Strings with empty spaces are NOT valid strings. So no cases of ” ” are valid.

NOTE: When a review is added, you must calculate/re-calculate the average of all reviews and update the overallRating field in the main document to be the average of all the review ratings.

async getAll(restaurantId);

</div>
</div>
<div class="layoutArea">
<div class="column">
https://sit.instructure.com/courses/50148/assignments/273386 5/12

</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="section">
<div class="layoutArea">
<div class="column">
12/14/21, 11:46 PM Lab 6

</div>
</div>
<div class="section">
<div class="section">
<div class="layoutArea">
<div class="column">
This function will return an array of objects of the reviews given the . If there are no reviews for the restaurant, this function will return an empty array

If the restaurantId is not provided, the method should throw.

If the restaurantId provided is not a string, or is an empty string, the method should throw. If the restaurantId provided is not a valid ObjectId , the method should throw

If the restaurant doesn’t exists with that restaurantId , the method should throw.

async get(reviewId);

When given a reviewId , this function will return a review from the restaurant.

If the reviewId is not provided, the method should throw.

If the reviewId provided is not a string, or is an empty string, the method should throw. If the reviewId provided is not a valid ObjectId , the method should throw

If the review doesn’t exists with that reviewId , the method should throw.

async remove(reviewId):

This function will remove the review from the restaurant in the database.

If the reviewId is not provided, the method should throw.

If the reviewId provided is not a string, or is an empty string, the method should throw. If the reviewId provided is not a valid ObjectId , the method should throw

If the review doesn’t exists with that reviewId , the method should throw.

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>restaurantId
</pre>
</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
General note on all data functions: Whenever you return data that has an _id included in the returned data, return it as a string as shown in all the examples below. Do NOT return it as an ObjectId

NOTE: When a review is removed, you must calculate/re-calculate the average of all reviews and update the overallRating field in the main document to be the average of all the review ratings.

routes/restaurants.js

You must do FULL error handling and input checking for ALL routes! checking if input is supplied, correct type, range etc. and responding with proper status codes when you encounter bad input. All the input types, values and ranges that apply to the DB functions apply to the

</div>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
https://sit.instructure.com/courses/50148/assignments/273386

</div>
<div class="column">
6/12

</div>
</div>
</div>
</div>
<div class="page" title="Page 7">
<div class="section">
<div class="section">
<div class="layoutArea">
<div class="column">
12/14/21, 11:46 PM Lab 6

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre> GET /restaurants
</pre>
<pre>"restaurant_name"}
</pre>
<pre> POST /restaurants
</pre>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>{"_id": "restaurant_id", "name":
</pre>
</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
https://sit.instructure.com/courses/50148/assignments/273386 7/12

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>[{ "_id": "603d965568567f396ca44a72","name": "The Saffron Lounge"},{ "_id": "704f456673467g306fc44c3
4","name": "Black Bear"},.....]
</pre>
</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>{
    name: "The Saffron Lounge",
    location: "New York City, New York",
    phoneNumber: "123-456-7890",
    website: "http://www.saffronlounge.com",
    priceRange: "$$$$",
    cuisines: ["Cuban", "Italian" ],
    serviceOptions: {dineIn: true, takeOut: true, delivery: false}
</pre>
}

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
If the JSON provided does not match that schema, you will issue a 400 status code and end the request.

If the JSON is valid and the restaurant can be created successfully, you will return the newly created restaurant (as shown below) with a 200 status code.

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>{
    _id: "507f1f77bcf86cd799439011",
    name: "The Saffron Lounge",
    location: "New York City, New York",
    phoneNumber: "123-456-7890",
    website: "http://www.saffronlounge.com",
    priceRange: "$$$$",
    cuisines: ["Cuban", "Italian" ],
    overallRating: 0
    serviceOptions: {dineIn: true, takeOut: true, delivery: false}
    reviews: []
</pre>
}

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>GET /restaurants/{id}
</pre>
</div>
</div>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
<pre>GET /restaurants/
</pre>
</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
<pre>507f1f77bcf86cd799439011
</pre>
</div>
</div>
</td>
</tr>
</tbody>
</table>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
routes as well so you will do all the same checks in the routes that you do in the DB functions before sending the data to the DB function

Responds with an array of all restaurants in the format of

Note: Notice you are ONLY returning the restaurant ID as a string, and restaurant

name

Creates a restaurant with the supplied data in the request body, and returns the new restaurant (ALL FIELDS MUST BE PRESENT AND CORRECT TYPE).

You should expect the following JSON to be submitted in the request.body:

</div>
</div>
<div class="layoutArea">
<div class="column">
Example:

</div>
</div>
</div>
</div>
<div class="page" title="Page 8">
<div class="section">
<div class="layoutArea">
<div class="column">
12/14/21, 11:46 PM Lab 6

</div>
</div>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
Responds with the full content of the specified restaurant. So you will return all details of the restaurant. Your function should return the restaurant _id as a string, not an object ID

If no restaurant with that _id is found, you will issue a 404 status code and end the request.

You will return the restaurant (as shown below) with a 200 status code along with the restaurant data if found.

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
<pre>{
    _id: "507f1f77bcf86cd799439011",
    name: "The Saffron Lounge",
    location: "New York City, New York",
    phoneNumber: "123-456-7890",
    website: "http://www.saffronlounge.com",
    priceRange: "$$$$",
    cuisines: ["Cuban", "Italian" ],
    overallRating: 3.5
    serviceOptions: {dineIn: true, takeOut: true, delivery: false}
    reviews: [{_id: 609f1f77bcf86cd799439023, title: "Amazing" ,.... } ,.... ]
</pre>
}

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
<pre> PUT /restaurants/{id}
</pre>
Example:

This request will update a restaurant with information provided from the PUT body. Updates the specified restaurant by replacing the restaurant with the new restaurant content, and returns the updated restaurant. (All fields need to be supplied in the request.body, even if you are not updating all fields)

You should expect the following JSON to be submitted:

</div>
</div>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
<pre>PUT /restaurants/
</pre>
</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
<pre>507f1f77bcf86cd799439011
</pre>
</div>
</div>
</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
<pre>{
    name:  "Saffron Lounge",
    location: "SoHo, New York",
    phoneNumber: "123-456-1234",
    website: "http://www.thesaffronlounge.com",
    priceRange: "$$$",
    cuisines: ["Italian"],
    serviceOptions: {dineIn: false, takeOut: false, delivery:true }
</pre>
}

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
reviews should not be able to be modified in this route. You must copy the old array of review ids from the existing restaurant first and then insert them into the updated document so they are retained and not overwritten. You should also not modify or overwrite the overallRating field, so copy that as well.

If the JSON provided in the PUT body is not as stated above, fail the request with a 400 error and end the request.

</div>
</div>
<div class="layoutArea">
<div class="column">
If no restaurant exist with an _id of {id} , return a 404 and end the request.

</div>
</div>
</td>
</tr>
</tbody>
</table>
<div class="layoutArea">
<div class="column">
https://sit.instructure.com/courses/50148/assignments/273386

</div>
<div class="column">
8/12

</div>
</div>
</div>
</div>
<div class="page" title="Page 9">
<div class="section">
<div class="section">
<div class="layoutArea">
<div class="column">
12/14/21, 11:46 PM Lab 6

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
If the update was successful, then respond with that updated restaurant (as shown below) with a 200 status code

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>{
    _id: "507f1f77bcf86cd799439011",
    name: "Saffron Lounge",
    location: "SoHo, New York",
    phoneNumber: "123-456-1234",
    website: "http://www.thesaffronlounge.com",
    priceRange: "$$$",
    cuisines: ["Italian" ],
    overallRating: 3.5
    serviceOptions: {dineIn: false, takeOut: false, delivery: true}
</pre>
<pre>reviews: [{_id: 609f1f77bcf86cd799439023, title: "Amazing" ,.... } ,.... ]
}
</pre>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>DELETE /restaurants/{id}
</pre>
</div>
</div>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
<pre>DELETE /restaurants/
</pre>
</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
<pre>507f1f77bcf86cd799439011
</pre>
</div>
</div>
</td>
</tr>
</tbody>
</table>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>{"restaurantId": "507f1f77bcf86cd799439011", "deleted": true}.
</pre>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>GET /reviews/{restaurantId}
</pre>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>GET /reviews/
</pre>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>     306f1f77bcf86cd799431423
</pre>
<pre>restaurantId
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>restaurantId
</pre>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>[{
     _id: "603d992b919a503b9afb856e",
     title: "This place was great!",
     reviewer: "scaredycat",
</pre>
</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
ttps://sit.instructure.com/courses/50148/assignments/273386 9/12

</div>
</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
Example:

If no restaurant exists with an _id of {id} , return a 404 and end the request. Deletes the restaurant, sends a status code 200 and returns:

routes/reviews.js

You must do FULL error handling and input checking for ALL routes! checking if input is supplied, correct type, range etc. and responding with proper status codes when you encounter bad input. All the input types, values and ranges that apply to the DB functions apply to the routes as well so you will do all the same checks in the routes that you do in the DB functions before sending the data to the DB function

Example:

Getting this route will return an array of all reviews in the system for the specified restaurant id.

If no reviews for the are found, you will issue a 404 status code and end the request.

if the is not found in the system, you will issue a 404 status code and end the request

You will return the array of reviews (as shown below) with a 200 status code along with the review data if found.

</div>
</div>
<div class="layoutArea">
<div class="column">
h

</div>
</div>
</div>
</div>
<div class="page" title="Page 10">
<div class="section">
<div class="section">
<div class="layoutArea">
<div class="column">
12/14/21, 11:46 PM Lab 6

</div>
</div>
<div class="layoutArea">
<div class="column">
https://sit.instructure.com/courses/50148/assignments/273386

</div>
<div class="column">
10/12

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>     rating: 5,
     dateOfReview: "10/13/2021",
     review: "This place was great! the staff is top notch and the food was delicious!  They really
</pre>
<pre> know how to treat their customers"
}, .........
]
</pre>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>POST /reviews/{restaurantId}
</pre>
</div>
</div>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
<pre>POST /reviews/
</pre>
</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
<pre>306f1f77bcf86cd799431423
</pre>
</div>
</div>
</td>
</tr>
</tbody>
</table>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>{
  title: "This place was great!",
  reviewer: "scaredycat",
  rating: 5,
  dateOfReview: "10/13/2021",
  review: "This place was great! the staff is top notch and the food was delicious!  They really kno
</pre>
<pre>w how to treat their customers"
}
</pre>
</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
If the JSON provided does not match that schema, you will issue a 400 status code and end the request. if the restaurantId is not valid (it cannot be found), you will issue a 400 status code and end the request.

If the JSON is valid and the review can be created successful, you will return all the restaurant data showing the reviews (as shown below) with a 200 status code.

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>{
    _id: "306f1f77bcf86cd799431423",
    name: "Black Bear",
    location: "Hoboken, New Jersey",
    phoneNumber: "456-789-0123",
    website: "http://www.blackbear.com",
    priceRange: "$$",
    cuisines: ["Cuban", "American" ],
    overallRating: 4
    serviceOptions: {dineIn: true, takeOut: true, delivery: true}
    reviews: [
    {
</pre>
<pre>     _id: "603d992b919a503b9afb856e",
</pre>
<pre>     title: "This place was great!",
     reviewer: "scaredycat",
     rating: 5,
     dateOfReview: "10/13/2021",
     review: "This place was great! the staff is top notch and the food was delicious!  They really
</pre>
<pre> know how to treat their customers"
},....]
}
</pre>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>GET /reviews/review/{reviewId)
</pre>
</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
Example:

Creates a review sub-document with the supplied data in the request body, and returns the new

review (ALL FIELDS MUST BE PRESENT AND CORRECT TYPE).

You should expect the following JSON to be submitted in the request.body:

</div>
</div>
</div>
</div>
<div class="page" title="Page 11">
<div class="section">
<div class="layoutArea">
<div class="column">
12/14/21, 11:46 PM Lab 6

</div>
</div>
<div class="section">
<div class="section">
<div class="layoutArea">
<div class="column">
Example:

If no review with that _id is found, you will issue a 404 status code and end the request. You will return the review (as shown below) with a 200 status code.

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>GET /reviews/review/
</pre>
</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>603d992b919a503b9afb856e
</pre>
</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>{
     _id: "603d992b919a503b9afb856e",
     title: "This place was great!",
     reviewer: "scaredycat",
     rating: 5,
     dateOfReview: "10/13/2021",
     review: "This place was great! the staff is top notch and the food was delicious!  They really
</pre>
<pre> know how to treat their customers"
}
</pre>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>Delete /reviews/{reviewId)
</pre>
</div>
</div>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
<pre>DELETE /reviews/
</pre>
</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
<pre>603d992b919a503b9afb856e
</pre>
</div>
</div>
</td>
</tr>
</tbody>
</table>
<div class="layoutArea">
<div class="column">
reviewId

</div>
</div>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
<pre>{"reviewId": "
</pre>
</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
<pre>603d992b919a503b9afb856e
</pre>
</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
<pre>", "deleted": true}
</pre>
</div>
</div>
</td>
</tr>
</tbody>
</table>
<div class="layoutArea">
<div class="column">
<pre>overallRating
</pre>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
Example:

Deletes the specified review for the specified , sends a 200 status code and returns:

.

NOTE: If a review is deleted, you need to recalculate the average for the field in the main restaurant document

app.js

Your app.js file will start the express server on port 3000, and will print a message to the terminal once the server is started.

Tip for testing:

You should create a seed file that populates your DB with initial data for both restaurants and reviews. This will GREATLY improve your debugging as you should have enough sample data to do proper testing and it would be rather time consuming to enter a restaurants and reviews for that restaurant one by one through the API. A seed file is not required and is optional but is highly recommended. You should have a DB with at least 10 restaurants and multiple reviews for each restaurants for proper testing (again, this is not required, but it is to ensure you can test thoroughly.)

</div>
</div>
</div>
</div>
