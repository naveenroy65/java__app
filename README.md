# Java Hello World - Maven + Jenkins

This is a simple **Java Hello World application** built using **Maven**.  
It is used to practice **CI/CD pipelines in Jenkins**.



## 📂 Project Structure
```

java__app/
├── pom.xml
└── src/
└── main/
└── java/
└── HelloWorld.java

````

---

##  Prerequisites
- Java (JDK 8 or 11)
- Apache Maven (3.6+)
- Jenkins (if running CI/CD)

---

##  Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/naveenroy65/java__app.git
   cd java__app
````

2. Build the project:

   ```bash
   mvn clean package
   ```

3. Run the program:

   ```bash
   java -cp target/classes HelloWorld
   ```

Expected Output:

```
Hello, Jenkins + Maven!
```

---

##  Running in Jenkins

1. Create a **Freestyle Project** in Jenkins.
2. Configure **Source Code Management → Git** with:

   ```
   https://github.com/naveenroy65/java__app.git
   ```
3. Under **Build → Invoke top-level Maven targets**, set:

   ```
   clean package
   ```
4. Save and click **Build Now**.
5. Check **Console Output** for `BUILD SUCCESS`.

---

##  Next Steps

* Add **JUnit tests** under `src/test/java`
* Configure Jenkins to run:

  ```
  clean test
  ```


jay Sharma, to also add a **sample JUnit test** section into this README so your juniors know exactly how to extend Task 8 → Task 9?
```
