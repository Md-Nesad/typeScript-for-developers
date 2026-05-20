# 3. Objects

```ts
const user: {
  name: string;
  age: number;
} = {
  name: "Nesad",
  age: 25,
};
```

### Explanation:

- object এর structure define করা হয়
- TypeScript নিশ্চিত করে সব property ঠিক আছে

---

## Type Aliases

```ts
type User = {
  name: string;
  age: number;
};

const user: User = {
  name: "Nesad",
  age: 25,
};
```

### Explanation:

- custom type তৈরি করার জন্য use হয়
- code reuse করা সহজ হয়

---

## Interfaces

```ts
interface Product {
  id: number;
  title: string;
  price: number;
}

const laptop: Product = {
  id: 1,
  title: "Macbook",
  price: 1200,
};
```

### Explanation:

- object structure define করার আরেকটা way
- mostly large applications এ use হয়

---

## Readonly & Optional Properties

```ts
interface User {
  readonly id: number;
  name: string;
}

const person: User = {
  id: 1,
  name: "Nesad",
};

// person.id = 10 ❌ Error
```

### Explanation:

- `readonly` মানে change করা যাবে না
- `?` মানে optional property

---
