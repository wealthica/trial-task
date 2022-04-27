Your day to day job at Vezgo would mostly consist of writing "connectors": connectors retrieve balances, holdings and transactions from various crypto wallets, enrich this data and return it in a unified format. 

In our trial task we suggest you to write a simplified version of a connector for the Ethereum network. You're free to choose any available data source, but you will need to explain what made you to choose it from all the others.

# Task 

For us, an Ethereum wallet consists of balance (in ETH), positions (ERC20 tokens) and transactions (both native and ERC20). You will need to accept a wallet as parameter, fetch its balance, posititions and transactions from somewhere and return a JSON as an output. Feel free to structure the returned data in a way which makes most sense for you. In the end your solution should be returning something like this, but not necessarily in this exact format:

```
{ 
  balance: 3.81,
  positions: [ 
    { symbol: "USDT", quantity: 1200 },
    { symbol: "WBTC", quantity: 0.45 },
    ...
  ],
  transactions: [...]
}
```

Bonus points for providing USD equivalents for the values above. Think of where and how to fetch the relevant exchange rates.

# Deliverable 

Implement code that would meet the needs of the description above. Feel free to organize it by files/modules as you prefer. We strongly recommend at least separating functions for balance, positions and transactions.

Then write the test script which will call the implementation and print the returned JSON. Test script should accept "--wallet" parameter and be executable from CLI.

Please push your submission to GitHub and provide us with the repository link.

# Assessment

Your submission will mostly be assessed on code quality, readability, and attention to corner cases. 

And it should work, too :slightly_smiling_face: 
