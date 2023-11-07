# Ex.No:10 To create a option menu to display menu items.
## AIM
To create a option menu to display menu items using Android Studio.

## EQUIPMENTS REQUIRED
Latest Version Android Studio

## ALGORITHM
- Open Android Studio and then click on File -> New -> New project.
- Then type the Application name as HelloWorld and click Next.
- Then select the Minimum SDK as shown below and click Next.
- Then select the Empty Activity and click Next. Finally click Finish.
- Design layout in activity_main.xml.
- Display message give in MainActivity file.
- Save and run the application.

## PROGRAM
```
Program to print the text “optionmenu”.
Developed by : DYANESHWARAN D
Registeration Number : 212221040046
```
## activity_main.xml
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```

## MainActivity.java
```
package com.example.myapplication;

import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.view.Menu;
import android.view.MenuInflater;

public class MainActivity extends AppCompatActivity {
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }
    @Override
    public boolean onCreateOptionsMenu(Menu menu) {
        MenuInflater m = getMenuInflater();
        m.inflate(R.menu.option,menu);
        return true;
    }
}
```

## option.xml
```
<?xml version="1.0" encoding="utf-8"?>
<menu xmlns:android="http://schemas.android.com/apk/res/android">
    <item android:title="Item 1" />
    <item android:title="Item 2" />
    <item android:title="Item 3" />
</menu>
```
## OUTPUT
![image](https://github.com/dyanesh-100/MAD_EXP_10/assets/114641798/7a29dd5d-05be-48fc-8397-3958b2740402)
![image](https://github.com/dyanesh-100/MAD_EXP_10/assets/114641798/ba1564b0-5bad-4860-adab-58dff5d19b4e)

## RESULT
Thus a Simple Android Application to create a option menu to display menu items using Android Studio is developed and executed successfully.
