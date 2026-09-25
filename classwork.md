# Classwork - Objects & Arrays 🧩

## Task 1 - Student Profile 🎓

მოცემულია სტუდენტების სია:

```js
const students = [
  {
    name: "Nika",
    age: 19,
    city: "Tbilisi",
    score: 87,
    isActive: true,
  },
  {
    name: "Ana",
    age: 21,
    city: "Batumi",
    score: 94,
    isActive: true,
  },
  {
    name: "Giorgi",
    age: 18,
    city: "Kutaisi",
    score: 68,
    isActive: false,
  },
];
```

### დავალებები

1. კონსოლში გამოიტანე პირველი სტუდენტის სახელი.

```js
// მოსალოდნელი შედეგი:
// Nika
```

2. გამოიტანე მეორე სტუდენტის ქალაქი.

3. გამოიტანე მესამე სტუდენტის ქულა.

4. გამოიტანე პირველი სტუდენტი მთლიანად.

5. `if / else`-ის გამოყენებით შეამოწმე:

თუ `Ana`-ს ქულა მეტია ან ტოლია `90`-ზე:

```txt
Excellent result
```

სხვა შემთხვევაში:

```txt
Keep practicing
```

6. შეამოწმე არის თუ არა `Giorgi` აქტიური სტუდენტი.

თუ `isActive === true`:

```txt
Student is active
```

სხვა შემთხვევაში:

```txt
Student is inactive
```

---

# Task 4 - Online Shop 🛒

აქ ობიექტში კიდევ ერთი ობიექტი გვაქვს.

```js
const products = [
  {
    name: "MacBook Air",
    price: 3200,
    stock: 4,
    details: {
      color: "Midnight",
      storage: "256GB",
    },
  },
  {
    name: "iPhone",
    price: 2500,
    stock: 0,
    details: {
      color: "Black",
      storage: "128GB",
    },
  },
  {
    name: "AirPods",
    price: 550,
    stock: 12,
    details: {
      color: "White",
      storage: undefined,
    },
  },
];
```

### დავალებები

1. გამოიტანე `MacBook Air`-ის ფასი.

2. გამოიტანე `iPhone`-ის ფერი.

```txt
Black
```

3. გამოიტანე `MacBook Air`-ის მეხსიერება.

```txt
256GB
```

4. გამოიტანე `AirPods`-ის `storage`.

რა მნიშვნელობას მიიღებ?

5. შეამოწმე `iPhone`-ის `stock`.

თუ `stock > 0`:

```txt
Available
```

სხვა შემთხვევაში:

```txt
Out of stock
```

6. თუ `MacBook Air`-ის ფასი მეტია `3000`-ზე:

```txt
Expensive product
```

სხვა შემთხვევაში:

```txt
Good price
```

---

# Task 6 - Destructuring 🧨

მოცემულია:

```js
const user = {
  username: "CodeMaster",
  age: 22,
  city: "Tbilisi",
  profession: "Developer",
};
```

### 1.

Destructuring-ის გამოყენებით შექმენი:

```js
username;
age;
```

ცვლადები.

შემდეგ გამოიტანე ორივე კონსოლში.

### 2.

Destructuring-ის გამოყენებით ამოიღე:

```js
city;
profession;
```

### 3.

`user.city`-ის გამოყენების გარეშე შეამოწმე:

თუ `city === "Tbilisi"`:

```txt
Lives in Tbilisi
```

სხვა შემთხვევაში:

```txt
Lives somewhere else
```

---

# Task 7 - Array Destructuring 📦

```js
const technologies = ["JavaScript", "React", "Node.js", "PostgreSQL"];
```

### დავალებები

1. Array destructuring-ის გამოყენებით შექმენი:

```js
firstTechnology;
secondTechnology;
```

მოსალოდნელი მნიშვნელობები:

```js
firstTechnology; // JavaScript
secondTechnology; // React
```

2. პირველი ორი ელემენტის გამოტოვებით ცვლადში შეინახე:

```txt
Node.js
```

3. destructuring-ის გამოყენებით ცალკე ცვლადებში შეინახე ოთხივე ტექნოლოგია.

---

```js
const cars = [
  {
    brand: "Tesla",
    model: "Model Y",
    year: 2021,
    price: 8500,
    specs: {
      fuel: "Electric",
      drive: "AWD",
    },
  },
  {
    brand: "BMW",
    model: "330i",
    year: 2020,
    price: 10500,
    specs: {
      fuel: "Petrol",
      drive: "RWD",
    },
  },
  {
    brand: "Hyundai",
    model: "Ioniq 5",
    year: 2022,
    price: 9200,
    specs: {
      fuel: "Electric",
      drive: "RWD",
    },
  },
];
```

### დავალებები

1. გამოიტანე Tesla-ს მოდელი.

2. გამოიტანე BMW-ს `drive`.

3. გამოიტანე Hyundai-ს `fuel`.

4. შეადარე Tesla-სა და Hyundai-ს ფასი.

გამოიტანე რომელი უფრო იაფია.

5. შეამოწმე Tesla:

თუ:

```js
year >= 2021;
```

და:

```js
specs.fuel === "Electric";
```

გამოიტანე:

```txt
Modern electric car ⚡
```

სხვა შემთხვევაში:

```txt
Does not match
```

6. Destructuring-ის გამოყენებით პირველი მანქანიდან ამოიღე:

```js
brand;
model;
price;
```

7. Nested destructuring-ის გამოყენებით პირველი მანქანიდან ამოიღე:

```js
fuel;
drive;
```

ისე, რომ შემდეგ შეგეძლოს პირდაპირ დაწერო:

```js
console.log(fuel);
console.log(drive);
```

---

```js
const candidates = [
  {
    name: "Luka",
    age: 17,
    score: 91,
    hasLaptop: false,
  },
  {
    name: "Mariam",
    age: 20,
    score: 88,
    hasLaptop: true,
  },
];
```

ლეპტოპის მისაღებად სტუდენტი უნდა აკმაყოფილებდეს ორივე პირობას:

```txt
score >= 90
```

და

```txt
hasLaptop === false
```

შეამოწმე `Luka`.

თუ ორივე პირობა სრულდება:

```txt
Luka gets the laptop 💻
```

სხვა შემთხვევაში:

```txt
Luka does not qualify
```

შემდეგ იგივე პირობა შეამოწმე `Mariam`-ზე.

**მთავარი პირობა:** არ გამოიყენო `function`, loop ან ისეთი მეთოდები, რომლებიც ჯერ არ გვასწავლია. გამოიყენე მხოლოდ Array/Object-ზე წვდომა, ცვლადები, `if / else`, შედარების ოპერატორები, logical operators და destructuring.
