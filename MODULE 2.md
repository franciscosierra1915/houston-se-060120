# Module 2

### Learning Goals

- Sinatra & MVC
  - Define the following tools
    - Rack
    - Shotgun
    - Sinatra
    - Rails
  - Explain the responsibilities of the following application components:
    - Model
    - View
    - Controller
- HTML & CSS
  - Identify the common components of HTML elements
  - Identify Common HTML and CSS Elements
  - Use EJS to interpolate Ruby variables into HTML pages
- Forms
  - Identify HTML elements and attributes common to forms
  - Describe how to send data from the browser to the server with a Form
  - Build a form which creates a nested hash through input name
- Web Applications
  - Focus on the methodology of using tools to build an app
- Web Associations
  - Use foreign keys to create references between Table Rows
  - Use user input to define foreign keys
  - Use other types of inputs to improve the user's experience when creating associations
- Rails
  - Create a Rails app
  - Create & Run Migrations with Rails
  - Create Controllers and route requests to those controllers using rails
  - Use the methods of strong params to filter user input
- Route Helpers
  - Use `resources` to automate the routing process
  - Use `link_to` to automate `a` tags
- Form Helpers
  - Use rails helpers to create a form
  - Use `form_with` to create a form for a resource
  - Use `collection_select` and `collection_check_boxes` to create inputs for associations
- Sessions & Cookies
  - Define statelessness in the context of programming
  - Explain what it means for HTTP to be stateless 
  - Explain the roles that sessions and cookies play in solving the challenges posed by statelessness
- Rails Validations
  - Explain the advantage of fat models and skinny controllers
  - Use ActiveRecord validation helpers to validate data
  - Check for resource validity in the controller
  - Display error messages in the view
- Authentication
  - Define Authentication, Authorization, Hashing, Encryption, and BCrypt
  - Add a secured password to a user model using `bcrypt` and `password_digest`
  - Implement a sign in form
  - Implement authorization to protect a route in an application

### Code Challenge Rubric


#### Models, Associations, and Validations

1. Models, associations, and validation not started or have errors that prevent the application from running. Missing validations, or validation syntax is incorrect. May have introduced models outside the specified domain.

2. Models, associations, and validations attempted but incomplete or have errors. Associations may construct the wrong relationships. Validations may be missing or applied to the wrong models. Advanced query methods incomplete or have errors.

3. Models, associations, and validations mostly complete and correct per the deliverables. Advanced validations and methods may be incomplete. May have unused or unnecessary code, possibly including duplication. May have written validations instead of using appropriate built-in validations. May implement advanced query methods with iterators instead of using built-in methods.

4. All models, associations, and validations are complete and correct, save minor mistakes in advanced deliverables. Advanced validations are complete and add informative error messages.

5. All specified models, associations, and validations are complete and correct. Built-in validations are used when appropriate. Variable and method names are intention-revealing. Models have appropriate logic extracted from controllers and views. Advanced query methods use appropriate built-in methods.

#### Routes, Controllers, and REST

1. Routes missing, naming does not follow REST, controller actions incomplete or with errors.

2. Some routing and controller logic implemented, but incompletely or incorrectly. May have routes or controller actions not included in the deliverables. May include routes that have no corresponding controller action or vice versa. Controller methods might do work beyond their responsibility in MVC.

3. Most routing and controller logic working as specified. Some advanced deliverables may be incomplete. Routing follows REST convention. Routing table might include some unused routes, or routes and actions that were not specified in the deliverables. Logic may be duplicated between methods.

4. Nearly all routing and controller deliverables completed, possibly with minor errors in advanced deliverables. Routing follows REST conventions. Some logic may be duplicated between controller actions, or not respect MVC separation of concerns. Attempts to use filters and private helper methods to reduce duplication, but some duplication may remain.

5. All routes and controllers deliverables work as described in the instructions. Routing follows REST naming conventions. Controller actions respect MVC separation of concerns, and don't have logic that belongs in the model or the view. ActionController filters and private helper methods are used appropriately to reduce duplication in controller actions.

#### Views and Forms

1. Missing or unattempted views and forms, or erb syntax errors in views and forms. Forms created in the wrong views, do not accept the correct input, or do not submit to the correct location. Data not displayed correctly.

2. Views display some data correctly. Forms attempted, but with some errors that prevent submitting data correctly. May not have attempted or may have significant errors in advanced deliverables.

3. Uses view to show data as specified. At least one working form that submits data to the correct location. May not have attempted some advanced view features. May have included views not specified by the deliverables. May include model or controller logic in the view. Forms may accept invalid input (for example, out of range numbers). May not display validation errors correctly. May not use view helper methods to reduce duplication.

4. Nearly all view and form deliverables are complete and correct. May have minor logic errors in advanced deliverables. Mostly does not include controller or model logic in the views. Mostly uses helpers to reduce duplication.

5. All view and form deliverables are complete and correct, including advanced form components. No views not specified by the instructions. No model or controller logic present in the views. Appropriate use of helpers and built-ins to reduce duplication. Validation errors displayed correctly on form.