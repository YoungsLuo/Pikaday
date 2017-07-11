Pikatime 
========


### A refreshing JavaScript Timepicker based on Datepicker

* Lightweight (less than 5kb minified and gzipped)
* No dependencies (but plays well with [Moment.js][moment])
* Modular CSS classes for easy styling


![Pikatime Screenshot][Pikatime-image]

## Usage

**Pikatime** use like **Datepicker**, just add some options:

```json
default = {
	isTimePicker: true,
	format: 'YYYY-MM-DD HH:mm:ss',
	timelabelWidth: 55,  	 //label width for different language, defualt for Eng
	i18n: {
       hours: 'hours',
       minutes: 'minutes',
       seconds: 'seconds'
    },
}
	
```

can be bound to an input field:

```html
<input type="text" id="timepicker">
```

Add the JavaScript to the end of your document:

```html
<script src="pikaday.js"></script>
<script>
    var picker = new Pikaday({ 
    	field: document.getElementById('timepicker'), 
    	isTimepicker: true, format: 'YYYY-MM-DD HH:mm:ss', 
    	timelabelWidth: 55, 
    	i18n: {
            previousMonth : 'Previous Month',
            nextMonth     : 'Next Month',
            months        : ['January','February','March','April','May','June','July','August','September','October','November','December'],
            weekdays      : ['Sunday','Monday','Tuesday','Wednesday','Thursday','Friday','Saturday'],
            weekdaysShort : ['Sun','Mon','Tue','Wed','Thu','Fri','Sat'],
            hours: 'hours',
            minutes: 'minutes',
            seconds: 'seconds'
        },
    });
</script>
```

[Pikatime-image]: https://ws4.sinaimg.cn/large/006tNc79gy1fhfr2w2l0aj307408haab.jpg