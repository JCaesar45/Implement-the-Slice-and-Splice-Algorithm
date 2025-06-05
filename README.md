````markdown
# Slice and Splice Algorithm

This project implements the `frankenSplice` function, which merges two arrays by inserting the elements of one array into another at a specified index — without modifying the original arrays.

## 📋 User Stories

- ✅ Create a function called `frankenSplice` that accepts two arrays and an index.
- ✅ Copy each element of the first array into the second array, starting at the given index.
- ✅ Return a new array with the merged values.
- ✅ The original input arrays must remain unchanged after the function is executed.

## 🚀 Function Signature

```javascript
function frankenSplice(arr1, arr2, n) {
  // Implementation
}
```

## 🧠 How It Works

* **Step 1**: Clone the second array using `.slice()` to avoid modifying the original.
* **Step 2**: Use `.splice()` with the spread operator to insert all elements of the first array at the specified index.
* **Step 3**: Return the resulting array.

## ✅ Example Usage

```javascript
frankenSplice([1, 2, 3], [4, 5], 1);
// Returns: [4, 1, 2, 3, 5]

frankenSplice(["claw", "tentacle"], ["head", "shoulders", "knees", "toes"], 2);
// Returns: ["head", "shoulders", "claw", "tentacle", "knees", "toes"]
```

## 🧪 Test Cases

| Input                                                                            | Output                                                       |
| -------------------------------------------------------------------------------- | ------------------------------------------------------------ |
| `frankenSplice([1, 2, 3], [4, 5], 1)`                                            | `[4, 1, 2, 3, 5]`                                            |
| `frankenSplice([1, 2], ["a", "b"], 1)`                                           | `["a", 1, 2, "b"]`                                           |
| `frankenSplice(["claw", "tentacle"], ["head", "shoulders", "knees", "toes"], 2)` | `["head", "shoulders", "claw", "tentacle", "knees", "toes"]` |
| `frankenSplice([1, 2, 3, 4], [], 0)`                                             | `[1, 2, 3, 4]`                                               |

## 📂 Project Structure

```
├── index.js        # frankenSplice function
├── test.js         # Optional test file (if needed)
└── README.md       # Project documentation
```

## 📌 Notes

* Uses ES6 syntax including `...` spread operator.
* Designed for clarity and functional immutability.
* Ideal for beginner algorithm practice.

## 🛠️ Technologies

* JavaScript (ES6)

## 📄 License

This project is open-source and free to use under the [MIT License](LICENSE).
