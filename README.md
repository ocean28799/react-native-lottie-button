## react-native-scrollable-tabview

## Add it to your project

### Install

First, you must need to install lottie-react-native: (https://github.com/lottie-react-native/lottie-react-native)

Then, run `npm install @ocean28799/react-native-lottie-button --save`

OR `yarn add @ocean28799/react-native-lottie-button`

### Import

`import { LottieButton } from '@ocean28799/react-native-lottie-button';`

## Demo

| ![Screenshot](https://github.com/ShaunLWM/react-animated-heart/blob/HEAD/img/ss.gif) |

## Basic usage

```javascript
import React from "react";
import { LottieButton } from "@ocean28799/react-native-lottie-button";

export default function Demo() {
  const [status, setStatus] = useState(false);
  return (
    <LottieButton
      width={48}
      status={status}
      onPress={() => {
        console.log("Doing sth when press button");
        setStatus(!status);
      }}
      // source = {require("./lottiefile.json")}
    />
  );
}
```

## Props

- **`source`** _(JSON FILE)_ - (**require**) - source of lottie file, you can get on: (https://lottiefiles.com/). Default is heart animation.
- **`width`** _(Number)_ - size of lottie file, default to 48
- **`status`** _(Boolean)_ - status of the animation, if it's true -> animation is finished
- **`containerStyle`** _(Object)_ - Additional styles to the container of button.
- **`onPress`** _(Function)_ - function when on press button
- **`...props`** _(Props)_ - another props valid to TouchableOpacity of React Native
