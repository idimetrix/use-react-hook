# `useEffectOnce`

React lifecycle hook that runs an effect only once.

## Usage

```jsx
import {useEffectOnce} from 'use-react-hook';

const Demo = () => {
  useEffectOnce(() => {
    console.log('Running effect once on mount')

    return () => {
      console.log('Running clean-up of effect on unmount')
    }
  });

  return null;
};
```

## Reference

```js
useEffectOnce(effect: EffectCallback);
```
