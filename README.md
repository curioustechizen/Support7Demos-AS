Support7Demos-AS
================

The Support7Demos project imported into Android Studio 0.8.1, and suitable modifications to make it run.

The `Support7Demos` in my sdk/extras folder was in Eclipse project structure. Importing it into Android Studio using the wizard did most of the work for me, but the dependencies were not set up correctly.

Currently, I've set everything (`minSdk`, `compileSdk` and `targetSdk`) to Android L preview but this is a __support__ demo after all so it should ideally work with older versions of Android as well. Getting this to work is a TO-DO.

Also, it seems like Google changed some APIs after these samples were packaged. For example, in `com.example.android.supportv7.widget.AnimatedRecyclerView.java` there was a sub-class of `LayoutManager` that overrode a method `supportsItemAnimations()`. However, this method has been renamed `supportsPredictiveItemAnimations()` in the preview SDK.


LICENSE
========

 Copyright (C) 2014 The Android Open Source Project

 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at

 http://www.apache.org/licenses/LICENSE-2.0

 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
