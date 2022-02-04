# ispace-people-app
![TheMaster](https://github.com/Albert-Osei/ispace-people-app/blob/main/app/src/main/res/raw/demo1.png)

![TheMaster](https://github.com/Albert-Osei/ispace-people-app/blob/main/app/src/main/res/raw/demo2.png)

![TheMaster](https://github.com/Albert-Osei/ispace-people-app/blob/main/app/src/main/res/raw/demo3.png)

It uses a BitmapShader and *does not*:
* create a copy of the original bitmap
* use a clipPath (which is neither hardware accelerated nor anti-aliased)
* use setXfermode to clip the bitmap (which means drawing twice to the canvas)

Gradle
------

dependencies {
    ...
    implementation 'androidx.core:core-ktx:1.7.0'
    implementation 'androidx.appcompat:appcompat:1.4.1'
    implementation 'com.google.android.material:material:1.5.0'
    implementation 'androidx.constraintlayout:constraintlayout:2.1.3'
}


 Usage
-----
xml
 <androidx.recyclerview.widget.RecyclerView
        android:layout_width="match_parent"
        android:id="@+id/recyclerViewpm"
        android:scrollbars="vertical"
        android:layout_height="match_parent"/>
  
  <TextView
              android:id="@+id/textView"
              android:layout_width="match_parent"
              android:layout_height="wrap_content"
              android:layout_marginStart="10dp"
              android:layout_marginTop="30dp"
              android:layout_marginEnd="20dp"
              android:layout_toEndOf="@+id/profile_image_root"
              android:gravity="center"
              android:padding="5dp"
              android:text="Name"
              android:textColor="#808080"
              android:textSize="25sp"
              android:textStyle="bold|italic" />
              
   <ImageView
        android:layout_width="24dp"
        android:layout_alignParentEnd="true"
        android:layout_marginTop="40dp"
        android:layout_marginEnd="20dp"
        android:src="@drawable/arrowdetails"
        android:layout_height="24dp"/>
		


License
-------

 	Copyright 2022 - 2023 Albert
