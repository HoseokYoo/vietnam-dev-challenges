# Description | Question 01

사용자 객체 목록에서 나이가 20 이상인 사용자들의 이름을 추출하고 출력하는 프로그램을 작성하세요.

Write a program to extract and print the names of users aged 20 or older from a list of user objects.

Viết một chương trình để trích xuất và in ra tên của những người dùng từ 20 tuổi trở lên từ danh sách các đối tượng người dùng.

Java 혹은 C# 코드로 작성하시오.

Write the code in either Java or C#.

Viết mã bằng Java hoặc C#.


```java
import java.util.Arrays;
import java.util.List;
import java.util.stream.Collectors;

public class Main {
    public static void main(String[] args) {
        // Create a list of user objects
        List<User> users = Arrays.asList(
            new User("Alice", 25),
            new User("Bob", 19),
            new User("Charlie", 30),
            new User("Diana", 18)
        );



        // Filter users aged 20 or older and extract their names
        // Write your code here


        // Print the result
        // Write your code here
    }
}

// Define the User class
class User {
    private String name;
    private int age;

    // Constructor to initialize name and age
    public User(String name, int age) {
        this.name = name;
        this.age = age;
    }

    // Getter method for the name
    public String getName() {
        return name;
    }

    // Getter method for the age
    public int getAge() {
        return age;
    }
}


```


```csharp
using System;
using System.Collections.Generic;
using System.Linq;

class Program {
    static void Main(string[] args) {
        // Create a list of user objects
        List<User> users = new List<User> {
            new User("Alice", 25),
            new User("Bob", 19),
            new User("Charlie", 30),
            new User("Diana", 18)
        };

        // Filter users aged 20 or older and extract their names
        
        var filteredNames = users.Where(user => user.Age >= 20).Select(user => user.Name).ToList();

        // Print the result

        filteredNames.ForEach(name => Console.WriteLine(name));
    }
}

class User {
    public string Name { get; set; }
    public int Age { get; set; }

    public User(string name, int age) {
        Name = name;
        Age = age;
    }
}



```
