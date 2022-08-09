# build.gradle dependencies

### Ktx
    plugin :
    id 'kotlin-kapt'

### Hilt : 2.38.1
    plugin : 
    id 'dagger.hilt.android.plugin'
    
    implementation 'com.google.dagger:hilt-android:' + hilt_version
    kapt 'com.google.dagger:hilt-compiler:' + hilt_version
    
    classpath 'com.google.dagger:hilt-android-gradle-plugin:' + hilt_plugin_version

### Room : 2.4.1
    implementation "androidx.room:room-runtime:$room_version"
    implementation "androidx.room:room-ktx:$room_version"
    kapt "androidx.room:room-compiler:$room_version"
    
 ### Navigation : 2.4.2
    plugin:
    id 'androidx.navigation.safeargs.kotlin'
 
    implementation 'androidx.navigation:navigation-fragment-ktx:' + navigation_version
    implementation 'androidx.navigation:navigation-ui-ktx:' + navigation_version
    classpath "androidx.navigation:navigation-safe-args-gradle-plugin:$navigation_version"
        
### Fragment : 1.4.1
    implementation "androidx.fragment:fragment-ktx:" + fragment_version
    
### Lifecycle : 2.4.1
    implementation 'androidx.lifecycle:lifecycle-runtime-ktx:' + lifecycle_version
    
### Retrofit : 2.9.0
    implementation "com.squareup.retrofit2:retrofit:$retrofit_version"
    implementation "com.squareup.retrofit2:converter-gson:$retrofit_version"
    implementation("com.squareup.okhttp3:okhttp:4.9.1")

### Glide Dependencies : 4.12.0
    implementation "com.github.bumptech.glide:glide:$glide_version"
    kapt "com.github.bumptech.glide:compiler:$glide_version"
    
### Databinding :
    buildFeatures.dataBinding = true

