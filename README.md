# Currency-converter
Currency Converter is a web app built with HTML, CSS, and JavaScript that allows users to convert one currency to another. It uses live exchange rates fetched from an API, providing real-time conversions. The app features a clean, user-friendly interface for easy and accurate currency conversion.


# Currency Converter

## Description
This is a simple **Currency Converter** web application built using **HTML**, **CSS**, and **JavaScript**. It allows users to convert one currency to another by providing the amount in the base currency and selecting the target currency. The conversion uses live exchange rates fetched from a public API.

## Features
- **Live Exchange Rates**: Fetches up-to-date exchange rates for currency conversion.
- **User-friendly Interface**: Simple and clean design using HTML and CSS.
- **Multiple Currency Support**: Supports a variety of currencies for conversion.

## Technologies Used
- **HTML**: Structure of the web page.
- **CSS**: Styling of the web page for a clean and responsive design.
- **JavaScript**: Fetching live exchange rates and performing the conversion logic.

## Steps to Run the Project Locally

1. **Clone the Repository**:
   First, clone the repository to your local machine using Git. Run the following command in your terminal:
   bash:
   git clone https://github.com/vaibhav-araikar/currency-converter.git
2. **Navigate to the Project Directory:** After cloning the repository, go to the project folder:
    cd currency-converter
3. **Open the index.html File:** You can open the index.html file in any modern web browser (such as Chrome, Firefox, etc.):
   open index.html  # on Mac
   start index.html # on Windows
4. **Using the Currency Converter:**
   - Enter the amount you want to convert.
   - Select the base currency (the currency you are converting from).
   - Select the target currency (the currency you want to convert to).
   - The conversion rate and result will be shown automatically.
5. **Enjoy**
   That's it! You should now be able to use the currency converter on your local machine.



**Instructions for Handling API Issues in Currency Converter**
Thank you for using the Currency Converter! Occasionally, the API we rely on to fetch currency exchange rates may face issues, such as downtime, rate limit restrictions, or service changes. To ensure that your currency conversion remains accurate and functional, we recommend trying alternative APIs.
**Steps to Use Alternative Currency Conversion APIs:**
1. **Check for API Issues:**
   - If you notice that the currency conversion isn't working or the exchange rates seem outdated, the first step is to check if the current API is down. This could be due to a temporary service outage or rate         limit restrictions.
   - If possible, try reloading the page or restarting the application to see if the issue resolves on its own.
2. **Update API Key:**
   - Many APIs require an API key for access. If you have received an API key from a provider, make sure it's up to date. If the key is expired or invalid, you will need to request a new one from the API provider.
3. **Try Alternative APIs:** If the current API is causing issues or you want to explore other reliable options, here’s a list of alternative APIs you can integrate into the application for fetching accurate currency rates:
   - ExchangeRate-API: A simple API offering free and paid plans for currency conversion.
   - Fixer.io: A popular API that provides real-time foreign exchange rates for 170 world currencies. Offers both free and premium plans.
   - CurrencyLayer: A robust API with support for over 170 currencies and historical data.
   - Open Exchange Rates: This API provides exchange rates and currency data, with free and paid options.
   - XE Currency Data API: A well-known and reliable currency conversion API that offers both real-time and historical exchange rates.
4. **Modify API Integration in Your Code:**
   - Update the API endpoint URL and API key in your project to the new provider’s details. Make sure to check the documentation of the selected API for correct implementation.
   Example of updating API URL:
   const apiURL = "https://api.exchangerate-api.com/v4/latest/USD"; // Change this URL to the new API endpoint
5. **Handle API Errors Gracefully:**
   - Implement error handling in your code to deal with potential API failures. This could include displaying a friendly error message to the user or attempting to switch to a secondary API if the primary one fails.
   - Example in JavaScript:
   try {
    const response = await fetch(apiURL);
    if (!response.ok) {
        throw new Error("API error: Unable to fetch exchange rates");
    }
    const data = await response.json();
    // Process the data...
} catch (error) {
    console.error(error.message);
    alert("There was an issue with the currency data. Please try again later.");
}
6. **Monitor API Usage:**
   - Be aware of any rate limits imposed by the API provider, especially if you're using a free plan. Some providers have limits on the number of requests you can make per minute, hour, or day.
7. **Stay Updated on API Changes:**
   - Regularly check the API provider’s documentation for updates or changes to their endpoints, authentication methods, or pricing plans. If the API provider makes major changes, you may need to update your project accordingly.
   - By following these instructions and keeping an eye on the API’s performance, you'll be able to avoid disruptions and continue enjoying smooth currency conversion functionality in your project.









   
