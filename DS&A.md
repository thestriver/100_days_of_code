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

---
Validate Subsequence
<pre>
function isValidSubsequence(array, sequence) {
  // Write your code here.
	let seqIndex = 0;

	for (const value of array){
		if(seqIndex === sequence.length) break;
		if (sequence[seqIndex] === value) seqIndex++;
	}
	return seqIndex === sequence.length
}
</pre>