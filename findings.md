

The [NG2-native rendering library](https://github.com/angular/react-native-renderer) is under the angular organisation.

So it's officially endorsed in a way. But currently it's a small french company developing it.

Currently it's in alpha; looking for feedback etc. So we'll have to keep track to see whether it will evolve enough.

At this point it runs on iOs and Android. MS and Facebook are collaborating to make React Native support Windows Universal Platform. Then this stack will also run on Windows Universal Platform.

How it works is easily seen from the diagram on 

The seed project includes the following tests:
 - e2e using Appium running in the native rendering in simulators
 - protractor in the browser
 
it feels a bit challenging to have js dev tools, ios devtools and node tools work together flawlessly. Your build inevatibily will contain more moving parts.
 

you can reuse components unchanged between native platforms (if you use components that are supported on both).
But there was some discussion whether you can render it in the browser as well. It's not in the seed project.
But it might be feasible since the elements are just selectors for ng2 components.

Otherwise you'd have to refactor out some shared logic and different UI wrapping. 
Then you'd create NG2 services to encapsulate the logic. The components will probably be have to be different 

The trade off between NG2 + React Native vs say Cordova is similar to
SWT vs Swing

Lots of large collaborators: Google, Facebook, Microsoft. But primary development by 1 man/small french company.
* + Native widgets
* + Developer skill sharing, Knowledge sharing (angular2 skills translate)
* + Possibility for code sharing
* +/- Might be feasible to develop for web+native mobile with this if you start with it in mind or heavily refactor
* - Not magically run an angular2 app on your phone
* - No HTML or CSS on mobile, which a Webview wrapper/Cordava

Potential areas of further research: 
- compare with alternatives like Nativescript and Ionic 2
