# Flutter/MX

Programming [Flutter](https://flutter.dev/?gclid=CjwKCAjwwdWVBhA4EiwAjcYJEEoxUuE14sd2MGLJW35qeuJynmTRjqpUL3SbIUhOiS4TihjyZ9iTVRoCJkoQAvD_BwE&gclsrc=aw.ds) with [ClojureDart](https://github.com/Tensegritics/ClojureDart) and [Matrix](https://github.com/kennytilton/matrix), a generic, fine-grained, transparent, reactive state manager.

## Documentation
See our Wiki! (Soon)

## Running the demos/examples

If you just want to run the thing...

### 0. Preparing environment, on Mac OS X

First, complete the [ClojureDart "Flutter Quick Start"](https://github.com/Tensegritics/ClojureDart/blob/main/doc/flutter-quick-start.md). Help with that can be had in the #ClojureDart channel on the #Clojurians Slack. Or ping @Tilton on that Slack or the Flutter Community Slack.

### 1. Download this repo
`git clone` this [mxFlutter repo](https://github.com/kennytilton/mxflutter).

### 2. Running the sample app.

In a terminal:
* `cd flutter-mx`, or wherever you cloned it;
* start a sim: `open -a Simulator`

TIP: If you forget that step, the next command will run for ages and open a tab in your browser. Start over. 

* `clj -M -m cljd.build flutter`

This ^^^ command does not return. After thirty seconds you should see these last lines of output:
```
An Observatory debugger and profiler on iPhone 12 is available at: http://127.0.0.1:61081/v17dEYvUuuQ=/
The Flutter DevTools debugger and profiler on iPhone 12 is available at: http://127.0.0.1:9100?uri=http://127.0.0.1:61081/v17dEYvUuuQ=/
```
Visit either debugger at the URLs shown if you like. We get by on the console output.

You should also see our "hello, world" app in the sim:

![FMX Hello World screenshot](image/hello-world-app.jpg)

### Workflow
Here is how I work:

* start with the above;
* edit this project in IntelliJ+Cursive, with the Flutter plug-in installed;
* * I told IntelliJ to use clj formatting for .cljd files; more Cursive support is on the way;
* after changes I save in IntelliJ and look at the "build" terminal for errors;
* if I am curious some CLJD issue, like how to run the Math `abs` method, I do this:
* * add snippets of code to the main function, after the test suite runner;
* * save;
* * check the "build" for errors;
* * switch to the build terminal and hit Return to trigger a sim reload;
* * check the Flutter console for print output.

Ping @kennytilton on #clojurians Slack for help!
