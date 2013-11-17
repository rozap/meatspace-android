# Meatspace-android

An android client for the great chatting space [https://chat.meatspac.es](https://chat.meatspac.es).

## Setting up

Check out the sources and submodules:
```bash
> git submodule update
```

### Run on your machine:

To run the server on your machine, follow the instructions described [there](https://github.com/meatspaces/meatspace-chat).

In the android project, edit the variable `url_api_debug` Meatspace/src/main/res/values/urls.xml:

```xml
    <string name="url_api_debug">http://192.168.1.110:3000</string> // set your computer IP here
```

List your keys in the file located at

```xml
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <string name="key_api_debug">blahblahblah</string>
    <string name="key_api_staging"></string>
    <string name="key_api_release"></string>
</resources>
```

To start the android app in debug mode, run that from the android project folder:

```bash
> ./gradlew installDebug
```

### Using production server:

```bash
> ./gradlew installRelease
```

## Libraries used

Thanks to the creators/contributors of all of these open-source libraries:
- [android-websockets](https://github.com/koush/android-websockets)
- [butterknife](https://github.com/JakeWharton/butterknife)
- [google-gson](https://code.google.com/p/google-gson)
- [retrofit](https://github.com/square/retrofit)
- [otto](https://github.com/square/otto)
