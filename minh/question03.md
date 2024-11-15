# Description | Question 03

주어진 부서와 급여 데이터를 포함하는 맵(Map)에서, 부서별 평균 급여를 계산하고 평균 급여가 5000 이상인 부서만 출력하는 프로그램을 작성하세요.

Write a program to calculate the average salary for each department from a map containing department and salary data, and print only the departments with an average salary of 5000 or higher.

Viết một chương trình để tính lương trung bình cho từng phòng ban từ một bản đồ chứa dữ liệu về phòng ban và lương, sau đó chỉ in ra các phòng ban có lương trung bình từ 5000 trở lên.

Java 혹은 C# 코드로 작성하시오.

Write the code in either Java or C#.

Viết mã bằng Java hoặc C#.


```java
import java.util.*;

public class Main {
    public static void main(String[] args) {
        // Create a map of department and salaries
        Map<String, List<Integer>> departmentSalaries = new HashMap<>();
        departmentSalaries.put("HR", Arrays.asList(4000, 5000));
        departmentSalaries.put("IT", Arrays.asList(6000, 8000));
        departmentSalaries.put("Finance", Arrays.asList(7000, 4000));
        departmentSalaries.put("Marketing", Arrays.asList(3000, 2000));

        // Calculate average salary for each department and filter
        // Write your code here

        // Print the result
        // Write your code here
    }
}
```


```csharp
using System;
using System.Collections.Generic;
using System.Linq;

class Program {
    static void Main(string[] args) {
        // Create a dictionary of department and salaries
        Dictionary<string, List<int>> departmentSalaries = new Dictionary<string, List<int>> {
            { "HR", new List<int> { 4000, 5000 } },
            { "IT", new List<int> { 6000, 8000 } },
            { "Finance", new List<int> { 7000, 4000 } },
            { "Marketing", new List<int> { 3000, 2000 } }
        };

        // Calculate average salary for each department and filter
        // Write your code here

        // Print the result
        // Write your code here
    }
}

```
