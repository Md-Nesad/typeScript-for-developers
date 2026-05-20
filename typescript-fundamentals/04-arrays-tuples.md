# 4. Arrays & Tuples

## Array of Strings

```ts
let fruits: string[] = ["apple", "banana", "mango"];
console.log(fruits);
```

### Explanation:

- শুধুমাত্র string value রাখা যাবে
- Example: names, fruits, skills

---

## Array of Numbers

```ts
let numbers: number[] = [1, 2, 3, 4, 5];
console.log(numbers);
```

### Explanation:

- শুধুমাত্র number value রাখা যাবে

---

## Array of Boolean

```ts
let flags: boolean[] = [true, false, true];
console.log(flags);
```

### Explanation:

- শুধু true/false value

---

## Mixed Array (Union Type Array)

```ts
let mixed: (string | number | boolean)[] = ["hello", 10, true, "world", 20];
console.log(mixed);
```

### Explanation:

- একাধিক type allow করা যায়
- Union type ব্যবহার করা হয়েছে

---

## Tuple Type

```ts
let user: [string, number] = ["Nesad", 25];
console.log(user);
```

### Explanation:

- Fixed order এবং fixed type থাকে
- প্রথমে string, তারপর number

---

## Tuple with Multiple Types

```ts
let response: [number, string, boolean] = [200, "Success", true];
console.log(response);
```

### Explanation:

- Fixed structure data রাখার জন্য use হয়
- API response এর মতো ক্ষেত্রে useful

---

## Array of Objects (Very Important)

```ts
type User = {
  id: number;
  name: string;
  isActive: boolean;
};

let users: User[] = [
  { id: 1, name: "Nesad", isActive: true },
  { id: 2, name: "Rahim", isActive: false },
  { id: 3, name: "Karim", isActive: true },
];

console.log(users);
```

### Explanation:

- এখানে প্রতিটি object একই structure follow করে
- Real-world API data handle করার জন্য খুব common
- Type safety নিশ্চিত করে

---
