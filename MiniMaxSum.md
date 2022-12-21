```js
    function miniMaxSum(arr) {
    // Write your code here
    arr.sort()
    // sort array in ascending order, that way if summing from the lowest number to the
    // second 2 last, you will return the minimum sum
    let minSum =0;
    let maxSum = 0;
    for(let i=0; i<arr.length - 1; i++){
        minSum += arr[i];
    }
    // sum the numbers from the second index to the final index to return the maximum sum
    for(let i=1; i<arr.length; i++){
        maxSum += arr[i];
    }
    console.log(minSum + " " + maxSum)
    }
```