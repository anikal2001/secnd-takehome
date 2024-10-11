### iOS Developer Test (4 Hours)

#### Task Overview:
Develop a **"Virtual Wardrobe" feature** for our second-hand fashion app using **SwiftUI**. This feature allows users to browse their purchased items, add new ones, and retrieve fashion categories from an external API.

---

### Part 1: Feature Implementation (3 hours)

1. **Virtual Wardrobe UI:**
   - Create a SwiftUI `List` or `LazyVGrid` to display the items in the user’s wardrobe. Each item should show:
     - A thumbnail image
     - The item’s name
     - The item’s category (e.g., shirt, pants, dress)
   - Include sorting options (by category, purchase date, brand) using a segmented control or picker.

2. **Filter Bar:**
   - Add a Horizontal Scrollable Filter Bar at the top to allow users to filter for items by Category, Brand, Size, Color, Price, and Condition. With each button toggling a dropdown (that goes over the existing content) with the respective filters. Please see following Figma link for inspiration: https://www.figma.com/design/oDpzYbov2BNirt99QiX3UA/Filter-Bar?node-id=0-1&t=uP8yeMWu3Nus74EV-1

3. **Add to Wardrobe:**
   - Create a form where users can manually add items to their wardrobe. Fields should include:
     - Image of the item (use `ImagePicker` to let users select from their photo library)
     - Item name
     - Item category (dropdown populated from API, explained below)
     - Brand name
     - Purchase date (use a `DatePicker`)
   - Validate the form to ensure all fields are completed before saving.

4. **Data Persistence:**
   - Use **Core Data** to save and persist wardrobe items across app sessions. Store the image, name, category, brand, and purchase date for each item.

---

### Part 2: API Call (1 hour)

1. **Fetch Categories from API:**
   - Make an API call to fetch fashion categories for use in the "Add to Wardrobe" form. Use this endpoint:
     - **API Endpoint:** `https://fakestoreapi.com/products/categories`
     - This will return a list of categories like `electronics`, `jewelery`, etc. (You can assume that this API returns the categories for now, though it's not fashion-specific.)
   - Populate the category dropdown dynamically with the data fetched from the API.

2. **Error Handling for API:**
   - Implement basic error handling for the API call. If the API fails to fetch the categories, show an appropriate error message and provide a fallback (e.g., use locally stored categories).

---

### Part 3: Code Quality and Problem-Solving (Optional Bonus)

1. **Code Architecture:**
   - Structure your code using the **MVVM** pattern, ensuring that networking, UI, and data models are cleanly separated.
   - Make your code modular, reusable, and easy to test.

2. **Optional Bonus:**
   - **Favorites:** Add functionality for users to mark items as "favorite" and filter their wardrobe to view only favorite items.
   - **Dark Mode:** Ensure that your app supports both light and dark modes.

---

### Submission Guidelines:
- Submit your project via GitHub (or any other version control platform).
- Provide clear instructions on how to run the app.

---
