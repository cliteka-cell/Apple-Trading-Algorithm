# Apple Stock Strategy and SQL Database

This is a project I built to track Apple (AAPL) stock trends and save my trade ideas into a database.

### What it does:
* **The Math:** I used three moving averages (30-day, 50-day, and 120-day) to find the best times to buy or sell. 
* **The Logic:** The code only triggers a "Buy" if the short-term trend and the long-term trend both look good at the same time. This helps avoid bad trades when the market is just being noisy.
* **Saving Data:** Instead of just showing the results on a screen, the code automatically sends every signal to a SQL database (SQLite). This way, I have a permanent history of every trade the algorithm suggested.
* **Testing:** I added a section to check how much money the strategy would have made compared to just holding the stock normally.

### How to use the data:
Since everything is in SQL, you can run simple commands to find specific trades. For example:
"Find all buy signals for Apple where the price was above $200."

### Tools I used:
* Python (Pandas and Matplotlib)
* SQL (SQLite)
* Yahoo Finance API
