```js
    function plusMinus(arr) {
    // Write your code here

    // initialize values to zero
    let positives = 0;
    let negatives = 0;
    let zeros = 0;

    //use for loop to add to positives, negatives, and zeros sum
    for (let i=0; i<arr.length; i++){
        if (arr[i] > 0){
            positives++;
        }
        else if (arr[i] < 0){
            negatives++;
        }
        else{
            zeros++;
        }
    }

    // create ratio by dividing the values by the array length
    positives /= arr.length;
    negatives /= arr.length;
    zeros /= arr.length;

    //use toFixed method to use 6 decimal places
    console.log(positives.toFixed(6));
    console.log(negatives.toFixed(6));
    console.log(zeros.toFixed(6));
    }
    ```