# Android_Libriary_List_Notes
List of Android Kotlin and Java Libraries used for building Application with Android Studio.

Created by PAPPU BISWAS<br>
Follow Me on Linked In : https://linkedin.com/in/mr-pappubiswas

---

<h1> Room Libriary for SQL Data Management </h1>
<h3> - Module app under plugins kotlin</h3>

  ```
  id("com.google.devtools.ksp")
  id("kotlin-android")
  id("kotlin-kapt")
  ```
<h3> - Module Project under plugins kotlin</h3>

```
id("com.google.devtools.ksp") version "1.5.31-1.0.0" apply false
```

<h3> - Dependencies </h3>

  ```
  implementation("androidx.room:room-runtime:2.6.0")
  ksp("androidx.room:room-compiler:2.6.0")  // ksp is for kotline new version
  annotationProcessor("androidx.room:room-compiler:2.6.0") // annotattionrpcessor is for java
  ```


  ---

  
