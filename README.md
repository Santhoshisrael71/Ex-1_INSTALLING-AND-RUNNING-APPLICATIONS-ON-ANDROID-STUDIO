# EX-1: INSTALLING AND RUNNING APPLICATIONS ON ANDROID STUDIO

**Name:** Santhosh P

**Register Number:** 212224220088

## Software Requirements
- Android Studio
- Android SDK
- Android Virtual Device (AVD)
- Java
- XML

---

## Step 1 – System Requirements

The required software tools are used to develop, design, and run Android applications. Android Studio provides the development environment, Java is used to implement application functionality, and XML is used to design the user interface.

### Required Software
- Android Studio
- Java Development Kit (JDK)
- Android SDK
- Android Emulator

---

## Step 2 – Setup Android Studio

Android Studio is the official Integrated Development Environment (IDE) used for Android application development.

### Installation Procedure
1. Download Android Studio from the official website.
2. Run the installer and follow the installation instructions.
3. Install the required Android SDK components.
4. Configure the Android SDK location.
5. Set up the Android Virtual Device if required.
6. Launch Android Studio.
7. Create a new Android project using the Empty Views Activity template.
8. Select Java as the programming language.

---

## Creating the Student Details Application

1. Open the project in Android Studio.
2. Design the user interface using the `activity_main.xml` file.
3. Add a heading named **STUDENT DETAILS**.
4. Add a button to reveal the student information.
5. Add a TextView to display the student name and register number.
6. Open the `MainActivity.java` file.
7. Initialize the Button and TextView using `findViewById()`.
8. Implement the button click event using `setOnClickListener()`.
9. Display the student information when the button is clicked.
10. Change the button text to **Details Revealed** after displaying the information.

---

## Step 3 – Create Android Virtual Device (AVD)

An Android Virtual Device is used to test and run the application without requiring a physical Android phone.

### Procedure
1. Open Device Manager in Android Studio.
2. Click **Create Virtual Device**.
3. Select a suitable device configuration.
4. Select and download an Android system image if required.
5. Finish the configuration and start the emulator.
6. Select the emulator from the device dropdown menu.

---

## Step 4 – Run the Application

1. Open the Student Details project.
2. Select the configured Android Emulator.
3. Click the **Run ** button in Android Studio.
4. Wait for the application to build and launch.
5. Verify that the Student Details screen appears.
6. Click the button to display the student information.

---

## Application Display Program ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to print the text “Hello World”.
Developed by: Santhosh P
Registeration Number : 212224220088
*/
```
### MainActivity.Java

```
package com.example.myapplication;

import android.os.Bundle;
import android.widget.Toast;

import androidx.activity.EdgeToEdge;
import androidx.appcompat.app.AppCompatActivity;
import androidx.core.graphics.Insets;
import androidx.core.view.ViewCompat;
import androidx.core.view.WindowInsetsCompat;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);

        setContentView(R.layout.activity_main);
        Toast toast= Toast.makeText(getApplicationContext(),"OnCreated Executed",Toast.LENGTH_LONG);
        toast.show();

    }
    protected void onStart(){
        super.onStart();
        Toast toast= Toast.makeText(getApplicationContext(),"OnStart Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onResume(){
        super.onResume();
        Toast toast= Toast.makeText(getApplicationContext(),"OnResume Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onPause(){
        super.onPause();
        Toast toast= Toast.makeText(getApplicationContext(),"onPause Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStop(){
        super.onStop();
        Toast toast= Toast.makeText(getApplicationContext(),"onStop Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onRestart(){
        super.onRestart();
        Toast toast= Toast.makeText(getApplicationContext(),"onRestart Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onDestroy(){
        super.onDestroy();
        Toast toast= Toast.makeText(getApplicationContext(),"onDestroy Executed",Toast.LENGTH_LONG);
        toast.show();
    }
}
```

### Activity_main.xml

```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Helllo World"
        android:textAppearance="@style/TextAppearance.AppCompat.Body2"
        android:textColor="#DE2323"
        android:textSize="24sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/textView2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Life Cycle Methods in Android"
        android:textColor="#20C338"
        android:textSize="24sp"
        android:textStyle="bold|italic"
        android:visibility="visible"
        app:layout_constraintBottom_toTopOf="@+id/textView"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>
```



## Output

<img width="1920" height="1080" alt="Screenshot (8)" src="https://github.com/user-attachments/assets/a280f0e8-5900-4e76-970c-60534df064f3" />





## Result

Thus, the Student Details application was successfully created and executed using Android Studio, and the content information was displayed .
