# Context Api

v16.3  에 추가된 Context API와 관련하여 알아보겠습니다.



Store 생성

```javascript
import React from 'react';
const Store = React.createContext(null);
export default Store;
```

Provider 정의

```javascript
import React, { Component } from "react";
import AppPresenter from "./AppPresenter";
import Store from "store";

class AppContainer extends Component {
  render() {
    return (
      <Store.Provider>
        <AppPresenter />
      </Store.Provider>
    );
  }
}

export default AppContainer;
```





