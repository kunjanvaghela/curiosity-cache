
[[API Testing]]
[[Automation Testing]]



## Testing Pyramid
<img src="https://www.onpathtesting.com/hs-fs/hubfs/agile%20testing%20pyramid%20onpath%20testing%20QA.png?width=7781&name=agile%20testing%20pyramid%20onpath%20testing%20QA.png">



## 1. Fundamentals

Defect vs Bug vs Mistake


### Testing Principles:
1) Testing shows presence of defects
2) Exhaustive testing is impossible
3) Early testing
4) Defect clustering
5) Pesticide Paradox
6) Testing is context dependent
7) Absense-of-errors fallacy


### Fundamental Test process

Few terms: **confirmation testing, exit criteria, incident, regression testing, test basis, test condition, test coverage, test data, test execution, test log, test plan, test strategy, test summary report and testware**

1. Test Planning and Control
	1. Determine risks
	2. Determine test approach
	3. Determine resources
	4. Determine exit criteria
2. Test Analysis and design
	1. Test basis
	2. Test Analysis: What to test?
	3. Test Design: How to test?
3. Test Implementation and Execution
4. Evaluating Exit Criteria and Reporting
5. Test Closure Activities




## 2. Testing throughout the Life Cycle

SDLCs:
1. Waterfall Model --> V-Model
		
	<img src="https://static.javatpoint.com/tutorial/software-engineering/images/software-engineering-v-model.png">
	
2. Iterative Life Cycles --> Agile



### Test Levels
1. Component Testing
	1. Stubs - From the component under test
	2. Driver - Calls the unit under test
2. Integration Testing
	1. Top-down: From GUI/main menu --> Components/systems are substituted by stubs.
	2. Bottom-up: From the bottom of the control flow --> Components/systems are substituted by drivers.
	3. Functional incremental --> on the basis of the functions or functionality, as per functional specification.
3. System Testing
4. Acceptance Testing


Test Driver Development
<img src="https://images.spiceworks.com/wp-content/uploads/2022/09/29095630/How-TDD-Works.png">


### Test Types
1. Functional Testing
	1. Black-box testing
	2. Specification-based
2. Non-Functional Testing
	1. Performance
	2. Load
	3. Stress
	4. Usability
	5. Maintainability
	6. Reliability
	7. Portability
3. Structural Testing
	1. White-box/Glass-box
	2. Code coverage
4. Confirmation and Regression Testing
5. Maintenance Testing
	1. Checks maintainability of a software in production.
	2. Triggers:
		1. Planned modifications
		2. Ad-hoc corrective modifications
	3. Impact Analysis and Regression testing are crucial





## 3. Static Techniques

#### Review Process:

Formal Review Process
1. Planning
2. Kick-off
3. Preparation
4. Review meeting
5. Rework
6. Follow-up

Roles and responsibilities
1. The moderator - Lead, type of review, perform checks, entry checks, follow ups
2. The author - To improve quality
3. The scribe - Records and suggestions
4. The reviewers - Checks material for bugs
5. The manager - Allocates time and resources

Types of Review (in the order of formality):
1. Informal
2. Walkthrough
3. Technical Review
4. Inspection

Review by:
1. Ad hoc
2. Checklist based
3. Scenarios and Dry Runs
4. Perspective-based
5. Role-based

Static Analysis by Tools
1. Coding Standards
	1. Using Linters
2. Code Metrics
3. Code Structure
	1. Control Flow Structure
	2. Data Flow Structure
	3. Data Structure






## 4. Test Design Techniques

Test Analysis - process of looking for something to test using a set of inputs and outputs
Test Case - A set of preconditions, inputs, expected results and postconditions, developed based on test condition.
Test Condition - An item/event of a component or system that could be verified by one or more test cases.
Test Oracle - 

#### Static Testing Techniques:
Covered in 3. chapter:
1. Informal Reviews
2. Walkthroughs
3. Technical Reviews
4. Inspection
5. Static Analysis: Data Flow & Control Flow

#### Dynamic Testing Techniques
1. Structure-based (White-Box Testing):
	1. Statement
	2. Decision
	3. Condition
	4. Multiple Condition
2. Experience Based
	1. Error Guessing - based on testers knowledge working with similar functionalities, for ex:
		- errors encountered in past
		- what kind of errors that tend to come up
		- failures encountered in another parts
	1. Exploratory Testing
3. Specification-based (Black-Box Testing mainly)
	1. Equivalence Partitioning
		- can be applied to any test level
		- Process:
			- Divide data into partitions, with all members of a given partition are expected to be processed in same way.
			- Partitions can divided to sub-partitions if required.
			- Test case must process with minimum of 1 value per partition with hypothesis that if 1 value of the partition works, then all others will also work.
	2. Boundary Value Analysis
	3. Decision Tables
		- Cause-Effect table
		- Process:
			- Identify conditions and resulting actions.
			- Inputs at top, actions at bottom
	4. State Transition
	5. Use Case Testing



## 5. Test Management

Roles:
- Test Manager
	- assembles & leads teams
	- defines scopes
	- distributes resources
	- makes sure that the process runs smoothly & achieves results
- Tester
	- designs &
	- executes tests

Documentation Standards
- Master Plan
- Plans for test levels
- Plans for functional tests
- Plans for non-functional tests

Test Approaches/Strategies
1. Analytical: Risk-based
2. Model-based
3. Methodical
4. Process- or standard-compliant
5. Directed or Consultative
6. Regression-averse


Define:
	- Entry Criteria
	- Exit Criteria
	- Find Test Dependencies
	- Estimate sufficient time for Confirmation & Regression testing


Test Estimate Techniques:
1. Metric-based
2. Expert based


Test Control Estimation
- Percentage of planned work done
- Test Case Execution
- Defect Information
- Test Coverage
- Task Completion, Resources Allocation & Usage
- Cost of Testing


Risks:
1. Product Risks - Product fails to satisfy legitimate needs of its stakeholders.
2. Project Risks


Focus on Incident Reporting, Traceability to make sure that defects do not regress





## 6. Tool support for Testing

Types of Test Tool:
1. Test Management Tools
	- Like Jira, HPALM, Zephyr, TestRail, Test Collab, XQual, qTest, Qase, etc.
2. Test Design and Implementation Tool
	- On input of test field format, gives output like acceptable & Rejected cases
	- Ex. Shsha testing tool.
3. Test Execution & Logging Tools
4. Static Testing Tools
	- Like IDEs
5. Performance Measurement & Dynamic Analysis Tools
	- Ex. Apache JMeter, LoadInjector, LoadRunner, etc
6. Specialized Testing Tools


Test Execution Tools:
1. Capture Test Approach - can capture UI steps by a user, but needs to be done again and again
2. Data-Driven Test Approach - actions remain same, but input data is different.
3. Keywork-Driven Test Approach - Sailfish Testing Tools.


Tool Selection:
1. Looking for Bottlenecks in the current Organization
2. Compatibility of existing tools with the new tool
3. Evaluate the tool against clear requirements and objective criteria
4. Review Vendor for:
	1. Reliability
	2. Training & Support
	3. Robust services
5. Proof of Concept
	1. Also settle on naming conventions, selecting coding standards, creating libraries, understanding the metrics for the new tool