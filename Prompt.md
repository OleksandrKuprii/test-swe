Create an algorithm that accepts a single string input (a compound word) and breaks it down into its constituent words based on a predefined dictionary. The algorithm should be able to process an array of compound words and return the breakdown for each, matching the expected output provided in the tests.

Requirements
Implement the findWords function that takes a string as input and returns an array of strings, representing the constituent words as per the dictionary provided.
You must ensure the algorithm is efficient and able to handle the provided test cases, returning the exact match of expected output.
Evaluation Criteria
Correctness: The submitted solution must pass all the provided test cases.
Efficiency: The algorithm should minimize computational time and memory usage.
Code Quality: The code should be well-organized, commented, and easy to read.
Scalability: While the provided dictionary is fixed for the tests, the solution should be adaptable to changes in the dictionary size.

Example test cases

```
const dictionary = [
"assembly",
"hall",
"of",
"ass",
"the",
"theo",
"t",
"okt",
"oktober",
"fest",
"oktoberfest",
"top",
"3d",
"ent",
"ist",
"3",
"dentist",
"fashion",
"u",
"vco",
"nv",
"ers",
"ion",
"weight",
"losss",
"loss",
"software",
];


const tests = [
{ word: "oefiassemblyhall", expected: ["assembly", "hall"] },
{ word: "theoktoberfest", expected: ["the", "oktoberfest"] },
{ word: "top3dentists", expected: ["top", "3", "dentists"] },
{ word: "ufashion", expected: ["u", "fashion"] },
{ word: "vconversion", expected: ["conversion"] },
{ word: "weightlosssoftware", expected: ["weight", "loss", "software"] },
];


for (const test of tests) {
expect(findWords(test.word)).to.equal(test.expected);
}

```
