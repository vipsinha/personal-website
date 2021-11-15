---
title: "C++ Notes"
published: true
---

**Hello everyone**, this is myblog post on C++ and its knowledge.

I hope you like it!

# Standard library
## std::accumulate

It is use to provide the sum, multiply, etc. I t usually takes pointers as input
```c++
/*example 1*/
int sum = std::accumulate(v.begin(), v.end(), 0);

/*example 2*/
int product = std::accumulate(v.begin(), v.end(), 1, std::multiplies<int>());

/*example 3*/
class Employee {
/** All kinds of data: name, ID number, phone, email address... */
public:
 int monthlyPay() const;
};

/** Simple class defining how to add a single Employee's
 *  monthly pay to our existing tally */
auto accumulate_func = [](int accumulator, const Employee& emp) {
   return accumulator + emp.monthlyPay();
 };

// And here's how you call the actual calculation:
int TotalMonthlyPayrollCost(const vector<Employee>& V)
{
 return std::accumulate(V.begin(), V.end(), 0, accumulate_func);
}
```

## std::ceil
To get the ceiling value of any data
```c++
/*example 1*/
// to get the centuary of the year
int solution(int year) {
    int century;
    if(year%100){
        century = std::ceil(year/100) + 1; 
    }else{
        century = std::ceil(year/100); 
    }
    
    return century;
}

/*example 2*/
std::ceil(5/4) = 2 
std::ceil(10/2) = 5 
```

## Java
```java
public class java {
    public static void main(String[] args) {
        System.out.println("Hello World");
    }
}
```

## HTML
```html
<html>
  <head><title>Title!</title></head>
  <body>
    <p id="foo">Hello, World!</p>
    <script type="text/javascript">var a = 1;</script>
    <style type="text/css">#foo { font-weight: bold; }</style>
  </body>
</html>
```

## Console
```console
# prints "hello, world" to the screen
~# echo Hello, World
Hello, World

# don't run this
~# rm -rf --no-preserve-root /
```

## Css
```css
body {
    font-size: 12pt;
    background: #fff url(temp.png) top left no-repeat;
}
```

## Yaml
```yaml
---
one: Mark McGwire
two: Sammy Sosa
three: Ken Griffey
```
