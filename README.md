# Final project for ITF Manual Testing Course

The scope of the final project for ITF Manual Testing Course is to use all gained knowledge throught the course and apply them in practice, using a live application. 

Application under test: <a href="https://autokarma.ro" target="_blank">Autokarma.ro website</a>

Tools used: JIRA, Zephyr Squad

# Functional specifications

www.autokarma.ro is a website designed to provide information and services related to automotive repair and maintenance. The website aims to cater to both vehicle owners and automotive professionals by offering a user-friendly interface and a range of useful features.

### Functional Requirements:

__- User Registration and Authentication:__ Users can create accounts with a username and password. Users can log in and log out securely.

__- User Profile Management:__ Users can update their profile information. Users can reset their password if they forget it.

__- Search Functionality:__
Users can search for automotive products, services, and articles using keywords.
Advanced search options, such as filters by category, brand, and price, are available.

__- Product Listings:__
The website displays a list of automotive products with details, including price, availability, and product descriptions.
Users can click on a product to view more information.

__- Service Listings:__
The website displays a list of automotive services offered by registered service providers.
Users can click on a service to view more information.

__- Booking and Appointments:__
Users can book automotive services from service providers.
Users can select their preferred date and time for the service.
Users receive confirmation emails for their bookings.

__- Blog and Articles:__
The website features a blog section with articles related to automotive tips, news, and guides.
Users can comment on articles and share them on social media.

__- User Reviews and Ratings:__
Users can leave reviews and ratings for products and services they have used.
Reviews are displayed along with product or service listings.

__- Shopping Cart and Checkout:__
Users can add products to their shopping cart.
Users can proceed to checkout, enter shipping details, and make payments securely.

__- Contact and Support:__
Users can contact the website administrators or support team through a contact form.
Frequently Asked Questions (FAQs) are available.

__- User Notifications:__
Users receive email notifications for account activities (e.g., registration, password reset) and booking confirmations.
Users receive notifications for new articles and updates.

# 1 Testing section

## 1.1 Test Planning

The Test Plan is designed to describe all details of testing for the __Users area__ from the Autokarma.ro website

The plan identifies the items to be tested, the features to be tested, the types of testing to be performed and the risks associated with the plan

#### 1.1.1 Roles assigned to the project and persons allocated
- Adrian Sandu (ITF coursant)

#### 1.1.2 Entry criteria defined
- Availability of the test environment
- Test data prepared and available

#### 1.1.3 Exit criteria defined
All high-priority defects are fixed and retested
- Test coverage meets the predefined criteria
- Acceptance criteria are met
- The product is stable and meets performance criteria
  
#### 1.1.4 Test scope
* __Tests in scope:__
  - User registration
  - Login functionality
  - User profile management
  - Password reset
  - User dashboard
  - User account settings

* __Tests not in scope:__
  - Payment processing
  - Admin area
  - Performance testing
  - Stress testing
  - Regression testing


#### 1.1.5 Risks detected

* Project risks:
  - Resource constraints
  - Schedule delays
  - Communication gaps with providers
  - The risk of not having enough employees
  - Problems with courier companies
  
* Product risks:
  - Servers malfunction
  - Database errors
  - Security risks
  - Compatibility issues with certain browsers
  - Functional defects

#### 1.1.6 Evaluating entry criteria

The entry criteria defined in the Test Planning phase have been achieved, and the test process can continue.

## 1.2 Test Monitoring and Control

Test monitoring and control will be done by generating periodic reports that reflect the current status of the test.

## 1.3 Test Analysis

The testing process will be executed based on the above requirements for the Dependents module. The following test conditions were found:
 *  Verify user registration process
 - Validate login functionality
 - Test user profile update
 - Verify password reset functionality
 - Validate user dashboard features
 - Test user account settings

## 1.4 Test Design

Functional test cases were created in Zephyr Squad. Based on the analysis of the specifications, the test design techniques used for generating test cases 
are:
1. User Registration Test Case
2. Login Functionality Test Case
3. User Profile Update Test Case
4. Password Reset Test Case
5. User Dashboard Test Case
6. User Account Settings Test Case

**Test cases:**
- AS-35 Verify if the user is able to create a new account
- AS-9 Verify if the user can login into his account
- AS-22 Verify if the user can access his already created account
- AS-15 Verify the "Forgot password" function
- AS-20 Verify if the user can add products to cart
- AS-28 Verify if an user can add products to wishlist
- AS-25 Verify if the user is able to add his own car model into his account dashboard.
- AS-18 Verify if the user can search by chasis code (VIN)
- AS-19 Verify if the user can search products by universal name or product code
- AS-21 Verify if the user can find parts for a specific car
- AS-33 Verify the GUI elements from the website
Example of test case with examples can be found here: [AS-2.pdf](https://github.com/AdrianSanduroiect-practic-testare-manuala/blob/main/AS-2.pdf)

## 1.5 Test Implementation

The following elements are needed to be ready before the test execution phase begins:

* The following elements need to be ready before the test execution phase begins:
- Test environment setup
- Test data availability
- Test scripts and automation tools configured (JIRA, Zephyr Squad)

## 1.6 Test Execution
* Test cases are executed on the created test cycle. A summary of the test executions can be found in the document:
  [Jira.doc]()


* Bugs have been created based on the failed tests. Bug titles:

  - Problems displaying header at different resolutions (Responsiveness bug)
  - The website no longer displays error details after generating verification code
  - The quantity field accept letters and special characters
  - Email validation rules don't work
  - Forgot password function is actually generate new password
  - Users can create accounts with less than 8 characters on password field
 The complete bug reports can be found here: [Bugs.pdf](https://github.com/AdrianSandu92/Proiect-practic-testare-manuala/blob/main/Bugs.pdf)


## 1.7 Test Completion

* Exit criteria was evaluated and passed
* The traceability matrix was generated and can be found here: [matrix.png](https://github.com/AdrianSandu92/Proiect-practic-testare-manuala/blob/main/matrix.png)
* Test execution chart was generated and can be found here: [testex.png](https://github.com/AdrianSandu92/Proiect-practic-testare-manuala/blob/main/testex.png)
* The final report shows that 14 tests were valid and 1 was failed.

