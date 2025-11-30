# Shopping List App 

## Overview
This project is an Android application built with **Kotlin** and **Jetpack Compose** that stores shopping list items in a local database using **Room**.  
Each item includes:
- Name  
- Quantity  
- Unit of measurement  
- Price  

The app displays items in a scrollable list and supports adding, editing, and deleting entries. Data persistence is handled with Room, and the **Database Inspector** can be used to verify stored data.


##  Features
- Add new shopping items with name, quantity, unit, and price.  
- Display items in a structured list using **LazyColumn**.  
- Edit and delete items (optional feature implemented).  
- Persistent storage with **Room SQLite database**.  
- Reactive UI updates with **ViewModel** and **Jetpack Compose**.  

## Tech Stack
- **Kotlin**  
- **Jetpack Compose**  
- **Room Database**  
- **MVVM Architecture**  
- **Database Inspector** (for debugging and verification)  

```kotlin
plugins {
    id("com.google.devtools.ksp")
}

dependencies {
    implementation("androidx.lifecycle:lifecycle-runtime-ktx:2.6.2")
    implementation("androidx.lifecycle:lifecycle-viewmodel-compose:2.6.2")
    implementation("androidx.room:room-runtime:2.6.1")
    implementation("androidx.room:room-ktx:2.6.1")
    ksp("androidx.room:room-compiler:2.6.1")
    annotationProcessor("androidx.room:room-compiler:2.6.1")
}
```

In **build.gradle.kts (Project)**:
```kotlin
id("com.google.devtools.ksp") version "2.0.21-1.0.27" apply false
```

---

## Example Output
```
Name: Orange Juice
Quantity: 2 liter
Price: €2.5
```

---

## ✅ Conclusion
This app demonstrates how to integrate **Room database** with **Jetpack Compose** to build a modern Android application. It fulfills the assignment requirements by storing shopping list items locally, displaying them in a structured list, and supporting CRUD operations.
