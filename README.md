# Gadget Gear Hub - A Tourism Management Website

Live Link: [Gadget Gear Hub](https://gadget-gear-hub.web.app/)

---

## **Overview**

Welcome to **Gadget Gear Hub**, a tourism management website tailored to showcase and explore tourist spots from Middle Eastern countries. The platform enables users to view, add, update, and manage information about fascinating travel destinations with ease.

---

## **Features**

### **1. Navbar**
- Includes the **Website Name/Logo** and navigation links:
  - **Home**
  - **All Tourists Spots**
  - **Add Tourist Spot** *(Private/Protected Route)*
  - **My List** *(Private/Protected Route)*
  - **Login** and **Register** (conditional display)
  - If logged in:
    - Shows the **user's photo** (on hover, displays the username).
    - Includes a **Log Out** button.

### **2. Home Page**
- A **Banner/Slider Section** showcasing videos of popular Middle Eastern travel spots.
- A **Country Slider Section** displaying tourist spots from various Middle Eastern countries.
- Includes:
  - **Tourist Spots Section**: Cards for tourist spots with details fetched from the database.
  - **Two Extra Sections**: Highlight meaningful travel-related information.
  - **Dark/Light Mode Toggle** for theme switching.

### **3. Tourist Spots Management**
- **All Tourist Spots Page**:
  - Displays cards with:
    - Spot image
    - Name
    - Location
    - Cost
    - Visitors per year
    - Travel time
    - Seasonality
    - "View Details" button (redirects to the details page).
  - Sorting functionality based on "Average Cost."
- **Add Tourist Spot Page** *(Private Route)*:
  - Allows users to add a spot by filling out a form:
    - Image URL, Name, Country, Location, Description, Cost, Visitors per year, Travel time, Seasonality, User Email, and Name.
    - Success notification on submission.
- **My List Page** *(Private Route)*:
  - Displays spots added by the user in a table with:
    - Spot details
    - **Update** and **Delete** buttons.
- **Update Tourist Spot** *(Private Route)*:
  - Editable form or modal to update tourist spot information.
  - Success notification upon update.
- **Delete Tourist Spot**:
  - Confirmation prompt before deletion.
  - Removes the selected spot from the database.

### **4. View Details Page**
- Provides detailed information for a tourist spot.
- **Protected Route**: Redirects unauthenticated users to the login page.

### **5. Authentication**
- **Login Page**:
  - Email/Password-based login.
  - Social login options (Google, Facebook, etc.).
  - Redirect link to the Register page.
  - Error handling using toasts/alerts for invalid credentials.
- **Register Page**:
  - User registration with:
    - Name, Email, Photo URL, Password.
    - Password must meet specific criteria (uppercase, lowercase, 6+ characters).
    - Success notification upon registration.

### **6. Countries Section**
- Displays cards for six Middle Eastern countries:
  - Country Name
  - Image
  - Short Description.
- Clicking a country card redirects to a page displaying all tourist spots for that country.

### **7. Additional Pages**
- **404 Page**: Displays a "Page Not Found" message for invalid routes.
- **Footer**:
  - Website name, copyright information, contact details, and social media links.

---

## **Technologies Used**

### **Frontend**
- **React.js**: For a dynamic and interactive UI.
- **Tailwind CSS**: For responsive and modern styling.
- **Firebase**: Authentication and hosting.

### **Backend**
- **Node.js** with **Express.js**: For API creation.
- **MongoDB**: Database to store tourist spot data.

### **Third-Party Libraries**
- **Lottie React**: For animations.
- **React Awesome Reveal**: For animated content transitions.
- **React Toastify**: For user notifications.

---

## **Deployment**

### **Hosting**: 
- **Frontend**: Hosted on Firebase.
- **Backend**: Hosted on Render/Heroku.

### **Steps to Run Locally**

#### **Frontend**
1. Clone the client-side repository:
   ```bash
   git clone <client-repo-url>
   cd client
   npm install
   npm start
