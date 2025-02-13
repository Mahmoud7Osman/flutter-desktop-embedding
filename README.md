# Adjusting Window Size
<pre>
  // git clone this repo and rename the folder to 'plugins'
  
  // main.dart
  import "package:cvenom/window_size.dart";
  
  void main(){
  	  WidgetsFlutterBinding.ensureInitialized(); // Initialization
  	  setWindowTitle("Title");            // Window Title
	  setWindowMinSize(Size(1000, 1000)); // Minimum Window Size
	  setWindowMaxSize(Size(1000, 1000)); // Maximum Window Size
    
	  runApp(MaterialApp(home:App()));
  }
  // Copy window_size.dart and src/ from plugins to lib/
  // then your pubspec.yaml should look like this
  // ------------------------------------------------
  
  // pubspec.yaml
  dependencies:
  	window_size:
		path: plugins/window_size
</pre>

# Desktop Embedding for Flutter

This project was originally created to develop Windows, macOS, and Linux
embeddings of [Flutter](https://github.com/flutter/flutter). That work has
since become part of Flutter, and all that remains here are experimental,
early-stage desktop
[plugins](https://flutter.dev/docs/development/packages-and-plugins/developing-packages).

If you want to get started with Flutter on desktop, the place to start is now
[the Flutter documentation](https://flutter.dev/desktop), rather than this project.
You will already need to have followed the instructions there to get an application
running on desktop before using any of the plugins here.

## Feedback

**Do not file issues about Flutter for desktop here.** Since the
embeddings have all moved to the Flutter project, the place for desktop bugs
and feature requests is now [the Flutter issue
tracker](https://github.com/flutter/flutter/issues).

For bug reports and feature requests **related to the plugins in this repository**,
please file issues here.

## Repository Structure

The `plugins` directory contains all the plugins. See
[its README](plugins/README.md) to get started.

## Caveats

* This is not an officially supported Google product.
