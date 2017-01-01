#Android GoUbiquitous - Watch Face Sync 
===================================

Synchronizes weather information from [OpenWeatherMap](https://openweathermap.org/) on **Android Phones**, **Tablets** and **Watch**. Watch Face in Wear displays the weather information and uses services to sync the data

##Run it on your machine
---------------
- **Setup mobile and wear**:
  You need to first connect your mobile and wear, either using emulator or physical devices.
  In my case I used physical mobile phone and wear emulator. For setup please refer [Documentation](https://developer.android.com/training/wearables/apps/creating.html).

- **Clone the project**:
  Go to any directory in your machine and run the below command on the terminal:
  ```
  git clone https://github.com/abilaashsai/Android-GoUbiquitous-WatchFaceSync.git
  ```
- **Get OpenWeatherMap API key**:
  - Go to [OpenWeatherMap](https://openweathermap.org/) and get the key. It's totally free.
  - In [build.gradle(Module:app)](https://github.com/abilaashsai/Android-GoUbiquitous-WatchFaceSync/blob/5502b3ce0cca2032ef664c12431a0f300ce6bd84/app/build.gradle) replace `ENTER_YOUR_KEY_HERE` with your _API_KEY_ on line 22.
   ```
   it.buildConfigField 'String', 'OPEN_WEATHER_MAP_API_KEY', '"ENTER_YOUR_KEY_HERE"'
   ```

- **Run the project**:
  I use Android Studio. Here you have to _Import_ the project and _Run_ on _wear_ and _mobile_.

##Contribution
-------
Patches are encouraged, and may be submitted by forking this project and
submitting a pull request through GitHub.

##Issue:
-------
Initially when _Watch Face_ is selected, data is not synced. When some data is changed in mobile, it is reflected in Watch Face.

License
-------
The contents of this repository are covered under the [MIT License](https://github.com/abilaashsai/Android-GoUbiquitous-WatchFaceSync/blob/master/LICENSE).
