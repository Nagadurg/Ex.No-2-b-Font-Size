
# Ex.No:2 Develop an application that uses Font Size using Android Studio.


## AIM:
To develop an application that uses Font Size using android studio.

## EQUIPMENTS REQUIRED:

Android Studio(Min. required Artic Fox)


## ALGORITHM:
Step 1: Create a New Android Project:
              • Click New in the toolbar.
              • In the window that appears, open the Android folder, select Android Application Project,
              and click next.
              • Provide the application name and the project name and then finally give the desired
              package name.
              • Choose a launcher icon for your application and then select Blank Activity and then click
              Next
              • Provide the desired Activity name for your project and then click Finish.

Step 2: Create a New AVD (Android Virtual Device):
        • click Android Virtual Device Manager from the toolbar.
        • In the Android Virtual Device Manager panel, click New.
        • Fill in the details for the AVD. Give it a name, a platform target, an SD card size, and
        a skin (HVGA is default).
        • Click Create AVD and Select the new AVD from the Android Virtual Device
        Manager and click Start.

Step 3: Design the graphical layout with a text view and two command buttons.

Step 4: Run the application.

Step 5:On pressing the change font size button, the size of the font gets altered.       
       
Step 6:Close the Android project. 


## Program:
 ```
/*
Program to Develop an application that uses Font Size using Android Studio .
Developed by: Chevula Naga Durga
RegisterNumber:  212221230014
*/
```

## MainActivity.java:
```
package com.firstapp.fontsize;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;

import android.app.Activity;
import android.graphics.Typeface;
import android.graphics.Color;
import android.view.View;
import android.widget.Button;
import android.widget.TextView;


public class MainActivity extends AppCompatActivity {
    float font = 24;
    int i = 1;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        final TextView t1 = (TextView)findViewById(R.id.textView1);
        Button b1 = (Button)findViewById(R.id.button1);
        b1.setOnClickListener(new View.OnClickListener()    {
            public void onClick(View view) {
                t1.setTextSize(font);
                font = font+4;
                if(font==40)
                    font = 20;
            }
        });


    }
}
``



## activity_main.xml:
```
package com.firstapp.fontsize;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;

import android.app.Activity;
import android.graphics.Typeface;
import android.graphics.Color;
import android.view.View;
import android.widget.Button;
import android.widget.TextView;


public class MainActivity extends AppCompatActivity {
    float font = 24;
    int i = 1;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        final TextView t1 = (TextView)findViewById(R.id.textView1);
        Button b1 = (Button)findViewById(R.id.button1);
        b1.setOnClickListener(new View.OnClickListener()    {
            public void onClick(View view) {
                t1.setTextSize(font);
                font = font+4;
                if(font==40)
                    font = 20;
            }
        });


    }
}


```

## Output:
![2](https://user-images.githubusercontent.com/94185707/233934109-2f892ca1-f698-4408-a140-9ef98ff24d94.jpg)
![3](https://user-images.githubusercontent.com/94185707/233934261-e53c5872-ecf0-436c-8133-e2c839fcb711.jpg)




## Result:
Thus, the program for android application, Font Size was executed successfully using Android Studio.
