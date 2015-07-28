dm_notify.js
---------------------------------------------------


A Light jQuery notification plugin. For websites and mobile apps


## Installation

Dependency: [jQuery](http://jquery.com)

Download dm_notify.js:
- from [Github](https://github.com/mastavralis/dm-notify.git)

Add a `div with id #dm-notif` ti will hold all the notifications :

    <div id="dm-notif"></div>

### Styling

Furthermore, ohSnap.js creates a div with classes `.alert .alert-color` so you will want to have something like :
The plugin creates a div with the classes ' .dm-notification .dm-notify-red .dm-notify-green .dm-notify-blue .dm-notify-yellow .dm-notify-orange ' so copy and paste it to your stylesheet.

/* NOTIFICATIONS BASED ON BOOTSTRAP*/
.dm-notification {
	text-align: right;
  	margin-top: 5px;
  	padding: 15px;
  	border: 1px solid #eed3d7;
  	border-radius: 4px;
  	float: right;
  	clear: right;
}

.dm-notify-red {
  color: white;
  background-color: #DA4453;
}
.dm-notify-green {
  color: white;
  background-color: #37BC9B;
}
.dm-notify-blue {
  color: white;
  background-color: #4A89DC;
}
.dm-notify-yellow {
  color: white;
  background-color: #F6BB42;
}
.dm-notify-orange {
  color:white;
  background-color: #E9573F;
}

ul li:hover {
	cursor:pointer;
}

How to use it:
-----

Call a notification, with the function ' dm_notification(text, color, time, icon); ' Examples :

    dm_notification('Ooops! The is a problem with your details', 'red', 'icon class from bootstrap');
    dm_notification('Your request was submitted succesfully', 'blue');
	
You can alway create a custom color by adding classes in the css file like: ' .dm-notify-royalblue ' ;

To close a notification, call  the function ' dm_notification_close() '.

When a notification is clicked, it will close automatically regardless the specified time.

Developed by 
- Dionisis Mastavralis -
