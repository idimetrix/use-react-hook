# `useMouseWheel` 
React Hook to get deltaY of mouse scrolled in window. 

## Usage

```jsx
import { useMouseWheel } from 'use-react-hook';

const Demo = () => {
  const mouseWheel = useMouseWheel()
  return (
    <>
      <h3>delta Y Scrolled: {mouseWheel}</h3>
    </>
  );
};
```
