# Stacked-CardViews


![GIF](https://github.com/AnkitDroidGit/Stacked-CardViews/blob/master/app/art/video.gif)


To use this libraray there are two ways.. You can use either one of both.


1. Use Maven
open Project level Project.gradle file and add this inside dependencie

		maven {
			 url 'https://dl.bintray.com/ankitdroiddeveloper/FreeStacks'
			}
		
Now add this dependency to your app.gradle

	    compile 'com.freeankit.freestack:freeStack:1.0.0@aar'
	
	
2. Use JCenter. Easier ways

add this dependency to your app.gradle

	     compile 'com.freeankit.freestack:freeStack:1.0.0'
			
In your xml file assign StackedCardview as below

        <com.freeankit.freestack.CardStackView
        android:id="@+id/stackview_main"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:background="@android:color/white"
        android:clipToPadding="false"
        android:paddingLeft="12dp"
        android:paddingRight="12dp"
        android:paddingTop="12dp" />
				
				
Assign and use in Activity

        mStackView = (CardStackView) findViewById(R.id.stackview_main);
        mStackView.setItemExpendListener(this);
        freeAnkitStackAdapter = new FreeAnkitStackAdapter(this);  // See code for implementation
        mStackView.setAdapter(freeAnkitStackAdapter);
