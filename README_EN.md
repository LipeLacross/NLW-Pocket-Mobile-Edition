## 🌐 [Versão em Português do README](README.md)

# Nearby

Nearby is an application developed in React Native using Expo Router. Its goal is to provide an experience that allows users to explore and activate coupons in nearby partner locations. The app integrates interactive maps, categories, and detailed information about places with available coupons.

## 🔨 Project Features

- View nearby establishments on an interactive map.
- Navigate between categories of places.
- Redeem coupons via QR Code.
- Detailed information about locations, including address, phone, and available coupons.
- Rules for using coupons.

### Visual Example of the Project

![image](https://github.com/user-attachments/assets/28fd4ae2-4413-4a61-af1c-be876e6b8fe2)
![image](https://github.com/user-attachments/assets/668e46ec-e4a7-4976-adda-6e26001fe502)
![image](https://github.com/user-attachments/assets/6b614059-ff66-4a91-9cfe-ebcd720c4e7f)

## ✔️ Techniques and Technologies Used

- **React Native**
- **Expo Router** for navigation.
- **Axios** for API consumption.
- **Tabler Icons** for custom icons.
- **Expo Camera** for QR Code scanning.
- **React Native Maps** for rendering the interactive map.
- **Prisma** as an ORM for database management.
- **SQLite** as the local database for development.

## 🗁 Project Structure

- **assets/**
    - **images/**: Contains icons and images like `splash.png` and `icon.png`.
    - Other graphical resources for the app.
- **api/**
    - **prisma/**: Contains database configuration files, including the schema and migrations.
    - **src/**: Includes controllers, middleware, and the Express server.
    - **seed.ts**: Script to populate the database with initial data.
- **src/**
    - **app/**: Contains the main routes and screens of the app.
    - **components/**: Reusable components like buttons, lists, and maps.
    - **services/**: API connection setup.
    - **styles/**: Global style files like colors and font families.
    - **utils/**: Helper functions and icons for categories.

Detailed Example:

- **src/app/home.tsx**: Main screen displaying the map and places.
- **src/app/market/[id].tsx**: Detailed screen for a specific location.
- **src/components/button/**: Reusable custom buttons.
- **src/styles/theme.ts**: Theme configurations with colors and fonts.
- **api/seed.ts**: Script to populate the database with initial data, including categories, markets, and rules.

## 🛠️ Running the Project Locally

To run the project locally, follow these steps:

1. **Ensure Node.js is installed**:
    - [Node.js](https://nodejs.org/) is required to run the project. You can check if it's already installed by running:
      ```bash
      node -v
      ```
    - If not installed, download and install the recommended version.

2. **Clone the Repository**:
    - Copy the repository URL and run the following command in the terminal:
      ```bash
      git clone <REPOSITORY_URL>
      ```

3. **Install Dependencies**:
    - Navigate to the project directory and run:
      ```bash
      npm install
      ```

4. **Set up and start the backend**:
    - Navigate to the `api` directory:
      ```bash
      cd api
      ```
    - Generate the necessary Prisma client for the database:
      ```bash
      npx prisma generate
      ```
    - Run the following command to start the backend:
      ```bash
      npm run start
      ```

5. **Start the mobile app**:
    - Navigate to the `mobile` directory:
      ```bash
      cd mobile
      ```
    - Run the following command:
      ```bash
      npx expo start
      ```

6. **Access the application**:
    - Use the Expo Go app to scan the generated QR Code.
    - Or run the application on an Android emulator (e.g., Android Studio).

## 📚 Supporting Material

- Additional Documentation: [NLW Mobile Guide](https://docs-rocketseat.notion.site/NLW-Mobile-149395da577080a398d5dde2d90321ad)
