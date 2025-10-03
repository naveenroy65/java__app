# Java Hello World - Maven + Jenkins

This is a simple "Java Hello World application" built using "Maven".  
It is used to practice "CI/CD pipelines in Jenkins".



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

1. Create a "Freestyle Project" in Jenkins.
2. Configure "Source Code Management → Git" with:

   ```
   https://github.com/naveenroy65/java__app.git
   ```
3. Under "Build → Invoke top-level Maven targets", set:

   ```
   clean package
   ```
4. Save and click "Build Now".
5. Check "Console Output" for `BUILD SUCCESS`.

---

##  Next Steps

* Add "JUnit tests" under `src/test/java`
* Configure Jenkins to run:

  ```
  clean test
  ``
````
<br>
<br>
<img width="1566" height="564" alt="Screenshot 2025-10-03 200828" src="https://github.com/user-attachments/assets/617f33ff-4377-4181-b606-5659d8e59a38" />
<br>
<br>
<br>
<br>
<img width="1282" height="256" alt="Screenshot 2025-10-03 203151" src="https://github.com/user-attachments/assets/2ed5218c-276a-4505-a25e-57663e9731e7" />
<br>
<br>
<img width="1315" height="424" alt="Screenshot 2025-10-03 203217" src="https://github.com/user-attachments/assets/e260fb8f-9b18-4072-a940-b77aba2ebbc9" />
<br>
<br>
<img width="1338" height="852" alt="Screenshot 2025-10-03 203306" src="https://github.com/user-attachments/assets/d0398760-fc90-4daa-9db2-297c05ad5289" />
