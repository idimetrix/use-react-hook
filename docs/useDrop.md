# `useDrop` and `useDropArea`

Triggers on file, link drop and copy-paste.

`useDrop` tracks events for the whole page, `useDropArea` tracks drop events
for a specific element.


## Usage

`useDrop`:

```jsx
import {useDrop} from 'use-react-hook';

const Demo = () => {
  const state = useDrop({
    onFiles: files => console.log('files', files),
    onUri: uri => console.log('uri', uri),
    onText: text => console.log('text', text),
  });

  return (
    <div>
      Drop something on the page.
    </div>
  );
};
```

`useDropArea`:

```jsx
import {useDropArea} from 'use-react-hook';

const Demo = () => {
  const [bond, state] = useDropArea({
    onFiles: files => console.log('files', files),
    onUri: uri => console.log('uri', uri),
    onText: text => console.log('text', text),
  });

  return (
    <div {...bond}>
      Drop something here.
    </div>
  );
};
```
