# SpliteEase

A bill-splitting application to track shared expenses in a group, developed with Node.js, Express, MongoDB, and React.

## Explanation of Transaction Minimization Algorithm

We implemented a greedy algorithm to minimize the number of transactions required to settle the debts between all members of a group when the user toggles 'Smart Split'. The algorithm runs in **O(n log n)**, where **n** is the number of users—this ensures scalability as the number of users increases.

A simple example of this algorithm is shown below. In this example, Alice owes Bob $10, and Bob owes Charlie $10 for a total of two transactions. The algorithm will suggest that Alice pays Charlie $10 directly, reducing it to one transaction.

![SpliteEase - Minimizing Transactions](https://user-images.githubusercontent.com/47993930/193157219-12522cfb-f831-48d3-9140-bf1cab09d3b5.png)

For larger groups, the optimization becomes even more significant. The following diagram demonstrates a scenario where six users initially have six transactions. The algorithm reduces this to only four transactions.

![SpliteEase - Complex Minimization](https://user-images.githubusercontent.com/47993930/193157096-98f00f14-8548-4093-a213-8e8975a6e036.png)

---

## Features

- **Group Expense Tracking**: Easily add and manage shared expenses.
- **Smart Split Algorithm**: Reduces the number of transactions needed for settlement.
- **User-Friendly Interface**: A clean and modern UI for effortless navigation.
- **Real-Time Updates**: Syncs expenses and debts instantly.
- **Multiple Currencies Support**: Manage expenses in various currencies.

---

## Screenshots


![image](https://github.com/user-attachments/assets/321ba2a0-c634-476b-89f2-60426f5303c5)


---

## Installation and Usage

### Setting Up MongoDB Database

1. Create a file in the `server` directory named: `.env`
2. Open the file in a text editor and add the following line, replacing `<uri>` with your MongoDB URI:

```txt
MONGODB_URI="<uri>"
```

3. Save the file.

### Running the Server

1. Open a terminal window.
2. Navigate to the project root directory: `cd SpliteEase`
3. Go to the server directory: `cd server`
4. Install dependencies: `npm install`
5. Run the server: `node app`

### Running the Client

1. Open a new terminal window.
2. Navigate to the client directory: `cd client`
3. Install dependencies: `npm install`
4. Start the client: `npm start`
5. Open the provided URL in your browser.

---

## Running Tests

### Running Server Tests

1. Open a terminal window.
2. Navigate to the server directory: `cd server`
3. Install dependencies: `npm install`
4. Run tests: `npm test`

---

## Future Enhancements

- **OAuth Integration**: Sign in with Google/Facebook for quick access.
- **Expense Categorization**: Label expenses for better tracking.
- **Recurring Expenses**: Automate monthly bill payments.
- **Mobile App**: Native iOS and Android support.

---
## Contact
For any questions or feedback, feel free to reach out to [yuvrajsogarwal@gmail.com].

---

Enjoy using **SpliteEase** and simplify your group expenses effortlessly! 🎉
