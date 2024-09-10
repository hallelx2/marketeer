Marketeer
=========

**Marketeer** is a web application designed to help users gain valuable insights into the market and make informed marketing decisions. By entering a product link from Amazon or Alibaba, Marketeer will scrape, store, and track the product information, enabling users to monitor price changes and discover similar products. The app sends email notifications whenever there is a price change, making it easier to keep track of important updates.

Features
--------

-	**Product Scraping**: Input product links from Amazon or Alibaba, and the app will scrape essential details such as the product title, current price, discount rates, and more.

-	**Product Tracking**: Keep track of a specific product's price over time and receive email alerts when the price changes.

-	**Similar Product Search**: Marketeer can search for products similar to the one you provided, helping users find competitive options.

-	**Email Notifications**: When a product's price changes, the app will automatically send an email alert to the user.

-	**Automated Tasks**: Cron jobs are used to regularly check product information and perform updates without manual intervention.

Tech Stack
----------

-	**Next.js**: The main framework used to build the web application.

-	**Playwright TS**: A powerful web scraping tool for automating the process of fetching data from Amazon and Alibaba product pages.

-	**Cheerio**: A parsing library used to extract the necessary product data from the scraped HTML pages.

-	**Email Sending**: Integrated email service for sending notifications to users when product prices change.

-	**Cron Jobs**: Automated scheduled tasks that check product prices periodically and send email notifications.

-	**Authentication**: Secure user authentication to ensure only authorized users can access and manage their tracked products.

Getting Started
---------------

### Prerequisites

Before you begin, make sure you have the following installed:

-	Node.js
-	npm or yarn
-	Git

### Installation

1.	Clone the repository:

	```bash
	git clone https://github.com/your-username/marketeer.git
	```

2.	Navigate to the project directory:

	```bash
	cd marketeer
	```

3.	Install dependencies:

	```bash
	npm install
	```

4.	Set up environment variables by creating a `.env` file:

	```bash
	touch .env
	```

Add the necessary environment variables for email services, cron jobs, and database configuration.

1.	Run the application:

	```bash
	npm run dev
	```

### Usage

-	Enter a product URL from Amazon or Alibaba.
-	Track product price changes automatically.
-	Receive email notifications on price changes.

### Running Cron Jobs

Cron jobs are used to automate product tracking and price updates. Make sure to set up your cron jobs properly by configuring the required time intervals in your `.env` file.

Contributing
------------

We welcome contributions to Marketeer! Please submit a pull request or open an issue to discuss the changes you would like to make.

License
-------

This project is licensed under the MIT License.
