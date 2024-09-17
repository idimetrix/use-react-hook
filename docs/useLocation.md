# `useLocation`

React sensor hook that tracks brower's location.

For Internet Explorer you need to [install a polyfill](https://github.com/idimetrix/use-react-hook/issues/73).


## Usage

```jsx
import {useLocation} from 'use-react-hook';

const Demo = () => {
  const state = useLocation();

  return (
    <pre>
      {JSON.stringify(state, null, 2)}
    </pre>
  );
};
```
