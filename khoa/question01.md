# Description | Question 01

주어진 숫자 배열에서 짝수만 필터링하여 새로운 배열을 생성하고, 생성된 배열의 총합을 출력하는 프로그램을 작성하세요.

Write a program to filter only the even numbers from a given array of numbers, create a new array, and print the sum of the new array.

Viết một chương trình để lọc chỉ các số chẵn từ một mảng số đã cho, tạo một mảng mới và in tổng của mảng mới.


```typescript
// Define the input array
const numbers: number[] = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

// Filter even numbers and create a new array
// Write your code here
let new_arr=[10];
for(let i=0;i<numbers.length;i++){
    if(numbers%2==0){
        new_arr.push(numbers[i]);
    }
}
// Calculate the sum of the new array
// Write your code here
let sum=0;
for(let i=0;i<new_arr.length;i++){
    sum+=new_arr[i];
}

// Print the new array and its sum
// Write your code here
console.log("new array: ",new_arr);
console.log("sum of new array: ",sum);

```

