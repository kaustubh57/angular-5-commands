# Angular Notes

- ng new [NEW_MODULE_NAME]
- ng serve
- ng g component [NEW_COMPONENT]
- ng g service [NEW_SERVICE]
- ng g class [NEW_MODEL_NAME]

=============

## Angular Learing
- **Application setup**
- **Directory setup**
- **Bootstraping process**

- **Components**
	- Components are the individual and free piece of logic and view
	- Use _@Component_ directive

- **Data Binding**
	- To connecting your DOM elements with components
	- Types
		- <span style="color:blue">Property binding: </span>
			1. String interpolation {{ }}
			2. Square bracket around attribute e.g. < input type="text" [value]= "propertyName">
			3. Using "bind-" prefix e.g. < input type="text" bind-value= "propertyName">
		- <span style="color:blue">Style binding (CSS)</span>
			1. [style.property] = "value"
			2. [ngStyle] = "{'property1': 'value', 'property2': 'value'}"
		- <span style="color:blue">Class binding (CSS)</span>
			1. [class.property] = "value"
			2. [ngClass] = "{'property1': 'value', 'property2': 'value'}"
		- Event binding:
		- Two way binding:
	- Custom property:
		- User @Input property in class

- **Directives**
	- Directives are used to extend HTML elements and attributes in Angular application
	- Directive also guide compiler to render specific view or behavior for certain HTML element or attribute
	- <span style="color:blue">Types of directives</span>
		1. Attribute directive
			- change the apperance or behavior of an element, component or another directive
			- e.g. _ngClass_, _ngStyle_
		2. Structural directive
			- change the DOM layout by adding or removing DOM elements
			- e.g. _*ngIf_, _*ngFor_, _*ngSwitch_
		3. Component directive
			- Directives with templates
			- e.g. <_app-root_>
	- <span style="color:blue">Role of Asterisk ( * ) symbol</span>
		- It's a syntactic sugar mechanism.
		- behind the scene, instruct the angular to enclose the parent element by < template > element and then apply the directive behavior on the child elements of < template >
		- After behavior implementation, remove the < template > element from view
		- ![](images/structural-element-parsing.png?raw=true)
	- <span style="color:blue">Custom Attribute directive</span>
		- Use _@Directive_ decorator

- **Services**
	- Services type script classes which can have specific functionality and that functionality can be performed in the component, directive or any other part of the applicaiton where we import and inject them.
	- Service can be injected using dependency injection.
	- Bind that in a component's _providers_ array and use it.

- **Angular Forms**
	- Types
		1. Template Driven Forms
			- Based on HTML DOM and Angular Directives
			- Use to create Simple Forms
			- Limit Controls over Form Elements
			- Normal Validations
		2. Reactive Forms
			- Use to create Complex Forms
			- Based on Class Body Programming
			- Full Control on Form Elements
			- Sync with HTML form
			- Need to import _ReactiveFormsModule_ in the module where it will be used (or AppModule)
			- Custom validations can be applied
	- Form Control Objects
		![](images/form-control-objects.png?raw=true)
	- **Form Array** to store multiple valus of an array
	- Template variable or local reference can be assigned using "#" symbol

- **Http Services**
	- Observables
		![](images/observables-life-cycle.png?raw=true)
	- Map operator

- Routers: Navigate to Application
	- Pass and extract multiple route parameters
	- Send and extract query parameter
		![](images/extract-route-param-and-query-param.png?raw=true =100px)

- Upgrade Angular app

=============

### Concepts
- bootstraping 
	- In angular means app automatically start with ngApp directive or < app-root> in angular 7.
	- Bootstrapping in web frameworks is pushed into index page (the bootstrapper), and then it loads the frameworks helpers, models, configuration, and then loads the controller and passes off control to it.
- string interpolation - {{ string }}
- Form Control: Individual form element
- Form Group: Group of form elements