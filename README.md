# Angular Notes

- ng new [NEW_MODULE_NAME]
- ng serve
- ng g component [NEW_COMPONENT]
- ng g class [NEW_MODEL_NAME]

=============

## Angular Learing
- Application setup
- Directory setup
- Bootstraping process
- Components
	- Components are the individual and free piece of logic and view
- Data Binding
	- To connecting your DOM elements with components
	- Types
		- Property binding: 
			1. String interpolation {{ }}
			2. Square bracket around attribute e.g. < input type="text" [value]= "propertyName">
			3. Using "bind-" prefix e.g. < input type="text" bind-value= "propertyName">
		- Style binding (CSS)
			1. [style.property] = "value"
			2. [ngStyle] = "{'property1': 'value', 'property2': 'value'}"
		- Class binding (CSS)
			1. [class.property] = "value"
			2. [ngClass] = "{'property1': 'value', 'property2': 'value'}"
		- Event binding:
		- Two way binding:
	- Custom property:
		- User @Input property in class
- Directives
	- Directives are used to extend HTML elements and attributes in Angular application
	- Directive also guide compiler to render specific view or behavior for certain HTML element or attribute
	- Types of directives
		1. Attribute directive
			- change the apperance or behavior of an element, component or another directive
			- e.g. _ngClass_, _ngStyle_
		2. Structural directive
			- change the DOM layout by adding or removing DOM elements
			- e.g. _*ngIf_, _*ngFor_, _*ngSwitch_
		3. Component directive
			- Directives with templates
			- e.g. <_app-root_>
	- Role of Asterisk ( * ) symbol
		- It's a syntactic sugar mechanism.
		- behind the scene, instruct the angular to enclose the parent element by < template > element and then apply the directive behavior on the child elements of < template >
		- After behavior implementation, remove the < template > element from view
		- ![](images/structural-element-parsing.png?raw=true)

=============

### Concepts
- bootstraping 
	- In angular means app automatically start with ngApp directive or < app-root> in angular 7.
	- Bootstrapping in web frameworks is pushed into index page (the bootstrapper), and then it loads the frameworks helpers, models, configuration, and then loads the controller and passes off control to it.
- string interpolation -< {{ string }}
- 