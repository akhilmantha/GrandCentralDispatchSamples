# GrandCentralDispatchSamples




In iOS, Apple provides two ways to do multitasking: The Grand Central Dispatch (GCD) and NSOperationQueue frameworks. Both of them work perfectly when it’s time to assign tasks to different threads, or different queues other than the main one. Which one should be use is a subjective matter, but in this tutorial we’ll focus on the first one, the GCD. No matter what, there’s one rule that should be always respected: The main thread must be always remain free so it serves the user interface and user interactions. Any time-consuming or CPU demanding tasks should run on concurrent or background queues. Maybe this is difficult for new developers to digest and apply, however it’s the way things should be.

The Grand Central Dispatch was first introduced in iOS 4, and it offers great flexibility and options when trying to achieve concurrency, performance, and parallel tasks. It had a great disadvantage though until Swift 3: It was difficult to memorise its commands or easily write code regarding it, as its coding style was quite close to low level C, and it was obviously different than any other coding style in Swift, even in Objective-C. That was also the main reason that many developers were avoiding GCD on purpose, and they were choosing the NSOperationQueue. A simple web search about GCD in Swift versions other than the last one will give you a good taste of how GCD syntax had been.
