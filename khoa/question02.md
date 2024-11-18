# Description | Question 02

주어진 학생 객체 배열에서, 평균 점수가 80 이상인 학생의 이름만 추출하여 출력하는 프로그램을 작성하세요.

Write a program to extract and print the names of students with an average score of 80 or higher from a given array of student objects.

Viết một chương trình để trích xuất và in ra tên của các học sinh có điểm trung bình từ 80 trở lên từ một mảng đối tượng học sinh.

```typescript
// Define the Student type
type Student = {
    name: string;
    scores: number[];
};

// Create an array of students
const students: Student[] = [
    { name: "Alice", scores: [85, 90, 78] },
    { name: "Bob", scores: [70, 75, 80] },
    { name: "Charlie", scores: [90, 85, 95] },
    { name: "Diana", scores: [60, 70, 65] }
];

// Calculate the average score and filter students
// Write your code here
for(var i=0;i<students.length;i++){
    students[i].avg_score = ((students[i].scores[0]+students[i].scores[1]+students[i].scores[2])/3);
}

// Print the names of students with an average score >= 80
// Write your code here
for(var i=0;i<students.length;i++){
   if( students[i].avg_score>=80){
    console.log(students[i]);
   }
}
```

