## Enums

The enum is for when you need to be one of the many options you could have

```javascript
enum Role {
  ADMIN = 'admin,
  AUTHOR = 'author',
  READ_ONLY = 'readonly'
}

const person = {
  name: 'John Smith',
  age: 30,
  role: ROLE // this would admit only 1 of the 3 possible roles
}
```

## Types

are to define a specific shape

```javascript
type User = {
  name: string,
  age: number,
  role: Role,
};

const user: User = {
  name: "John Smith",
  age: 30,
  role: "admin",
  isActive: true, // this line would throw an error since isActive prop is not defined in type User
};
```
