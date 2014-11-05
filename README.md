# Business Hours plugin for jQuery

[<img src="http://gendelf.github.io/jquery.businessHours/img/screen2.png" alt="business hours screenshot" />](http://gendelf.github.io/jquery.businessHours/)

[Demo](http://gendelf.github.io/jquery.businessHours/)

## Requirements

* [jQuery](http://jquery.com/) (>= 1.7)
* [jQuery timepicker](https://github.com/jonthornton/jquery-timepicker) (1.4.13)

## Bower

```
bower install -S jquery.business-hours
```

## Usage:

```JavaScript

/* initial data */
var operationTime = [
    {"isActive":false,"timeFrom":null,"timeTill":null},
    {"isActive":false,"timeFrom":null,"timeTill":null},
    {"isActive":false,"timeFrom":null,"timeTill":null},
    {"isActive":true,"timeFrom":"7:15","timeTill":"18:00"},
    {"isActive":true,"timeFrom":"9:00","timeTill":"18:00"},
    {"isActive":false,"timeFrom":null,"timeTill":null},
    {"isActive":false,"timeFrom":null,"timeTill":null}
    ];

$(selector).businessHours({
    operationTime: operationTime,           // list of JSON objects
    postInit:function() {                   // optional
        // post-init handler
    },
    checkedColorClass: "workingBusinssDay", // optional
    uncheckedColorClass: "dayOff",          // optional
    dayTmpl: " ... template content ..."    // optional
});
```

**Sponsored by**: [MVP engine](http://mvpngn.com)
