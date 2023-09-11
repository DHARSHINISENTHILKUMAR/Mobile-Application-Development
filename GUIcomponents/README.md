# Ex.No: 2 To develop an application that uses GUI Components with Fonts and Colors. 
Note: Create button for colors and fonts while clicking color or font button should change 


## AIM:

To create an application that uses GUI Components with Fonts and Colors using Android Studio.

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
Program to print the text “GUIcomponent”.
Developed by: Dharshini S
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

    <Button
        android:id="@+id/colbut"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="128dp"
        android:layout_marginTop="120dp"
        android:backgroundTint="#FFC107"
        android:text="Change Color"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <Button
        android:id="@+id/fonbut"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="132dp"
        android:layout_marginTop="48dp"
        android:backgroundTint="#FF5722"
        android:text="Change Font"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/colbut" />

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="48dp"
        android:layout_marginTop="152dp"
        android:text="PRIME PLAYS"
        android:textSize="40dp"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/fonbut" />
    </androidx.constraintlayout.widget.ConstraintLayout>
```
## Main Activity:
```
    package com.example.guicomps;

    import androidx.appcompat.app.AppCompatActivity;

    import android.content.res.AssetManager;
    import android.graphics.Color;
    import android.graphics.Typeface;
    import android.os.Bundle;
    import android.view.View;
    import android.widget.Button;
    import android.widget.TextView;

    import java.io.IOException;
    import java.io.InputStream;

    public class MainActivity extends AppCompatActivity implements View.OnClickListener {

    private TextView textView;
    private Button colorButton;
    private Button fontButton;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        textView = findViewById(R.id.textView);
        colorButton = findViewById(R.id.colbut);
        fontButton = findViewById(R.id.fonbut);

        colorButton.setOnClickListener(this);
        fontButton.setOnClickListener(this);
    }

    @Override
    public void onClick(View view) {
        switch (view.getId()) {
            case R.id.colbut:
                changeTextColor();
                break;
            case R.id.fonbut:
                changeFont();
                break;
        }
    }

    private void changeTextColor() {
        int randomColor = generateRandomColor();
        textView.setTextColor(randomColor);
    }

    private void changeFont() {
        Typeface newFont = Typeface.createFromAsset(getAssets(), "font/pacifico.ttf");
        textView.setTypeface(newFont);
    }

    private int generateRandomColor() {
        int red = (int) (Math.random() * 256);
        int green = (int) (Math.random() * 256);
        int blue = (int) (Math.random() * 256);
        return Color.rgb(red, green, blue);
    }
    }
```



## OUTPUT
![image](https://github.com/DHARSHINISENTHILKUMAR/Mobile-Application-Development/assets/113699377/555267ee-5b7a-416b-99fb-665086a382c0)

![image](https://github.com/DHARSHINISENTHILKUMAR/Mobile-Application-Development/assets/113699377/afb2ec4c-0422-437b-a202-643f3e7f3907)

![image](https://github.com/DHARSHINISENTHILKUMAR/Mobile-Application-Development/assets/113699377/44a55a3b-4331-4c72-be1b-aada7506ce03)

![image](https://github.com/DHARSHINISENTHILKUMAR/Mobile-Application-Development/assets/113699377/c0bf76e3-e262-4995-8493-e44e002050a5)

![image](https://github.com/DHARSHINISENTHILKUMAR/Mobile-Application-Development/assets/113699377/0d272efc-5b67-4a95-8222-509cc417aabb)

![image](https://github.com/DHARSHINISENTHILKUMAR/Mobile-Application-Development/assets/113699377/0afcc57e-5b95-42b4-a603-86ba761722d0)

![image](https://github.com/DHARSHINISENTHILKUMAR/Mobile-Application-Development/assets/113699377/fb41b2e5-b191-44b9-9bc6-3641c89569bc)

![image](https://github.com/DHARSHINISENTHILKUMAR/Mobile-Application-Development/assets/113699377/09f8a9d0-2e22-4515-b548-4bd0808e6575)

![image](https://github.com/DHARSHINISENTHILKUMAR/Mobile-Application-Development/assets/113699377/baa009ab-e441-4124-b5ff-c1de500322ea)

![image](https://github.com/DHARSHINISENTHILKUMAR/Mobile-Application-Development/assets/113699377/35f252a4-6247-4b38-b81f-25149ebdc57b)

![image](https://github.com/DHARSHINISENTHILKUMAR/Mobile-Application-Development/assets/113699377/1bc1cc9a-67a3-4d4d-b009-ac4e1bc026d9)

## RESULT
Thus a Simple Android Application that uses GUI Components with Fonts and Colors using Android Studio is developed and executed successfully.


