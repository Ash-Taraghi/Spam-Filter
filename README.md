# Spam Filter

This project is a simple spam filter implemented in JavaScript. It uses regular expressions to detect common spam patterns in text messages.

## Features

- Detects variations of the phrase "free money"
- Case insensitive matching
- Handles common leetspeak variations

## Getting Started

These instructions will help you set up and run the spam filter on your local machine.

### Prerequisites

- Node.js installed on your machine (optional, if running the script in a Node.js environment)

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/spam-filter.git
   cd spam-filter
    ```
    or simply click [here](https://ash-taraghi.github.io/Spam-Filter/)

2. (optional) Install dependencies if any (for testing)


## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

### Usage

You can run the spam filter using Node.js or directly in your browser's console.

#### Node.js

1. **Create a file `spamFilter.js` and add the following code**:

   ```javascript
   const freeRegex = /(?:\s|^)fr[e3][e3] m[o0]n[e3]y(?:\s|$)/i;

   function isSpam(text) {
       return freeRegex.test(text);
   }

   // Test the spam filter
   const testMessages = [
       "Get your fr33 m0ney now!",
       "This is a limited time offer.",
       "Don't miss out on free cash.",
       "Claim your frEe M0ney!",
       "This is not a spam message."
   ];

   testMessages.forEach(message => {
       console.log(`"${message}" is spam: ${isSpam(message)}`);
   });

   ```
2. **Run the Script**

    ```javascript
    node spamFilter.js
    ```

3. **Copy and phaste this code into browser console and check console output to see spam results**

    ```javascript
    const freeRegex = /(?:\s|^)fr[e3][e3] m[o0]n[e3]y(?:\s|$)/i;

    function isSpam(text) {
        return freeRegex.test(text);
    }

    // Test the spam filter
    const testMessages = [
        "Get your fr33 m0ney now!",
        "This is a limited time offer.",
        "Don't miss out on free cash.",
        "Claim your frEe M0ney!",
        "This is not a spam message."
    ];

    testMessages.forEach(message => {
        console.log(`"${message}" is spam: ${isSpam(message)}`);
    });

    ```