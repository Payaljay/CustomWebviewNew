# MobyCashbackWebView


#### Beautiful and customizable Android method for webview

* Builder pattern
* Dynamic url
* Location Enability
* Storage Permission
* Custom toolbar text color
* Custom background color for toolbar

## Getting started

#### Gradle Dependency (jcenter)

Add it in your root build.gradle at the end of repositories:

```java
	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
 ```
 
#### Gradle Dependency (jcenter)

Easily reference the library in your Android projects using this dependency in your module's `build.gradle` file.

```java
dependencies {
    implementation 'com.github.Payaljay:CustomWebviewNew:v1.0.5'
}
```


#### Manifest Settings

You have to add permission in your `AndroidManifest.xml`

```xml
    <uses-permission android:name="android.permission.INTERNET" />
    <uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION" />
    <uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" />
    <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />
    <uses-permission android:name="android.permission.CAMERA" />

    <uses-feature
        android:name="android.hardware.camera"
        android:required="true" />

<application
  android:requestLegacyExternalStorage="true">
```

#### Basic WebView

```java
FinestWebViewBuilder builder = new FinestWebViewBuilder().setUrl(url);
builder.loadWebView();
```


## Customization


#### GPS permission
```java
Enable GPS permission with below code.
setAccessGPS(true)
```

#### Storage permission
```java
Enable storage permission with below code.
setAccessStorage(true)
```

#### Toolbar Color
```java
Toolbar color will be set as `setPrimaryColor`.
setPrimaryColor("color")
```


#### Toolbar Menu Color
```java
Toolbar menu color will be set as `setSecondaryColor`.
setSecondaryColor("color")
```

#### Toolbar Text Color
```java
Toolbar color will be set as `setPrimaryTextColor`.
setPrimaryTextColor("color")
```

#### Toolbar Secondary Text Color
```java
Toolbar color will be set as `setSecondaryTextColor`.
setSecondaryTextColor("color")
```

#### 
```java
Toolbar color will be set as `setSecondaryTextColor`.
setSecondaryTextColor("color")
```




