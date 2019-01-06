# Inspiration

> 🎻 A collection of JavaScript+TypeScript design methods to inspire your coding.

I always ask myself the question **"What is the best way of writing this code?"** and so here is a collection of methods which you can use to help answer that question.

## Designs

### Imports

1. Import class as a default export.

```ts
import Inspo from 'inspiration';
```

2. Import class as a sub-module export.

```ts
import { Inspo } from 'inspiration';
```

3. Import a function as a default export.

```ts
import createInspiration from 'inspiration';
```

4. Import a function as a sub-module export.

```ts
import { createInspiration } from 'inspiration';
```

### Classes

1. Extend a class which already has some functionality.

```ts
class Inspiration {
  constructor(...args) {
    // code...
  }
  doSomethingCool() {
    // code...
  }
}

export default class SuperInspiration extends Inspiration {
  constructor(...args) {
    super(args);
  }
  doSomethingElseThatIsCool() {
    // code...
  }
}
```

2. Implement an interface which contains no functionality but does have a specific structure.

```ts
interface Inspiration {
  time: Date;
  setTime(t: Date);
}

export default class SuperInspiration implements Inspiration {
  time: Date;
  setTime(t: Date) {
    this.time = t;
  }
}
```

3. Use a static method to create and return an instance of a class.

```ts
class Inspiration {
  static create(...args) {
    return new Inspiration(...args);
  }
  name: string;
  constructor(name: string) {
    this.name = name;
  }
}

export default Inspiration.create('coolName');
```

## Authors

- Jack Scott [@jacrobsco](https://twitter.com/jacrobsco)
