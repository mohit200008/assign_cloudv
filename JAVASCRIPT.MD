2.JAVASCRIPT
A->
function reverseWordsInSentence(sentence) {
    const words = sentence.split(" ");
    const reversedWords = words.map(word => reverseWord(word));
    const reversedSentence = reversedWords.join(" ");
    return reversedSentence;
}

function reverseWord(word) {
    return word.split("").reverse().join("");
}

const inputSentence = prompt("Enter a sentence:"); 
const reversedSentence = reverseWordsInSentence(inputSentence);
console.log("Reversed sentence:", reversedSentence);

B->
function bubbleSortDescending(arr) {
    const n = arr.length;
    for (let i = 0; i < n - 1; i++) {
        for (let j = 0; j < n - i - 1; j++) {
            if (arr[j] < arr[j + 1]) {
                const temp = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = temp;
            }
        }
    }
    return arr;
}

const numbers = [5, 2, 9, 1, 5, 6];
const sortedDescending = bubbleSortDescending(numbers);

console.log(sortedDescending);


