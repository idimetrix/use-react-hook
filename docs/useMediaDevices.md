# `useMediaDevices`

React sensor hook that tracks connected hardware devices.


## Usage

```jsx
import {useMediaDevices} from 'use-react-hook';

const Demo = () => {
  const state = useMediaDevices();

  return (
    <pre>
      {JSON.stringify(state, null, 2)}
    </pre>
  );
};
```
