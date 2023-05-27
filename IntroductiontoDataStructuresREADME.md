Introduction to Data Structures and Procedural programming checkpoint 


```javascript


// Problem 1: Sum of Distinct Elements

// Function to calculate the sum of distinct elements from two sets
function sumOfDistinctElements(set1, set2) {
  let sum = 0;

  // Iterate over elements in set1
  for (let i = 0; i < set1.length; i++) {
    // Check if the element is not present in set2
    if (!set2.includes(set1[i])) {
      // Add the element to the sum
      sum += set1[i];
    }
  }

  // Iterate over elements in set2
  for (let i = 0; i < set2.length; i++) {
    // Check if the element is not present in set1
    if (!set1.includes(set2[i])) {
      // Add the element to the sum
      sum += set2[i];
    }
  }

  // Return the sum of distinct elements
  return sum;
}

// Example usage
const set1 = [3, 1, 7, 9];
const set2 = [2, 4, 1, 9, 3];
const sum = sumOfDistinctElements(set1, set2);
console.log(sum); // Output: 13


// Problem 2: Orthogonal Vectors

// Function to calculate the dot product of two vectors
function dotProduct(v1, v2) {
  let ps = 0;

  // Iterate over elements in v1 and v2
  for (let i = 0; i < v1.length; i++) {
    // Calculate the dot product
    ps += v1[i] * v2[i];
  }

  // Return the dot product
  return ps;
}

// Function to determine if two vectors are orthogonal
function orthogonalVectors(vectors) {
  // Iterate over pairs of vectors
  for (let i = 0; i < vectors.length; i += 2) {
    const v1 = vectors[i];
    const v2 = vectors[i + 1];

    // Calculate the dot product of v1 and v2
    const ps = dotProduct(v1, v2);

    // Check if the dot product is zero (orthogonal) or not
    if (ps === 0) {
      console.log(`Vectors ${v1} and ${v2} are orthogonal`);
    } else {
      console.log(`Vectors ${v1} and ${v2} are not orthogonal`);
    }
  }
}

// Example usage
const vectors = [
  [1, 2, 3],
  [4, 5, 6],
  [1, 0, 0],
  [0, 1, 0],
  [1, 1, 1],
  [1, -1, 0],
];
orthogonalVectors(vectors);
```
