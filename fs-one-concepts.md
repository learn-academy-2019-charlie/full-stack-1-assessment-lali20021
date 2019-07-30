# Full Stack 1 Assessment

Try your best to answer each question on your own before looking up the answer online. Once you're done writing your first answer, you can google the question and write the best answer you find.

#### 1. What is Enzyme and what are some of the methods that it provides?
Enzyme is testing utility package developed by Airbnb that makes testing React component easier. Enzyme provides more streamlined methods to carry out tests.
shallow() - will test the provided component and ignore any child components that may be present in the component tree thereafter.
shallow() is designed to only test one function.

mount():
- Full DOM rendering including child components.
- Ideal for use cases where you have components that may interact with DOM API, or use React lifecycle methods in order to fully test the component.
- As it actually mounts the component in the DOM .unmount() should be called after each tests to stop tests affecting each other.
- Allows access to both props directly passed into the root component (including default props) and props passed into child components.

shallow():
- Renders only the single component, not including its children. This is useful to isolate the component for pure unit testing. It protects against changes or bugs in a child component altering the behavior or output of the component under test.
- As of Enzyme 3 shallow components do have access to lifecycle methods by default.
- Cannot access props passed into the root component (therefore also not default props), but can those passed into child components, and can test the effect of props passed into the root component. This is as with shallow(<MyComponent />), you're testing what MyComponent renders - not the element you passed into shallow.

render():
- Renders to static HTML, including children.
- Does not have access to React lifecycle methods.
- Less costly than mount but provides less functionality.

#### 2. What is the difference between dynamic and a static routes?
In the Static routing, the table is set up and modified manually whereas in the Dynamic routing the table is built automatically with the help of the routing protocols.

#### 3. What is a JSON API?
JSON or JavaScript Object Notation is an encoding scheme that is designed to eliminate the need for an ad-hoc code for each application to communicate with servers that communicate in a defined way. JSON API module exposes an implementation for data stores and data structures, such as entity types, bundles, and fields.

#### 4. What is a migration and why would you use one?
Migration allows you to define changes to your database schema, making it possible to use a version control system to keep things synchronized with the actual code.
Migrations can create table, drop table, rename table, add column, rename column, change column, remove column.

#### 5. Explain how to set up a route in React.

#### 6. When would you use a generate resource over a generate controller?
Rails g controller only generates a controller. I would use resource if I need to generate a model, a controller and a migration.

#### 7. Explain the difference between a controller spec and a request spec.

#### 8. Describe the React component lifecycle. What are some of the lifecycle methods?

#### 9. At this point in the program, what technologies/languages do you find yourself gravitating to?
Ruby and Ruby on Rails