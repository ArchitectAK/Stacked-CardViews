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
	

### Contact - Let's connect to learn together
- [Twitter](https://twitter.com/KumarAnkitRKE)
- [Github](https://github.com/AnkitDroidGit)
- [LinkedIn](https://www.linkedin.com/in/kumarankitkumar/)
- [Facebook](https://www.facebook.com/freeankit)
- [Slack](https://ankitdroid.slack.com)
- [Stackoverflow](https://stackoverflow.com/users/3282461/android)
- [Android App](https://play.google.com/store/apps/details?id=com.freeankit.ankitprofile)


### License

    Copyright 2017 Ankit Kumar
    
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

