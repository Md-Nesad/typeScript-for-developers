## Baic types. Every typeScript developers journey beggins from here

## 1. string

```ts
let userName: string = "Nesad";
console.log(userName);
```

### Explanation:

- `string` text value store করে
- Example: `name`, `email`, `title`

---

## 2. number

```ts
let age: number = 25;
let price: number = 99.99;
```

### Explanation:

- `number` integer এবং decimal দুইটাই support করে

---

## 3. boolean

```ts
let isDeveloper: boolean = true;
let isLoggedIn: boolean = false;
```

### Explanation:

- শুধু `true` অথবা `false` value রাখে

---

## 4. null

```ts
let selectedUser: null = null;
```

### Explanation:

- Intentionally empty value বোঝাতে use হয়

---

## 5. undefined

```ts
let data: undefined = undefined;
```

### Explanation:

- Variable declare করা হয়েছে কিন্তু value assign হয়নি

---

## 6. any

```ts
let info: any = "Hello";

info = 100;
info = true;
```

### Explanation:

- যেকোনো type allow করে
- Avoid করা ভালো (Type safety ভেঙে যায়)

---

## 7. unknown

```ts
let apiResponse: unknown = "TypeScript";

if (typeof apiResponse === "string") {
  console.log(apiResponse.toUpperCase());
}
```

### Explanation:

- `any` এর safer version
- আগে check না করলে use করা যায় না

---

## 8. never

```ts
function throwError(message: string): never {
  throw new Error(message);
}
```

### Explanation:

- Function কখনো return করে না
- সাধারণত error throw করলে use হয়

---

## 9. void

```ts
function printMessage(message: string): void {
  console.log(message);
}
```

### Explanation:

- Function কোনো value return করে না
