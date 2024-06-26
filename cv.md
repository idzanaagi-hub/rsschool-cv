# Anastasiya Morgunova 
idzanaagi@gmail.com

### About:

Hello, I'm a software tester with over a year of experience in the field. Throughout my career, I've had the opportunity to work in various testing roles, including SDET, manual QA, and auto QA. My ability to seamlessly transition between different stacks has been one of my key strengths, and I thrive on continuously learning and adapting to new technologies.

My passion for testing stems from my desire to make the world a little less buggy through my work. I'm currently delving into front-end development to do my job more efficiently and effectively. I'm also taking courses in test automation to improve my skills.

### Skills: 

* Java, JavaScript (TypeScript)

* Selenium, Selenide, Selenium Grid, Selenoid, Playwright

* JUnit, TestNG

* MySQL, PostreSQL, Cassandra

* Docker, Allure, Kibana, Postman

### Code Example:
```java
/*
The main idea is to count all the occurring characters in a string. If you have a string like aba, then the result should be {'a': 2, 'b': 1}.
What if the string is empty? Then the result should be empty object literal, {}.
*/
public class Kata {
    public static Map<Character, Integer> count(String str) {
       if (str.isEmpty()) {
            return new LinkedHashMap<>();
        }
        List<String> arrayList = Arrays.stream(str.split("")).toList();
        List<String> distinct = Arrays.stream(str.split("")).sorted().distinct().toList();
        Map<Character, Integer> result = new LinkedHashMap<>();
        for (int i = 0; i < distinct.size(); i++) {
            int finalI = i;
            int count = arrayList.stream().filter(item -> Objects.equals(item, distinct.get(finalI))).toArray().length;
            result.put(distinct.get(i).charAt(0), count);
        }
        return result;
    }
}
```

```typescript
/*
Write a function that will take the number of petals of each flower and return true if they are in love and false if they aren't.
*/
export function lovefunc(flower1: number, flower2: number): boolean {
    return flower1 % 2 === 0 && flower2 % 2 !== 0 || flower1 % 2 !== 0 && flower2 % 2 === 0
}
```

### Work Experience (1 year and 3 months):

* Fullstack QA Engineer | High-Volume Financial Marketplace

* Auto QA Engineer | Cybersecurity System

### Education (Courses):

* Hexlet: frontend-developer

* SimbirSoft: SDET workshop

* OTUS: JavaScript QA Engineer (in progress)

### English:

A2-B1