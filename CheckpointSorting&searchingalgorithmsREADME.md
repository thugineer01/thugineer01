Checkpoint Sorting and searching algorithm 

This JavaScript repository features a concise and effective implementation of the Insertion Sort algorithm. By iteratively inserting each element into its rightful place within the sorted portion of the array this sorting function guarantees a return of integers in ascending order using the `insertionSort` function. This implementation optimizes two counters to effectively navigate through both unsorted and sorted portions of the provided array. 


  In addition to its efficiency this algorithm also provides well documented comments throughout for greater accessibility and comprehension ensuring that developers from all levels will find it easy to understand. To utilize this function simply call `insertionSort` with an array of integers as input. It will return your sorted array in no time at all! Here is an example:
  

function insertionSort(arr) {
  for (let i = 1; i < arr.length; i++) {
    let key = arr[i];
    let j = i - 1;
    
    while (j >= 0 && arr[j] > key) {
      arr[j + 1] = arr[j];
      j--;
    }
    
    arr[j + 1] = key;
  }
  
  return arr;
}

// Example usage
let arr = [5,2,4,6,1,3];
let sortedArr = insertionSort(arr);
console.log(sortedArr);


Finally lets get started with Insertion Sort! You can install and run this algorithm by following these steps:

1) Clone our repository right onto your local machine. 

  2) Once cloned locally open up index.html in your web browser of choice. 3) No additional dependencies are needed as we handcrafted plain JavaScript. 
