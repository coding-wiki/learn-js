## Misc React Native Examples
TODO: Move these into example folders

This is a temporary file.


## Flow
```js
// @flow

import types { Post } from '../types'

type Props = {
  id: number,
  post: Post,
}

class Button<Props, State> {
  miscRef: any; // Flow class property

  constructor(props) {
    super(props) {
    
    this.state = {};
  }
  
  render() {
    const { post } = this.props;
  
    return (
      <Post post={post} />
    );
  }
 }
```

