# UI Testing Espresso - Android
##### Tutorial: CodingWithMitch - UI Testing for Beginners (Espresso and androidx.test)

## Purpose: 
The purpose of this code base is to explore how UI Testing is done in Android using the Espresso library.

## Setup
### Dependencies
Check for new version updates. 

```
    // Espresso
    def androidx_test_espresso = "3.3.0"
    androidTestImplementation "androidx.test.espresso:espresso-core:$androidx_test_espresso"

    // androidx.test
    def androidx_test = "1.3.0"
    androidTestImplementation "androidx.test:runner:$androidx_test"
    androidTestImplementation "androidx.test:core:$androidx_test"
    androidTestImplementation "androidx.test.ext:junit-ktx:$androidx_test"
    
```

### Disable animations
You need to disable animations on the simulator/device as they can disrupt the UI test.
Device: System > Developer Options > Drawing
- Window Animation Scale
- Transition Animation Scale
- Animator Duration Scale


### Navigating 
app > src > androidtest > java > com. > testfile

Note: If you cannot see the src directory, go to the top drop down menu and change it from Android to Project.

### Adding Testing Files
The quickest way to add a test file is to go to the class that you want to test, right click on the class name, click generate, then select test.
- AndroidTestFolder = UITesting
- TestFolder = UnitTesting


## Implementation:
### Testing Activities in isolation

