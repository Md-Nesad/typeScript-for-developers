# Union and Intersection Type

## Union Type

```ts
let userId: string | number;

userId = "abc123";
userId = 100;
```

### Explanation:

- Multiple type allow করে

---

## Intersection Type

```ts
type Person = {
  name: string;
};

type Employee = {
  company: string;
};

type Developer = Person & Employee;

const dev: Developer = {
  name: "Nesad",
  company: "Google",
};
```

### Explanation:

- Multiple type combine করে
