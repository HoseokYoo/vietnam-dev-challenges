# Description | Question 02

주문 객체 목록에서 동일한 상품의 총합을 계산하고 상품 이름과 합계를 출력하는 프로그램을 작성하세요.

Write a program to calculate the total quantity for each product from a list of order objects and print the product name with its total quantity.

Viết một chương trình để tính tổng số lượng cho mỗi sản phẩm từ danh sách các đối tượng đơn hàng và in tên sản phẩm với tổng số lượng.

Java 혹은 C# 코드로 작성하시오.

Write the code in either Java or C#.

Viết mã bằng Java hoặc C#.

```java
import java.util.Arrays;
import java.util.List;
import java.util.Map;
import java.util.stream.Collectors;

public class Main {
    public static void main(String[] args) {
        // Create a list of order objects
        List<Order> orders = Arrays.asList(
            new Order("Apple", 3),
            new Order("Banana", 2),
            new Order("Apple", 1),
            new Order("Orange", 5),
            new Order("Banana", 4)
        );

        // Group by product name and calculate the total quantity
        // Write your code here

        // Print the result
        // Write your code here
    }
}

// Define the Order class
class Order {
    private String productName;
    private int quantity;

    // Constructor to initialize product name and quantity
    public Order(String productName, int quantity) {
        this.productName = productName;
        this.quantity = quantity;
    }

    // Getter method for the product name
    public String getProductName() {
        return productName;
    }

    // Getter method for the quantity
    public int getQuantity() {
        return quantity;
    }
}


```


```csharp

using System;
using System.Collections.Generic;
using System.Linq;

class Program {
    static void Main(string[] args) {
        // Create a list of order objects
        List<Order> orders = new List<Order> {
            new Order("Apple", 3),
            new Order("Banana", 2),
            new Order("Apple", 1),
            new Order("Orange", 5),
            new Order("Banana", 4)
        };

        // Group by product name and calculate the total quantity
        var groupOrders = orders
        .GroupBy(o => o.ProductName)
        .Select(g => new {
            ProductName = g.Key,
            TotalQuantity = g.Sum(o => o.Quantity)
        });

        // Print the result
        foreach (var order in groupOrders) {
            Console.WriteLine($"Product: {order.ProductName}, Total Quantity: {order.TotalQuantity}")
    }
}
}

class Order {
    public string ProductName { get; set; }
    public int Quantity { get; set; }

    public Order(string productName, int quantity) {
        ProductName = productName;
        Quantity = quantity;
    }
}

```
