# KangarooIMG
Javascript framework to create bouncing images on your website, quickly and easily.


Demo:
--------------


Setup:
--------------
First you need to implement the javascript and css files into your code. Add this to your code:

	<link href="kangarooimg.css" rel="stylesheet" type="text/css">
	<script src="kangarooimg.js"></script>

Next, you use javascript to call the one and only class in the framework, named **Kangaroo**. Add this to a variable to start preparing your first Kangaroo and give it a name and a ID name for the div it should be put in (This div will be added into the body by default). Like so:

	var kangaroo1 = new Kangaroo('Patrick', 'KangarooHuis');

**Kangaroo Class Paramaters**

| **Parameters** | **Type** | **Required**                              | **Description**   |
| -------------- | -------- | ----------------------------------------- | ----------------- |
|   *firstName*  | String   | Yes                 					    | Name of your Kangaroo.           |
|   *divName*    | String   | Yes                   					| Sets the id value of the div element that will be created around (future) Kangaroo divs.|
|  *parentName*  | String   | No (By default placed into body element.) | Selects the element id the div around the kangaroo elements will be placed in.  
|

Methods:
--------------
**createAvatar()**
| **Parameters** | **Type** | **Required** | **Description** |
| -------------- |--------- | ------------ | --------------- |
| *width*        | Int      | Yes          | Set width of image. |
| *height        | Int      | Yes          | Set height of image. |
| *source		 | String   | Yes          | Set url or file location of image. |

**speak()** (Requires createAvatar() method first.)
Displays a console log of your Kangaroo saying hello.

**speakOnClick()** (Requires createAvatar() method first.)
Displays an alert on leftclick of your Kangaroo saying hello.

**bounce()** (Requires createAvatar() method first.)
Makes your Kangaroo div element bounce up and down. 