# `useWindowSize`

React sensor hook that tracks dimensions of the browser window.


## Usage

```jsx
import {useWindowSize} from 'use-react-hook';

const Demo = () => {
  const {width, height} = useWindowSize();

  return (
    <div>
      <div>width: {width}</div>
      <div>height: {height}</div>
    </div>
  );
};
```
