# Contributing Guidelines

Thank you for considering contributing to the Prowide Core and Prowide ISO 20022 projects! We welcome contributions that help improve the libraries.
The following sections describe different options on how you can contribute.

## A) Submitting Code

If the contribution is small, just minor API changes or enhancements, you can follow this procedure:

1.	Fork the repository you want to contribute to:
*	[Prowide Core](https://github.com/prowide/prowide-core): Implements the core messaging framework and SWIFT MT message handling.
*	[Prowide ISO 20022](https://github.com/prowide/prowide-iso20022): Provides support for ISO 20022 message parsing, building.

2.	Create a branch for your changes:

```
git checkout -b feature/your-feature-name
```

3.	Write Clean, Documented Code

*	Follow the existing coding style.
*	Include **Javadocs** for public classes and methods.
*	Write **tests** for new functionality or changes.


4.	Run Tests: Ensure all tests pass before submitting your changes:

```
./gradlew test
```

5. Check the quality checks in the console and fix what is reported for the classes you have added or modified.


6.	Submit a Pull Request

*	Push your changes to your forked repository.
*	Open a Pull Request to the ```main``` branch with a clear description of the changes.

7. Check the code quality reports in the opened pull request and resolve the issues acordingly.

If the contribution is bigger, including a refactor, or with a high impact on the existing code base; it a good idea to propose it first and have a design interchange with other developers before jumping into code changes. 
You can initiate a discussion with your proposal at [Discussion](https://github.com/orgs/prowide/discussions/categories/ideas)

### Development Environment

*	Gradle: Use Gradle commands for building and testing, the Gradle wrapper is included in the project, thus no external Gradle installation is needed.
*	Recommended IDE: IntelliJ IDEA.
*	Notice the current code base is still compatible with *Java 8* (the Java 11+ version is being maintained in paralel), code contributions shoudl go to the ```main``` branch which is compiled with **Java 8**.
*	Notice some of the code is **generated** and the generation tools are not publicly available in the open source repositories. If the constribution or proposed changes are for code contained in the ```src/generated``` folder or flagged with the annotation ```@Generated``` do not change the code directly, propose the change in a discussion instead.

## B) Reporting Bugs

* Check existing issues: Before reporting a bug, check the [Prowide Core issues](https://github.com/prowide/prowide-core/issues) section or the [Prowide ISO 20022 issues](https://github.com/prowide/prowide-iso20022/issues) to avoid duplicates.
* Provide details: Include as much information as possible (library version, environment, steps to reproduce, and expected/actual behavior, and ideally a test case).
* Use the label bug when submitting an issue.

## C) Requesting Features

*	Describe the use case: Clearly explain the feature’s purpose and the problem it solves.
*	Scope: Feature requests should align with the goals and scope of the project.
*	You can initiate the feature request by either submitting an issue in the corresponding project or initiating a new Idea in the [Discussion](https://github.com/orgs/prowide/discussions/categories/ideas)

## D) Improving Documentation

Documentation is hosted at [Documentation resources](https://dev.prowidesoftware.com/latest/open-source/), written in markup and not public. However, you can propose enhancements.
Spot missing content or propose new section, corrections or ammendments via the [Prowide Core issues](https://github.com/prowide/prowide-core/issues) section or the [Prowide ISO 20022 issues](https://github.com/prowide/prowide-iso20022/issues)



## Need Help?

If you have questions or need guidance, feel free to:

*	Open a discussion in the [Discussions](https://github.com/orgs/prowide/discussions).
