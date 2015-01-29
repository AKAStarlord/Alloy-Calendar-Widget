Alloy-Calendar-Widget
=====================

In the .xml file of you controller require widget like this.

 <Widget id="calendarContainer" src="Calendar"></Widget>

Use it in .js file like this.

$.calendarContainer.init({
    'callback' : dates
});

function dates(args) {
    Ti.API.info('current date : ' + args.date);
    Ti.API.info('current month : ' + args.month);
    Ti.API.info('current year : ' + args.year);
};

Everytime a date is selected dates function is called and dates can be accessed;
