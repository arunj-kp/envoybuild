# envoybuild
Checkout this project and run release build ```./gradlew assembleRelease```, you will get the following error

```
Execution failed for task ':app:mergeDexRelease'.
> A failure occurred while executing com.android.build.gradle.internal.tasks.DexMergingTaskDelegate
   > There was a failure while executing work items
      > A failure occurred while executing com.android.build.gradle.internal.tasks.DexMergingWorkAction
         > com.android.builder.dexing.DexArchiveMergerException: Error while merging dex archives: 
           Type io.envoyproxy.envoymobile.R is defined multiple times: <user_directory>/envoybuild/app/build/intermediates/project_dex_archive/release/out/e17d2b7d3b3cd38559814e5bf3bad06f88686caea0b21925ac792110a6c8e56d_1.jar:classes.dex, <user_directory>/envoybuild/app/build/intermediates/external_libs_dex/release/mergeExtDexRelease/classes.dex
           Learn how to resolve the issue at https://developer.android.com/studio/build/dependencies#duplicate_classes.
           
```


Debug build works fine ```./gradlew assembleDebug``` 



