# `useMotion`

React sensor hook that uses device's acceleration sensor to track its motions.


## Usage

```jsx
import {useMotion} from 'use-react-hook';

const Demo = () => {
  const state = useMotion();

  return (
    <pre>
      {JSON.stringify(state, null, 2)}
    </pre>
  );
};
```
