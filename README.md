# book_price_tracker

## Overview

The **Book Price Tracker** is a UiPath automation project designed to monitor the prices of your favorite books. The user provides URLs for the books and a maximum price threshold. The automation checks the current prices and alerts the user via email if any of the book prices drop below the specified threshold. Additionally, the price information is recorded in a local Excel file for reference.

## Features

- **URL Input**: The user can input URLs for multiple books in a text box, separating them with a comma.
- **Price Threshold Input**: The user specifies the maximum price they are willing to pay for the books.
- **Price Monitoring**: The automation navigates to each URL provided and checks the current price of the book.
- **Price Comparison**: If the current price is below the threshold, the book's information is logged and saved.
- **Email Notification**: The user receives an email notification with details about the books whose prices are below the threshold.
- **Data Logging**: The price data is saved to an Excel file on the user's local machine.

## Workflow Breakdown

1. **Input Dialog for URLs**:
   - Prompts the user to input the URLs of the books they want to track.
   - The URLs are then split and stored in a list for further processing.

2. **Input Dialog for Price Threshold**:
   - Prompts the user to input the maximum price they are willing to pay for the books.

3. **For Each URL**:
   - The workflow iterates through each URL, opening the corresponding webpage in a browser.

4. **Price Extraction**:
   - The current price of the book is extracted from the webpage.
   - The extracted price is cleaned and formatted for comparison.

5. **Price Comparison**:
   - If the extracted price is below the specified threshold, the book's details are stored.

6. **Data Logging & Email Notification**:
   - The information is added to an Excel file, and an email is sent to the user, notifying them of the price drop.

## Requirements

- **UiPath Studio**: Ensure you have UiPath Studio installed.
- **Excel Application**: Microsoft Excel should be installed for data logging.
- **Outlook**: An Outlook account configured in UiPath for sending email notifications.

## How to Use

1. **Run the Project**: Open UiPath Studio and run the project.
2. **Input URLs**: When prompted, enter the URLs of the books you want to monitor, separated by commas.
3. **Set Price Threshold**: Enter the maximum price you're willing to pay for each book.
4. **Wait for Results**: The automation will notify you via email if any book's price is below your specified threshold.
5. **Check Excel File**: Review the Excel file saved on your local machine for detailed price information.

## Conclusion

The **Book Price Tracker** simplifies the process of monitoring book prices online, ensuring that you never miss out on a deal. With automatic email notifications and detailed logging, you can stay updated on price changes without the hassle of manually checking each site.
