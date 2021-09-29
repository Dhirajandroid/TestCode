<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <Button
        android:id="@+id/show_button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Show"
        android:layout_centerInParent="true"
        android:textSize="14sp"
        />

    <RelativeLayout
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_below="@+id/show_button"
        android:layout_marginTop="40dp"
        android:layout_centerHorizontal="true"
        android:visibility="invisible"
        >

        <ImageView
            android:id="@+id/close"
            android:layout_width="40dp"
            android:layout_height="40dp"
            android:layout_alignEnd="@+id/email"
            android:src="@drawable/close"
            android:layout_alignRight="@+id/name" />

        <LinearLayout
            android:id="@+id/name"
            android:layout_centerHorizontal="true"
            android:layout_marginTop="20dp"
            android:layout_width="wrap_content"
            android:layout_below="@+id/close"
            android:layout_height="wrap_content"
            >

            <TextView
                android:id="@+id/name_label"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="Name:"
                android:textSize="14sp"
                />

            <EditText
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:textSize="14sp"
                android:text="Madhuri"
                android:layout_marginStart="15dp"
                android:layout_marginLeft="15dp" />


        </LinearLayout>

        <LinearLayout
            android:id="@+id/designation"
            android:layout_width="wrap_content"
            android:layout_centerHorizontal="true"
            android:layout_below="@+id/name"
            android:layout_height="wrap_content">

            <TextView
                android:id="@+id/designation_label"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="Designation:"
                android:textSize="14sp"
                />

            <EditText
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:textSize="14sp"
                android:text="Trainee"
                android:layout_marginStart="15dp"
                android:layout_marginLeft="15dp" />


        </LinearLayout>

        <LinearLayout
            android:id="@+id/email"
            android:layout_width="wrap_content"
            android:layout_below="@+id/designation"
            android:layout_centerHorizontal="true"
            android:layout_height="wrap_content">

            <TextView
                android:id="@+id/email_label"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="Email:"
                android:textSize="14sp"
                />

            <EditText
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:textSize="14sp"
                android:text="madhuri@gmail.com"
                android:layout_marginStart="15dp"
                android:layout_marginLeft="15dp" />


        </LinearLayout>

    </RelativeLayout>

</RelativeLayout>
