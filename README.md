# Android_Libriary_List_Notes
List of Android Kotlin and Java Libraries used for building Application with Android Studio.

Created by PAPPU BISWAS<br>
Support My Youtube Channel : https://youtube.com/@bytenerd <br>
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

  ```
 implementation 'androidx.core:core-ktx:1.8.0'
    implementation 'androidx.appcompat:appcompat:1.5.0'
    implementation 'com.google.android.material:material:1.7.0'
    implementation 'androidx.constraintlayout:constraintlayout:2.1.4'
    implementation 'androidx.legacy:legacy-support-v4:1.0.0'
    testImplementation 'junit:junit:4.13.2'
    androidTestImplementation 'androidx.test.ext:junit:1.1.3'
    androidTestImplementation 'androidx.test.espresso:espresso-core:3.4.0'

    //roomdatabase
    implementation 'androidx.room:room-runtime:2.4.3'
    implementation 'androidx.room:room-ktx:2.4.3'
    kapt 'androidx.room:room-compiler:2.4.3'

    //jetPack Compose
    //implementation 'androidx.activity:activity-compose:1.5.1'
    //implementation 'androidx.compose.material:material:1.2.1'
    //implementation 'androidx.compose.animation:animation:1.2.1'
    //implementation 'androidx.compose.ui:ui-tooling:1.2.1'
    //implementation 'androidx.lifecycle:lifecycle-viewmodel-compose:2.5.1'
    //androidTestImplementation 'androidx.compose.ui:ui-test-junit4:1.2.1'

    //Compose Themes
    //implementation "com.google.android.material:compose-theme-adapter:1.1.16"
    //implementation "com.google.accompanist:accompanist-appcompat-theme:0.16.0"

    // Chart Lib
    //implementation 'com.github.PhilJay:MPAndroidChart:v3.1.0'

    // Photo Editor
    //implementation 'com.burhanrashid52:photoeditor:2.0.0'

    //PDF Viewer
    implementation 'com.github.barteksc:android-pdf-viewer:3.2.0-beta.1'

    //JSOUP HTML
    implementation 'org.jsoup:jsoup:1.15.1'

    //CSV
    implementation("com.github.doyaaaaaken:kotlin-csv-jvm:1.6.0")
    //implementation("com.github.doyaaaaaken:kotlin-csv-js:1.6.0")

    // Tensorflow lite
    //implementation 'org.tensorflow:tensorflow-lite:2.8.0'
    //  implementation 'org.tensorflow:tensorflow-lite-gpu:2.8.0'
    //  implementation 'org.tensorflow:tensorflow-lite-support:2.8.0'

    //Youtube
    implementation files('YouTubeAndroidPlayerApi.jar')

    //HTTP Client
    implementation "com.squareup.okhttp3:okhttp:4.9.2"
    implementation "com.android.volley:volley:1.2.1"

    //Saftey net
    implementation 'com.google.firebase:firebase-appcheck-safetynet:16.0.0'

    //Firebase Konnect
    implementation 'com.google.firebase:firebase-auth-ktx:21.0.7'
    implementation 'com.google.firebase:firebase-firestore-ktx:24.2.2'
    implementation 'com.google.firebase:firebase-database-ktx:20.0.5'
    implementation 'com.google.firebase:firebase-storage-ktx:20.0.1'

    //Lottie Animation
    implementation 'com.airbnb.android:lottie:3.4.0'

    //Status bar util
    implementation 'com.jaeger.statusbarutil:library:1.5.1'

    //GOOGLE
    implementation 'com.google.android.gms:play-services-auth:20.2.0'
    //implementation "com.google.android.gms:play-services-drive:20.2.0"

    //Glide Image
    implementation 'com.github.bumptech.glide:glide:4.12.0'
    annotationProcessor 'com.github.bumptech.glide:compiler:4.12.0'
    implementation ('com.github.bumptech.glide:okhttp3-integration:4.7.1'){
        exclude group: 'glide-parent'
    }

    //Fetch Andro
    implementation "androidx.tonyodev.fetch2:xfetch2:3.1.6"
    implementation "androidx.tonyodev.fetch2okhttp:xfetch2okhttp:3.1.6"

    //Ads
    implementation 'com.google.android.gms:play-services-ads:21.1.0'

    //Circular Image View
    implementation 'com.mikhaellopez:circularimageview:4.3.0'

    // Show Case View
    implementation 'com.elconfidencial.bubbleshowcase:bubbleshowcase:1.3.1'

    //Animated Bottom App Bar
    //implementation 'nl.joery.animatedbottombar:library:1.1.0'
    implementation 'com.gauravk.bubblenavigation:bubblenavigation:1.0.7'

    //Core Libriary
    implementation 'com.google.android.play:core:1.10.3'

    //Billing
    implementation("com.android.billingclient:billing:5.0.0")
    implementation("com.android.billingclient:billing-ktx:5.0.0")
```

---

# Data Formatting in Android Kotlin
<a href="https://github.com/pbgetwayscitech/Android_Libriary_List_Notes/blob/main/Date_formating_Kotlin.md"> Here </a>

---

# Single line Permission request for Android 

```
 val pb_requestPermissionLauncher =  registerForActivityResult( ActivityResultContracts.RequestPermission() ) { isGranted: Boolean -> }
```

Calling the object as 

```
pb_requestPermissionLauncher.launch(Manifest.permission.READ_EXTERNAL_STORAGE)
```

---

# Exo Video Player Libriary

```
    //Exoplayer
    // dependency for exoplayer
    implementation("com.google.android.exoplayer:exoplayer:r2.4.0")
    // for core support in exoplayer.
    implementation ("com.google.android.exoplayer:exoplayer-core:r2.4.0")
    // for adding dash support in our exoplayer.
    implementation ("com.google.android.exoplayer:exoplayer-dash:r2.4.0")
    // for adding hls support in exoplayer.
    implementation ("com.google.android.exoplayer:exoplayer-hls:r2.4.0")
    // for smooth streaming of video in our exoplayer.
    implementation ("com.google.android.exoplayer:exoplayer-smoothstreaming:r2.4.0")
    // for generating default ui of exoplayer
    implementation ("com.google.android.exoplayer:exoplayer-ui:r2.4.0")
```

---

  
