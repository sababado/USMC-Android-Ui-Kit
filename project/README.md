# USMC-Android-Ui-Kit
Android library with USMC styles

App Bar
- Must use Coordinator Layout
- Look at `activity_main.xml` for an example.
- Manually set background (for now)

```xml
<com.google.android.material.appbar.AppBarLayout
            android:layout_height="wrap_content"
            android:layout_width="match_parent"
            android:theme="@style/USMCTheme.Flavor.AppBarOverlay">

        <androidx.appcompat.widget.Toolbar
                android:id="@+id/toolbar"
                android:layout_width="match_parent"
                android:layout_height="?attr/actionBarSize"
                android:background="@drawable/usmc_bottom_border_small"
                app:popupTheme="@style/USMCTheme.Flavor.PopupOverlay"/>

</com.google.android.material.appbar.AppBarLayout>
```

# Personal Lazy Reminder.
To publish
```
$ ./gradlew clean build bintrayUpload -PbintrayUser=BINTRAY_USERNAME -PbintrayKey=BINTRAY_KEY -PdryRun=false
```