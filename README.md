# Codewars-Challenge
<br>
I solved this after getting confused about the math for a few minutes. I had to search up the method to get the nth root of a number.

We have the number 12385. We want to know the value of the closest cube but higher than 12385. The answer will be 13824.

Now, another case. We have the number 1245678. We want to know the 5th power, closest and higher than that number. The value will be 1419857.

We need a function find_next_power ( findNextPower in JavaScript, CoffeeScript and Haskell), that receives two arguments, a value val, and the exponent of the power, pow_, and outputs the value that we want to find.

```javascript
function findNextPower(val, pow_) {
    //your code here
    let cubedValue = Math.pow(val, 1/pow_)
    console.log(cubedValue)
    let roundedValue = Math.round(cubedValue)
    while(roundedValue < cubedValue){
        return (roundedValue + 1) ** pow_
    }
    return roundedValue ** pow_

}

```
 
