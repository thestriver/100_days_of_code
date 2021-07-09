## Coding Interview Questions

## Arrays

Two Number Sum

<pre>function twoNumberSum(array, targetSum) {
   const nums = {};
   for (const num of array){
   const y = targetSum - num
   //array.includes(y)
   if ( y in nums ) {
   return [y, num]
   } else {
   nums[num] = true;
   }
   }
   return [];
   }
   o(n) T & o(n) S
</pre>