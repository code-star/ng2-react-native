

The [NG2-native rendering library](https://github.com/angular/react-native-renderer) is under the angular organisation.

So it's officially endorsed in a way. But currently it's a small french company developing it.

Currently it's in alpha; looking for feedback etc. So we'll have to keep track to see whether it will evolve enough.

At this point it runs on iOs and Android. MS and Facebook are collaborating to make React Native support Windows Universal Platform. Then this stack will also run on Windows Universal Platform.

How it works is easily seen from the diagram on 

The seed project includes the following tests:
 - e2e using Appium running in the native rendering in simulators
 - protractor in the browser
 - 
 

you can reuse components unchanged between native platforms (if you use components that are supported on both).
But you can not render it in the browser as well. 
So you'd have to refactor out some shared logic and different UI wrapping. 

The trade off between NG2 + React Native vs say Cordova is similar to
SWT vs Swing


