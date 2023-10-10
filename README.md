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
- Adrian Sandu (QA engineer)

#### 1.1.2 Entry criteria defined
- Initial project risks were detected and mitigated
- The requirement document should be available.
- Complete understanding of the application flow is required.
  
#### 1.1.3 Exit criteria defined
All high-priority defects are fixed and retested
- Test coverage meets the predefined criteria
- All the test have been executed
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
  - Lack of experience of the QA engineer
  - Resource constraints: Short deadline of Zephyr Squad trial, unavailability of test environment.
  - Schedule delays: Bottlenecks or delays in testing phases.
  
* Product risks:
  - Compatibility issues with certain browsers: Internet Explorer, Opera browser
  - Layout issues: Website is not displayed properly with some browser resolutions

#### 1.1.6 Evaluating entry criteria

The entry criteria defined in the Test Planning phase have been achieved, and the test process can continue.

## 1.2 Test Monitoring and Control

Test monitoring and control will be done by generating periodic reports that reflect the current status of the tests.

<img src="https://raw.githubusercontent.com/AdrianSandu92/Manual-Testing-Project/main/files/testexecutions.png" />

## 1.3 Test Analysis

The testing process will be executed based on the above requirements for the Dependents module. The following test conditions were found:
 *  Verify user registration process:
- Ensure that the registration form is accessible and loads correctly.
- Test all mandatory fields (e.g., name, email, password) for validation, ensuring they are required and correctly validated (e.g., email format, password strength).
- Verify that the registration form submission successfully creates a new user account.
- Verify if the system is sending registration link to the user.
- Verify if the link is working properly and the system register the user into the database.

 * Validate login functionality:
- Confirm that the login page is accessible and loads without errors.
- Verify that registered users can log in successfully using their valid credentials.
- Test login with invalid credentials to ensure appropriate error messages are displayed.
- Check for security measures like account lockout after a certain number of failed login attempts.

* Test user profile section:
 - Ensure that users can access and edit their profiles after logging in.
- Validate that changes made to the user's profile (e.g., name, email, profile picture) are saved correctly.
- Verify that profile updates are reflected and displayed accurately in the user dashboard and elsewhere in the application.

* Verify password reset functionality:
 - Test the "Forgot Password" or "Reset Password" functionality.
 - Verify that users receive password reset emails with valid reset links.
 - Confirm that users can reset their passwords successfully by following the reset link.
 - Ensure that the old password is invalidated upon resetting.


## 1.4 Test Design

Functional test cases were created in Zephyr Squad. Based on the analysis of the specifications, the test design techniques used for generating test cases 
are: Use case testing, boundry-value analysis, negative testing.


**Test cases:**
<img src="https://raw.githubusercontent.com/AdrianSandu92/Manual-Testing-Project/main/files/testcases.png"/>

All the test cases exported into a xlsx can be downloaded from this link: [example](https://github.com/AdrianSandu92/Manual-Testing-Project/raw/main/files/testcases.xlsx)

## 1.5 Test Implementation

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

