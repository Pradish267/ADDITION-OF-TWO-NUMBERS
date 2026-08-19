# ADDITION-OF-TWO-NUMBERS
## Aim:
To create and design an addition of two numbers using android studio.
## EQUIPMENTS REQUIRED:
Android Studio(Latest Version)
## ALGORITHM:
Step 1: Open Android Studio and create a New Project using Empty Views Activity.

Step 2: Design the layout with two EditText boxes, one Button, and one TextView for the result.

Step 3: Give suitable IDs to all the UI components.

Step 4: Open MainActivity.java and connect the UI components using their IDs

Step 5: Get the two input values, convert them into numbers, and add them.

Step 6:Display the calculated sum in the result TextView when the Add button is clicked.

Step 7: Run the application, enter two numbers, click Add, and verify the result.
## PROGRAM:
Program to create and design an android application simple calculator using Intent.
### Developed by: PRADISH PRIYAN S P
### Register Number :212225230210

## AndroidMainfest.xml
```
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    android:padding="30dp">

    <EditText
        android:id="@+id/num1"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:hint="Enter first number"
        android:inputType="numberDecimal" />

    <EditText
        android:id="@+id/num2"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:hint="Enter second number"
        android:inputType="numberDecimal" />

    <Button
        android:id="@+id/addButton"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="ADD" />

    <EditText
        android:id="@+id/result"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:hint="Result"
        android:focusable="false"
        android:inputType="numberDecimal" />

</LinearLayout>
```
## MainActivity.java
```
package com.example.additionoftwo;

import android.os.Bundle;
import android.widget.Button;
import android.widget.EditText;

import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

    EditText num1, num2, result;
    Button addButton;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        num1 = findViewById(R.id.num1);
        num2 = findViewById(R.id.num2);
        result = findViewById(R.id.result);
        addButton = findViewById(R.id.addButton);

        addButton.setOnClickListener(v -> {

            double n1 = Double.parseDouble(num1.getText().toString());
            double n2 = Double.parseDouble(num2.getText().toString());

            double sum = n1 + n2;

            result.setText("" + sum);
        });
    }
}
```
### output
<img width="1913" height="1079" alt="Screenshot 2026-08-19 112825" src="https://github.com/user-attachments/assets/06b4dec1-b94d-4ffe-af93-1d3d23ab70ba" />

<img width="1919" height="1078" alt="Screenshot 2026-08-19 112836" src="https://github.com/user-attachments/assets/69e69ee9-7748-4115-9aa6-1a4a7b30d9b2" />

## RESULT
Thus the Addition of two numbers successfully performed and displayed in the text box.

