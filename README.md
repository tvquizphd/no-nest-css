## no-nest-css

Remove nesting from CSS

```
import { noNestCSS } from 'no-nest-css';

const result = noNestCSS(`
  div {
    & > p {
      color: red;
    }
    & > h1 {
      color: blue;
    }
  }
`);
```

Will result in `result` as

```
`
  div  > p  {  color: red;  }
  div  > h1  {  color: blue;  }
`
```

