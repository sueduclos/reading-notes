[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 22: React Testing and Deployment

### Links

- [Jest Testing with React](https://create-react-app.dev/docs/running-tests/) 
- [Snapshot Testing](https://jestjs.io/docs/en/snapshot-testing) 
- [Static Rendering - Enzyme](https://airbnb.io/enzyme/docs/api/shallow.html) 
- [Shallow Mounting - Enzyme](https://airbnb.io/enzyme/docs/api/render.html) 
- [Full Mounting - Enzyme](https://airbnb.io/enzyme/docs/api/mount.html) 
- [AWS S3 Deployment](https://www.youtube.com/watch?v=Kay-UvVCNFs) 
- [AWS Amplify Deployment](https://www.youtube.com/watch?v=DHLZAzdT44Y) 
- [Netlify Deployment](https://www.youtube.com/watch?v=sGBdp9r2GSg) 
                                              


### Discussion Questions:

#### 1. Describe a case where snapshot testing would be useful, and describe another case where it would be ineffective.
Snapshot testing is great for fully developed UI pages that you want to ensure does not change throughout development. Best for when you are doing some refactoring. Snapshot testing is not effective if you are consistently changing your UI since your snapshots become outdated and can cause your tests to fail incorrectly.

#### 2. What is the difference between full mount and shallow mount? 
Full mounting allows you render the entire component as well as any children components. This allows you to fully test the current component and any components it imports. Shallow mounting minimized the render of any imported components, and instead focuses on fully rendering the current component only.


#### 3. What does `npm run build` do? 
It creates a `build` directory with a production build of your app. It runs the build field from the `package.json` `scripts` field.
