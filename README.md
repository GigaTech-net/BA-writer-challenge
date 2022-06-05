# GigaTECH Writing/Business Analyst Challenge

Hi! Thank you for your interest in [GigaTECH][gigatech]. Our hiring process may include a writing challenge. This challenge allows us to gauge some of your basic written communication skills. We will follow the challenge up with aa  interview to discuss what you have submitted.

We appreciate that any research and writing challenge represents an investment of your time. We hope you see the value in having a writing sample that is relatable to both of us for the interview. You should feel free to use the paper you developed for this challenge in any way that you would like.

## The Challenge

One of the challenges we face as technical analysts is the ability to find and consume the appropriate information specific to a task, while disregarding what does not matter at that point in time. This challenge is designed for you to consume information and write a small paper. We will expose you to some of the concept, technologies, and regulations that we deal with everyday, such as [FHIR &reg;][fhir] and [SMART &reg;][smarttech]. You are not expected to learn these technologies but merely use them to create the browser based application.

A common problem for clinicians today is how to extend their Electronic Health Record (EHR) applications with functionality that is useful. New functionality must not interfere with their current workflow. SMART &reg; offers a mechanism to do just that. We would like for you to develop a browser based application that uses the [EHR launch sequence](http://www.hl7.org/fhir/smart-app-launch/#ehr-launch-sequence) to display the allergies (in json format) for the current patient being viewed in the EHR.

Ideally, this would take a junior developer no more than 1 hour to complete.

## Minimum Requirements

    Your browser based application must meet this minimum requirements.

- The application shall run on the following host/port, http://127.0.0.1:8080/, with the "npm run serve" command.
- The application shall display the allergy information for the selected patient.
- The application shall display an error message indicating allergies were not found if no allergies were found for the selected patient.
- The application shall use any provider (clinician) available when being launched.
  - Dr. Albertine Orn is a good default provider with which to log in with
- The application shall work with any patient in the patient list.
  - Ms. Mariana Acuna has at least one allergy.
- The application shall be able to be launched/tested by clicking this link ... [test me](http://127.0.0.1:8080/launch.html?launch=eyJhIjoiMSJ9&iss=https%3A%2F%2Flaunch.smarthealthit.org%2Fv%2Fr4%2Ffhir).
- The application shall communicate with a release 4 FHIR server.
  - for instance, https://r4.smarthealthit.org
- Your submittal shall be a GitHub repository that you create, either by forking this one or creating your own.

## Prerequisites

- None

## Getting started

- You will probably want to install npm
  - For MacOS, these links may help you (MacOS is not required to perform this challenge)
    - [Homebrew][homebrew]
    - [NVM][nvm]
    - [Nodejs][node]
- This is a sample "npm run serve" script
  - "serve": "./node_modules/http-server/bin/http-server src -p $npm_package_config_port --cors",
  - note the use of the http-server npm module
- Take the [SMART &reg; Building a Javascript tutorial][smarttutorial]! Really!

## Submission

When you are comfortable with your results, please email a link to your GitHub repository to [GigaTECH Development Challenge][gthr]. Please keep your emails short and to the point.

Any specific notes or further information you would like to add about your submittal, should be included in the GitHub project, as additional [GitHub Markdown][ghmd] notes.

Do not feel as though you must create a public fork of this repository. You are free to create a throwaway GitHub account or private fork. In those cases, please let us know, at the above address, so that we may send you the GitHub IDs to add to the repository.

## Evaluations

The code written for this challenge will be used in the next step of the interview process. You will discuss what you did with your technical interviewer. Although minimum requirements are set for this challenge, if you'd like to spend more time and enhance your submittal, you are welcome to, but this is not a requirement.

Areas to potentially expand upon (this is not an exhaustive list)

- add unit tests to your project
- parse the json and display the output, versus just displaying the json
- handle errors in a nice way for the user
- Responsive presentation, determining the screen size and autoscaling the display

## License

This project is [MIT Licensed](LICENSE).

## References

The following references may be useful in this challenge.

- [Github Markdown][ghmd]
- [FHIR Specification][fhir]
- [21st Century Cures Act][21curesact]

[gthr]: mailto:HR@gigatech.net?subject=[GigaTECH%20Development%20Challenge]%20Submittal "GigaTECH HR email submittal"
[gigatech]: https://gigatech.net "GigaTECH Home"
[ghmd]: https://guides.github.com/features/mastering-markdown/ "Github Markdown"
[smarttech]: http://docs.smarthealthit.org/ "SMART technical reference"
[fhir]: https://hl7.org/fhir "FHIR Specification"
[21curesact]: https://www.healthit.gov/curesrule/ "21st CEntury Cures Act"
