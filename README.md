# Documentation

These are the steps which used to make First AR app in Android Studio.


1.	If you new to AR Core then, firstly study about what is AR Core. Then know about Scenefrom library which is used to render 3D scenes in AR without having to learn OpenGL.
2.	Install Google Sceneform Tools from SDK under plugin.
3.	Then I add some dependencies to Gradle file.

```
// Provides ARCore Session and related resources.
implementation 'com.google.ar:core:1.12.0'

// Alternatively, use ArSceneView without the UX dependency.
implementation 'com.google.ar.sceneform:core:1.12.0'
```

And Sync.

4.	Then add some permission in manifest file to access camera and uses feature to access AR camera.
5.	Then download model which is used to place in real world from poly.google.com and copy to sampledata directory. Then click on model.obj to import Scenefrom asset.
6.	After That I add Fragment in my activity_main.xml layout file for AR Scenefrom.


```
<fragment
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:id="@+id/arFrag"
    android:name="com.google.ar.sceneform.ux.ArFragment"/>
```

7.	Then write code for implementing Scenefrom to render 3D model in MainActivity.java. If you having any issue see the codes.


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
[MIT](https://choosealicense.com/licenses/mit/)
