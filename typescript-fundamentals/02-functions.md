# 2. Functions

### Function Typing

```ts
function add(a: number, b: number): number {
  return a + b;
}
```

### Explanation:

- Parameter type define করা হয়েছে
- Return type number

---

### Optional Parameters

```ts
function greet(name: string, age?: number) {
  console.log(`Hello ${name}`);
}

greet("Nesad");
```

### Explanation:

- parameter optional করা যায় `?` দিয়ে
- value না দিলে default behavior ব্যবহার হয়

---

### Default Parameters

```ts
function welcome(user: string = "Guest") {
  console.log(`Welcome ${user}`);
}

welcome();
```

### Explanation:

- default value set করা যায়
- যদি value না দেওয়া হয়, default value use হয়

---
