```js
    function timeConversion(s) {
        // Write your code here

        //check if the string includes A at the 8th index
        if (s[8] === 'A'){
            if(s[0] === '1' && s[1] === '2'){
                return '00' + s.substring(2,s.length - 2);
                //if the string starts with 12, and is in the AM, the 24 hour clock should return 00:00 + how ever many minutes are on the clock
            }
        return s.substring(0,s.length-2);
        // else return the same time without the letters at the end since it is am. (04:00 am = 04:00)
        }

        // else it is PM
        else { 
            let hour = parseInt(s.substring(0,2));
            if (hour === 12){
                // if the hour is 12, it is 12pm and doesn't need to be converted
                return s.substring(0,s.length - 2)
                //cut off the last two indexes of the string (ie. PM)
            }
            //otherwise add 12 to convert it into military time
            hour += 12;
            return hour + s.substring(2,s.length - 2); 
        }   
    }
```