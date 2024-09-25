## Overview:
Create a simple mobile app (in Swift for iOS or Kotlin for Android) that fetches data from an external API and displays it on a second screen when a button is clicked. The goal is to evaluate basic mobile development skills, including API calls, navigation, and UI handling.

---

## Tasks:

1. **Set Up the Project**:
    - Create a new mobile project
        - Use Swift (iOS) or Kotlin (Android).
    - Use any tools you usually would for code quality, linting, formatting, testing etc.

2. **UI - First Screen**:
    - The first screen should contain:
        - A title: "Our Products"
        - A list of products generated from the `https://dummyjson.com/products` API.
        - These should all be individually clickable buttons that take you to the second screen detailed below
     
3. **UI - Second Screen**:
    - The second screen should contain:
        - A title: <the product name>
        - Details of the product selected -- This can either be passed in from the first screen or retrieved from the following API `https://dummyjson.com/products/<productId>`
            - Please include:
                - the image of the product from the API response
                - a description of the product
                - The price of the product
                - The shipping information for the product
                - A button to add the product to a basket.

---

## Bonus Tasks:

1. **Loading Indicator**:
    - Show a loading indicator when any API call is in progress.

2. **Error Handling**:
    - Display a toast message if any API call fails, with a retry option.

3. **UI Enhancements**:
    - Display reviews on the second screen.
    - Improve the layout with additional styling and visual elements.
