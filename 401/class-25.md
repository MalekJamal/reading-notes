### What is a Chakra UI?
> Chakra UI is a component-based library. It's made up of basic building blocks that can help you build the front-end of your web application.
> It is customizable and reusable, and most importantly it supports ReactJs, along with some other libraries too.
> Chakra UI is extremely simple to use, especially when you are familiar with how to use ReactJs components.
> Chakra UI is a more robust, layout-focused library that also provides developers with UI components similar to those that Material UI provides,
>  but has a greater focus on the creation of flexible, composable, and scalable code. 
>  A core concept to be considered when comparing the two frameworks is 'Ease of Modification'.

***
### Is Chakra UI better than material UI?
> First of let’s talk about ‘Ease of Modification’ with these two UI libraries, the Chakra UI is having clean class names structure. Now what does that mean,
> for example if you see the HTML source code build in both libraries, you will see the material UI adds so many classes to each HTML tags created for 
> material component, where Chakra UI adds comparatively less classes.
> Also, Chakra UI provides easy manual manipulation in CSS classes, where Material UI has way more options to do it for way more components than Chakra UI.
> In additions, Material UI components has more feature and properties which make them more Flexible.

> Then let’s talk about second point of comparison, which is ‘Ease of Use’. Since Material UI is having lot more controls and their too many numbers of properties,
> this will naturally lead to more time to understand them and decide which component to use in some scenarios. Since Chakra UI is newer, 
> it is currently easier to pick up controls from it. In terms of documentation, both options have good documentation but I think material UI will win in it, 
> but it takes more time to go through. So, both libraries are easy to use but Chakra is easier than Material UI.

> Now the last point ‘Reliability’, here in terms of reliability and active community, there is no competition and Material Ui is the definite winner here. 
> Material UI has 70.9K starts as of now on GitHub and strong community makes it most popular UI framework. The Chakra UI is created only 2 years back and currently 
> having over 20.6K stars as of now on GitHub, but during this short period of time Chakra UI has earned a lot of positive comments from top React developers as 
> it is very extensible and customizable.
- [‘Materials UI’ or ‘Chakra UI’](https://dev.to/paresh4734/materials-ui-or-chakra-ui-what-is-better-for-react-37mh)

***
### How to use Chakra UI?

> To use Chakra UI in your project, run one of the following commands in your terminal:

```javascript
npm i @chakra-ui/react @emotion/react @emotion/styled framer-motion
```

> After installing Chakra UI, you need to set up the ChakraProvider at the root of your application. This can be either in your index.jsx, index.tsx or 
> App.jsx depending on the framework you use.

```javascript
import * as React from 'react'

// 1. import `ChakraProvider` component
import { ChakraProvider } from '@chakra-ui/react'

function App() {
  // 2. Wrap ChakraProvider at the root of your app
  return (
    <ChakraProvider>
      <TheRestOfYourApplication />
    </ChakraProvider>
  )
}
```

