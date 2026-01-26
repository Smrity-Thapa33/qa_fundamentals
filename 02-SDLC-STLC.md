# Software Development Life Cycle (SDLC)
SDLC is a structured framework that defines the software development process from beginning to end i.e. from initial idea to final deployment and maintenance. The goal of SDLC is to develop a high-quality software that meets the customers’ requirements or satisfaction and to reach the completion within a dedicated time and cost.
## Stages of SDLC:
1.	**Planning and Requirements Analysis:** It is the most fundamental stage where team gathers business and functional requirements from stakeholders.
- **Goal:** To understand users and stakeholder expectations and constraints
- **Activities:** Identifying technical, operational, economic feasibility and risks, meeting with clients, documenting the software requirements
- **Outcome:** Requirements Specification Document (Software Requirement Specification-SRS/ Business Requirement Document-BRD) that outlines what the software should accomplish.
2.	**System Design:** After the plan is approved, the product requirements are documented for the actual development process.
- **Goal:** To convert requirements into a technical blueprint for development.
- **Activities:** Create High-Level Design (HLD) that defines architecture, database design, relationship between modules and Low-Level Design (LLD) that defines the logic of individual components, API interfaces and database tables. 
- **Outcome:** Design documents that guide developers and QA teams for implementation and testing highlighting how the software will be developed and how it will be working.
3.	**Development / Implementation:** This is the longest phase in which the actual building of software takes place.
- **Goal:** Build the software according to design specifications.
- **Activities:** Developers write code following coding standards using programming languages and development tools, and perform unit testing for individual modules.
- **Outcome:** Executable software
4.	**Testing:** Once the actual development process completes, testing begins for finding defects in the product before release to ensure quality of the product.
- **Goal:** Ensure the software works as expected and meets requirements.
- **Activities:** QA team executes manual or automated tests, logs defects, and verifies fixes.
- **Outcome:** Test cases, Quality Reports, Bug Reports, etc.
5.	**Deployment:** After the software becomes defect free, it will be released to the end-users. Deployment is often done via CI/CD pipelines.
- **Goal:** Make the software available to users so they can start using it.
- **Activities:** Deploy the application on machines or servers, perform smoke testing, and setup necessary environments.
- **Outcome:** Live software accessible to users.
6.  **Maintenance:** The SDLC must not just end at deployment since it needs maintenance for better experience and usage.
- **Goal:** Keep the software functioning efficiently after release and keep it up-to-date.
- **Activities:** Bug fixes, making updates, performance enhancements, and user support.
- **Outcome:** Reliable, secure, and continuously improved software.


# Software Testing Life Cycle (STLC)
STLC is a subset of SDLC which emphasizes the quality assurance and testing aspects of software development. STLC is like a roadmap for the testing process that is used by the testing teams to ensure the quality of the software product. The goal of STLC is to find and fix bugs so that the software is functional and reliable before the release.
## Stages of STLC:
1.  **Requirement Analysis:** In this stage, the team gathers information regarding the expectations from the software.
- **Goal:** To understand what needs to be tested on the basis of software requirements. 
- **Activities:** Identifying testable items and the types of tests needed, note constraints, reviewing the requirements.
- **Outcome:** Clear understanding of what needs to be tested and a traceability matrix linking requirements to test cases.
2.  **Test Planning:** In this phase, planning is done on what and how to test.
- **Goal:** Create a detailed plan on proper testing methods.
- **Activities:** Define scope, strategy, resources, timelines, and tools to prepare Test Plan document.
- **Outcome:** A test plan document that acts as a roadmap for the testing process. 
3.  **Test Case Development:** After the test planning is done, the test team will create instructions to check if the software works correctly as intended. Then, data required for the tests will be prepared.
- **Goal:** Prepare detailed test cases and scenarios for performing tests on the software.
- **Activities:** Write test cases for functional and non-functional requirements that describes what action to perform, prepare test data, review test cases.
- **Outcome:** Complete test case repository ready for execution.
4.  **Test Environment Setup:** In this stage, setup of computer, software, and tools needed for the tests is done.
- **Goal:** Prepare the environment (hardware, software, network etc.) for testing.
- **Activities:** Set up test servers, installing applications, performing network configuration to verify readiness.
- **Outcome:** Test environment that mirrors production environment and is ready for testing.
5.  **Test Execution:** This is the stage where tests are actually executed. If any issues are found, then it is documented with details for developers to fix.
- **Goal:** Execute tests and identify defects.
- **Activities:** Run test cases manually or via automation, record actual vs expected results, log defects with severity and priority, perform re-testing and regression testing.
- **Outcome:** Test reports consisting of success and failure of software in various aspects and details of any defects found.
6.  **Test Cycle Closure:** In this stage, testing is finished. The test results will be analyzed and lessons learned will be recorded. Any issues found during testing is reviewed and closed.
- Goal: Conclude testing activities, evaluate the results and learn from the process.
- Activities: Prepare a final Test Summary Report, analyze test metrics, document lessons learned, close test cycle.
- Outcome: Completed testing cycle with all results documented and shared.

# SDLC vs. STLC
Here’s a side-by-side comparison to understand the key differences between SDLC and STLC:

| Feature        | SDLC (Software Development Life Cycle) | STLC (Software Testing Life Cycle) |
|----------------|---------------------------------------|-----------------------------------|
| **Definition** | Defines all activities from requirement gathering to maintenance. | Defines all activities related to testing a software product. |
| **Focus**      | Complete software development.        | Quality assurance and testing.    |
| **Objective**  | Develop high-quality software meeting customer requirements. | Ensure software is defect-free and works as expected. |
| **Scope**      | Planning, design, development, testing, deployment, maintenance. | Requirement analysis, test planning, test case design, test execution, test closure. |
| **Performed by** | Developers, business analysts, project managers, testers. | Mainly QA/testing team.           |
| **Coding**     | Major activity.                       | No coding (except automation testing). |
| **Dependency** | Defines overall development process.  | Subset of SDLC.                   |
| **End Result** | Deployed and maintained software application. | Validated, quality-assured software product. |

