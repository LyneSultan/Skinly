<img src="./readme/title1.svg"/>

<br><br>

<!-- project philosophy -->
<img src="./readme/title2.svg"/>

###

> Skinly is an app that provides users with a personalized skincare experience by detecting skin type, analyzing the compatibility of ingredients with skin types, and searching for products across multiple platforms.


### User Stories
#### User

- As a user, I want to upload an image of my face, so I can detect my skin type.

- As a user, I want to scan product ingredients using OCR, so I can see if they are suitable for my skin type.

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

  - [Django](https://www.djangoproject.com/) is utilized for specific functionalities, including OCR and detecting the user’s skin type using a trained model.

- The app uses [ React Native Paper](https://reactnativepaper.com/) for the design and front-end components, providing a modern, responsive, and accessible user interface based on Material Design principles.
<!--
- The app uses the font ["Poppins"](https://fonts.google.com/specimen/Poppins) as its main font, offering a clean and modern design aesthetic that aligns with the material design guidelines.
 -->

<br><br>
<!-- UI UX -->
<img src="./readme/title4.svg"/>

###

> We designed Skinly using wireframes and mockups, iterating on the design until we reached the ideal layout for easy navigation and a seamless user experience.

- Project Figma design [figma](https://www.figma.com/design/QMLETGiujnRpv5Vc193IZc/UI-UX-Assignments?node-id=117-417&p=f&t=hetwMb0YXQQht2Jd-0)


### Mockups
| Home screen  | Menu Screen | Order Screen |
| ---| ---| ---|
| ![Landing](./readme/mockup1.png) | ![fsdaf](./readme/mockup2.png) | ![fsdaf](./readme/mockup3.png) |

<br><br>

<!-- Database Design -->

<img src="./readme/title5.svg"/>

###  Architecting Data Excellence: Innovative Database Design Strategies:

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
| Company Management Screen  |  Add New Company Screen |
| ![Landing](./readme/app/admin-companies.png) | ![fsdaf](./readme/app/admin-addCompany.png) |
<br><br>


<!-- Prompt Engineering -->
<img src="./readme/title7.svg"/>

###  Mastering Interaction: Unveiling the Power of Prompt Engineering:

This project leverages OpenAI to create intelligent interactions through precise prompts.<br>
 It focuses on optimizing tasks like ingredient compatibility checks and personalized recommendations, highlighting the transformative power of AI-driven solutions.<br>
 The goal is to showcase the power of AI-driven solutions for enhanced user experiences.

<br><br>

<!-- AWS Deployment -->
<!-- <img src="./readme/title8.svg"/>

###  Efficient Deployment: Unleashing the Potential with AWS Integration: -->



<!-- <br><br> -->

<!-- Unit Testing -->

<!-- How to run -->
<img src="./readme/title10.svg"/>

> To set up Skinly app locally, follow these steps:

### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* npm
  ```sh
  npm install npm@latest -g
  ```

### Installation

_Below is an example of how you can instruct your audience on installing and setting up your app. This template doesn't rely on any external dependencies or services._

1. Get an OpenAI API Key
2. Clone the repo
   git clone [github](https://github.com/LyneSultan/Skinly.git)
3. Install NPM packages
   ```sh
   npm install
   ```
4. Create a .env file in the root of the server project and add your environment variables and enter your API in
   ```js
   OPEN_AI_KEY = 'ENTER YOUR API';
   ```

Now, you should be able to run Skinly app locally and explore its features.
