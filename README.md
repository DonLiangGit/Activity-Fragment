Activity-Fragment
=================

Activity Manager in Android Framework and Fragment related things.

A complete Activity and Fragment lifecycle below:

![alt text](https://raw.githubusercontent.com/xxv/android-lifecycle/master/complete_android_fragment_lifecycle.png "Activity and Fragement Lifecycle")

Activity:
  1. onCreate() is called -> saveInstanceState = null, no state for the application
  2. onStart() and onResume() runs when the app runs
  3. onPause() - onStop() - onDestroy() are called sequentially when pressing the BACK button
  4. onPause() - onStop() are called when pressing the HOME button
  5. onRestart() - onStart() - onResume() are called when return to the activity

Fragment:
  1. onAttache(): attach the fragment to activity
  2. onCreate(): create the fragment itself
  3. onCreateView(): create the fragment UI
  4. onStart()/onResume() are similar to the activity
  5. onPause()/onStop()/onDestoryView()/onDestroy are called before the corresponding method of Activity
  6. onDetach()
