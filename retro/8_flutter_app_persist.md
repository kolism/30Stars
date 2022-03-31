## 💡 What we learned

- Alot of my learnings have been posted in the blog, we can direct you to there. But to recap:
- Flutter compilation targets explored: web, windows desktop, mac desktop, ios, android
  - Learned that we can develop flutter widgets to switch design/behavior based on environemnt
- Learned about navigation, having multiple pages, and how the navigator can control the flow/view of the application
- Learned about animating the switching between page widgets
- Learned about persistent storage options: namely a LocalStorage clone (kvp) or SQLite as top contendors
- Learned about timers in Flutter
- Learned about graphics drawing (canvas) within flutter and how to apply timing, math and ultimately animation to graphics
- Learned about widget dataflow and 2-way databinding
- Learned about custom dialogs and text inputs (where we handle the input data through a controller)

## ✅ Accomplishments that we're proud of

- A performant little spree tracking app!
- The UI is super sleek, was able to implement a splash screen and animated navigation buttons

## ⚠Challenges we ran into

- Typical learning curve when picking up a new language, dev environment and ecosystem. The same challenges lead to plenty of enjoyment and learning.
- Had a few areas such as design decisions for how to layout a splash widget which plays well with main view widgets
  - This would have been a nice topic to ask a SME

## 🚧 How we built it

- Started wireframing in Figma
- Began with a simple, single page splash page with a button and went from there, still many TODOs
- We leveraged shared_preferences for peristent app-wide storage
- Widgets maintain their own ephemeral data state where applicable

### 💎Full Feature List

- A spree tracking app! Click start, enter your goal and end the timer if you break your spree. Great way to get inspired to continue your goals.
- Example usage: I want to wake @ 5AM every day, if you fail to do this, maybe you break your spree, otherwise, let it run and see how long you can maintain!
