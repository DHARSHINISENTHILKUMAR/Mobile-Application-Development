# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
Program to print for Android lifecycle.
Developed by:Dharshini S
Registeration Number :212221220009
```
## XML File:
```
   <?xml version="1.0" encoding="utf-8"?>
   <androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
   xmlns:app="http://schemas.android.com/apk/res-auto"
   xmlns:tools="http://schemas.android.com/tools"
   android:layout_width="match_parent"
   android:layout_height="match_parent"
   tools:context=".MainActivity">

   <TextView
       android:id="@+id/textView"
       android:layout_width="298dp"
       android:layout_height="90dp"
       android:layout_marginBottom="341dp"
       android:text="ACTIVITY CYCLE"
       android:textColor="@color/teal_200"
       android:textSize="36sp"
       app:layout_constraintBottom_toBottomOf="parent"
       app:layout_constraintEnd_toEndOf="parent"
       app:layout_constraintHorizontal_bias="0.588"
       app:layout_constraintStart_toStartOf="parent"
       app:layout_constraintTop_toBottomOf="@+id/imageView"
       app:layout_constraintVertical_bias="0.499" />

   <ImageView
       android:id="@+id/imageView"
       android:layout_width="92dp"
       android:layout_height="91dp"
       android:layout_marginBottom="32dp"
       android:src="@drawable/img"
       app:layout_constraintBottom_toTopOf="@+id/textView"
       app:layout_constraintEnd_toEndOf="parent"
       app:layout_constraintHorizontal_bias="0.498"
       app:layout_constraintStart_toStartOf="parent"
       app:layout_constraintTop_toTopOf="parent"
       tools:srcCompat="@tools:sample/avatars" />
       </androidx.constraintlayout.widget.ConstraintLayout>
```
## Main Activity:
```
    package com.example.activity_cycle;
    import androidx.appcompat.app.AppCompatActivity;
    import android.os.Bundle;
    import android.widget.Toast;

    public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(),"Oncreate",Toast.LENGTH_SHORT);
        toast.show();
    }
    protected void onStart(){
        super.onStart();
        Toast toast = Toast.makeText(getApplicationContext(),"Onstart",Toast.LENGTH_SHORT);
        toast.show();
    }
    protected void onPause(){
        super.onPause();
        Toast toast = Toast.makeText(getApplicationContext(),"Onpause",Toast.LENGTH_SHORT);
        toast.show();
    }
    protected void onResume(){
        super.onResume();
        Toast toast = Toast.makeText(getApplicationContext(),"onResume",Toast.LENGTH_SHORT);
        toast.show();
    }
    protected void onStop(){
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(),"OnStop",Toast.LENGTH_SHORT);
        toast.show();
    }
    protected  void onDestroy(){
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(),"onDestroy",Toast.LENGTH_SHORT);
        toast.show();
    }
    protected void onRestart(){
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(),"onRestart",Toast.LENGTH_SHORT);
        toast.show();
    }
    }
```

## OUTPUT
![image](https://github.com/DHARSHINISENTHILKUMAR/Mobile-Application-Development/assets/113699377/41b17892-04c0-4e70-a1a7-51198cfdcb39)

![image](https://github.com/DHARSHINISENTHILKUMAR/Mobile-Application-Development/assets/113699377/7658ccbb-a59d-4ed9-bbed-e757069e4877)

![image](https://github.com/DHARSHINISENTHILKUMAR/Mobile-Application-Development/assets/113699377/e4876a41-35e3-40f9-a9b2-0a8dc314a376)

![image](https://github.com/DHARSHINISENTHILKUMAR/Mobile-Application-Development/assets/113699377/a5711c1a-7711-4543-9e68-58e78a862ed0)

![image](https://github.com/DHARSHINISENTHILKUMAR/Mobile-Application-Development/assets/113699377/4723c956-9b87-4bd0-8709-efd2affac5b2)

![image](https://github.com/DHARSHINISENTHILKUMAR/Mobile-Application-Development/assets/113699377/cdad8411-d911-44fa-ad12-de68b5bcb428)

![image](https://github.com/DHARSHINISENTHILKUMAR/Mobile-Application-Development/assets/113699377/29759c7c-44d0-41f9-8ff9-0ab076831475)

![image](https://github.com/DHARSHINISENTHILKUMAR/Mobile-Application-Development/assets/113699377/0596374c-d459-495f-a61f-ce65da0a58dd)


## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
