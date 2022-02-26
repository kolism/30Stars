## 💡 What we learned

- Learned about Redux stores and how provider wrappers programatically bind data such that rendered components receive updated data.
- Learned about yarn eject and ejecting create-react-app away from the react scripts into independant build scripts where webpack configs can be modified.
- Learned about the various versions of Chromium extension manifests and how popups, background, and content play together.
- Learned about extension permissions, script injection, and references web accessible assets.
- Learned about the chromium extension api, how to access tabs and window data.
- Learned more about font-face definitions and how to define your own font-families for usage.
- Firmed up my understanding of React useEffect hooks
- Firmed up my understanding of React functional vs class based components

## ✅ Accomplishments that we're proud of

- Functional extension that works quite smoothly!
- System is reactive, as tabs are updated/opened/closed, the elements in AlphaBar update and are ready for your command.
- Sleek build process where everything is layed out quite nicely at the moment: background, content and manifest are segregated well and are easy to develop against.

## ⚠Challenges we ran into

- This required more resources than expected, mainly due to attempted various approaches.
  - I had always intended to use a framework either React or Vue or similar.
  - Initially with Kbar (react) and finally with Ninja-Keys (web compoennt). We ran into web component consumption issues when used within a chrome/edge extension. 
  - We had to setup a message passing channel between React(content.js) and Redux store (background.js). 
    - The errors were a little ambiguous. All of these challenges serve as a beneficial lesson.

- We spend a fair bit of time trying to import material design icons for usage with Ninja-Keys, local fonts within a chrome/edge extension just weren't playing well!
  - We settled for SVG icons rather than font icons for now. Font icons has been added as a future ToDo item.

## 🚧 How we built it

- A base React application, using `create-react-app <name>` which was ejected with `yarn eject`.
- An updated webpack config to create extensionreferencable `content.js` and `background.js` entry points
- An updated `public/manifest.js` file to define the extension.
- The addition of `public/pages/content/index.js+++++` and `public/pages/background/index.js+++++` to define the application scripts.
- After the above scaffolding was done, we had our `content/index.js` updated to inject the React component containing Ninja-keys onto every web page.
- Finally, we used `webext-react`, `redux` to pass chromium message data between the content and background.

### 💎Full Feature List

- `CMD+K` and `CTRL+K` command bar on every web page
- Search and navigate to any open tab from the bar
- More features to come