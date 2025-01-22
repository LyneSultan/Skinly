<img src="./readme/title1.svg"/>

<br><br>

<!-- project philosophy -->
<img src="./readme/title2.svg"/>

###

> Skinly is an app that provides users with a personalized skincare experience by detecting skin type, analyzing the compatibility of ingredients with skin types, and searching for products across multiple platforms.


### User Stories
#### User

- As a user, I want to upload an image of my face, so I can detect my skin type.

- As a user, I want to scan product ingredients, so I can see if they are suitable for my skin type.

- As a user, I want to compare products across multiple online platforms to purchase the best skincare products.


#### Company
- As a company, I want to see my products listed on the platform.

- As a company, I want to add advertisements for my products to increase visibility and sales.

- As a company, I want to preview my advertisements before publishing them to ensure accuracy and appeal.


#### Admin
- As an admin, I want to add and remove companies to manage partnerships effectively.

- As an admin, I want to see the percentage and numbers of users engaging with the platform.

- As an admin, I want to manage users to ensure a smooth and secure experience.

<br><br>
<!-- Tech stack -->
<img src="./readme/title3.svg"/>

###  Here's a brief high-level overview of the tech stack the app uses:

- This project utilizes [React Native](https://reactnative.dev/) with [Expo](https://expo.dev/) for app development. React Native is a powerful JavaScript library that enables the creation of cross-platform mobile applications using a single codebase for both iOS and Android. Expo enhances the development experience by offering a suite of tools and services to streamline building, testing, and deploying apps efficiently.

- For persistent storage (database), the app uses [MongoDB](https://www.mongodb.com/), a NoSQL database, which allows us to store and manage flexible and scalable data structures.

- To handle backend routes and API calls, the app primarily uses [Nest.js](https://nestjs.com/), a progressive Node.js framework for building efficient, reliable and scalable server-side applications.

- [Docker](https://www.docker.com/) is used to containerize the server, ensuring consistent environments for development and deployment, simplifying scaling, and improving overall application reliability.

- [Django](https://www.djangoproject.com/) is utilized for specific functionalities, including OCR and detecting the user’s skin type using a trained model.

- [EasyOcr](https://github.com/JaidedAI/EasyOCR) an open-source Optical Character Recognition (OCR) library is utilized to extract text from images or scanned documents.

- [OpenCV](https://opencv.org/), a popular computer vision library, is used for face detection. It utilizes the pre-trained classifier model to detect face counting in images.

- The app uses [ React Native Paper](https://reactnativepaper.com/) for the design and front-end components, providing a modern, and accessible user interface based on Material Design principles.

- The app integrates [OpenAI](https://openai.com/) for AI-powered features enhancing user interaction.

- [String-Similarity](https://www.npmjs.com/package/string-similarity-js) is used to improve product search functionality by matching similar text strings, offering better comparison results.

- [Teachable Machine](https://teachablemachine.withgoogle.com/) is used for training machine learning model to integrate skin type classification.

- [JWT](https://jwt.io/) is utilized for authentication and session management.

<br><br>
<!-- UI UX -->
<img src="./readme/title4.svg"/>

###

> Skinly is designed using wireframes and mockups, iterating on the design until we reached the ideal layout for easy navigation and a seamless user experience.

- Project Figma design [figma](https://www.figma.com/design/QMLETGiujnRpv5Vc193IZc/UI-UX-Assignments?node-id=117-417&p=f&t=hetwMb0YXQQht2Jd-0)


### Mockups
| Welcome screen  | Onboarding Screen | Home Screen |
| ---| ---| ---|
| ![Landing](./readme/mockup1.png) | ![fsdaf](./readme/mockup2.png) | ![fsdaf](./readme/mockup3.png) |

<br><br>

<!-- Database Design -->

<img src="./readme/title5.svg"/>

###  Database Schema Design:

<!-- - Insert ER Diagram here -->
| User Schema  | Company Schema | AiRequests Schema |
| ---| ---| ---|
| ![Landing](./readme/user-snapshot1.png) | ![fsdaf](./readme/company-snapshot1.png)| ![fsdaf](./readme/ai-snapshot1.png) |


<br><br>


<!-- Implementation -->
<img src="./readme/title6.svg"/>


### User Screens (Mobile)
| Login screen  | OnBoarding screen | OnBoarding screen |
| ---| ---| ---|
| ![Landing](./readme/app/welcom-screen.jpeg) | ![fsdaf](./readme/app//onboarding1.jpeg) | ![fsdaf](./readme/app/onboarding2.jpeg) |
| OnBoarding screen  | Login Screen | Register Screen |
| ![Landing](./readme/app/onboarding3.jpeg) | ![fsdaf](./readme/app/login.jpeg) | ![fsdaf](./readme/app/register.jpeg) |
| Forgot Password Screen  | Verification Code Screen | Reset Password Screen |
| ![Landing](./readme/app/forget=password.jpeg) | ![fsdaf](./readme/app/verify.jpeg) | ![fsdaf](./readme/app/reseet.jpeg) |
| Home screen  | Product Comparison Screen | Ingredients Scan Screen |
| ![Landing](./readme/app/home.gif) | ![fsdaf](./readme/app/product.gif) | ![fsdaf](./readme/app/openai.gif) |
| Skin Type Detection Screen  | Recommendations Screen | Profile Screen |
| ![Landing](./readme/app/skin-detection-1.gif) | ![fsdaf](./readme/app/recommendations.jpeg) | ![fsdaf](./readme/app/profile.gif) |


### Company Screens
| Login Screen  | Home Screen |  Advertisement Creation Screen |
| ---| ---| ---|
| ![Landing](./readme/app/company-login.jpeg) | ![fsdaf](./readme/app/company-home.jpeg) | ![fsdaf](./readme/app/advertisment.jpeg) |

### Admin Screens (Web)
| Login Screen  | User Management Screen |
| ---| ---|
| ![Landing](./readme/app/admin-login.png) | ![fsdaf](./readme/app/admin-users.png) |
| Company Management Screen  | Add New Company Screen |
| ![Landing](./readme/app/admin-companies.png) | ![fsdaf](./readme/app/admin-addCompany.png) |
<br><br>


<!-- Prompt Engineering -->
<img src="./readme/title7.svg"/>

###
<!-- ###  Mastering Interaction: Unveiling the Power of Prompt Engineering: -->

This project uses OpenAI to optimize tasks like ingredient compatibility checks and personalized recommendations, highlighting the transformative power of AI-driven solutions.<br>
 The goal is to use AI-driven solutions to enhance user experiences.

To check ingredients, the app first processes the uploaded image by EasyOCR. The OCR extracts ingredient names, or product information converting it into text. Once the ingredients are extracted, the data is sent to OpenAI. OpenAI analyzes the data and checks the compatibility of ingredients.

To get personalized recommendations, the app processes the images using a pre-trained model (haarcascade_frontalface_default.xml) using OpenCV to detect number of faces within the image. If the count of faces detected is different than 1 the app will ask the user to retry. If one face detected the image wil be processed by skin type prediction model.Then this data is sent to OpenAI that generates personalized recommendations.


<img src="./readme/app/prompt.png"/>

<br><br>
<!-- < AWS Deployment> -->
 <img src="./readme/title8.svg"/>

###
<!-- ###  Efficient Deployment: Unleashing the Potential with AWS Integration: -->
This project uses AWS for seamless deployment of the backend server EC2 instance, ensuring scalability, reliability, and performance.<br>
API endpoints are tested using Postman


| Get Users  | Get Companies |
| ---| ---|
| ![Landing](./readme/app/getUsers1.png) | ![fsdaf](./readme/app/getCompanies1.png) |
| Get Similar Product  | Products Pagination |
| ![Landing](./readme/app/getSimilar1.png) | ![fsdaf](./readme/app/productPagination1.png) |


<br><br>

<img src="./readme/title10.svg"/>

###

> To set up Skinly app locally, follow these steps:

### Prerequisites

Ensure you have the following installed:

* Install Node.js and npm (Node Package Manager):
  ```sh
  npm install npm@latest -g
  ```
* Install Python (version 3.10 recommended)


#### Cloning the Repository

Run the following command to clone the repository and all its submodules

   ```sh
   git clone --recurse-submodules [github](https://github.com/LyneSultan/Skinly.git)
   ```

#### Server Configuration

1. Navigate to skinly-server directory

   ```sh
   cd nest-server
   ```

2. Install NPM packages
   ```sh
   npm install
   ```
3.  Get an OpenAI API Key

4. Run the following command and update the created .env file
   ```sh
   cp .env.example .env
   ```
5. Run Nestjs
   ```sh
   npm run start
   ```

#### App Configuration

1. Navigate to mobile-app directory

   ```sh
   cd mobile-app
   ```

2. Install NPM packages
   ```sh
   npm install
   ```
3. Run Nestjs
   ```sh
   npm run start
   ```
4. Test on a Device or Emulator:

* Physical Device: Install the Expo Go app from the App Store or Google Play. Use the QR code from the development server to open the app on your device.
* Emulator: Ensure your emulator (Android or iOS) is running, then select the appropriate option in the Expo development server interface.

#### Django Configuration

1. Navigate to django-server directory

   ```sh
   cd django-server
   ```

2. Create and Activate a Virtual Environment
   ```sh
   python -m venv venv
   venv\Scripts\activate
   ```
3. Install Dependencies
   ```sh
   pip install -r requirements.txt
   ```
4. Run the Server
   ```sh
   python manage.py runserver
   ```

#### Admin App Configuration

1. Navigate to admin-panel directory
   ```sh
   cd admin-panel
   ```

2. Install NPM packages
   ```sh
   npm install
   ```
3. Run the following command and update the created .env file
   ```sh
   cp .env.example .env
   ```
4. Run project
   ```sh
   npm run start
   ```
