## Business Requirements

Due to privacy concerns around user data and concerns that the cost of managed services for GenAI will exceed the budget set for this project.
The goal of this project is to create enhance the current platform available for students to learn and practice their Japanese.  In future
iterations the company would like to be able to provide the same experience with different languages.  This iteration will focus solely on Japanese.

## Functional Requirements

As stated above due to privacy concerns the company would like to invest in an in-house solution.  This will require the purchase of a computer that can support AI.  The company has a budget of 10-15k per computer and currently have 300 students located within the city of Nagaski.

## Non-functional Requiremnts

Students must experience a seamless experience and perform at a speed that keeps them engaged.  At any given time there could be 50-100 students engaged in learning activities.  Students must also be able to save their progress and be able to resume learning where they left off.


## Assumptions

We are assuming the following things:
- Students will access the portal at various times of the day so system uptime and availability must be a focus.
- The Open-source LLMs being used are routinely scanned and any vulnerabilities will be addressed.
- The network will be scanned on a schedule to make sure that no spyware or other viruses have been introduced.
- Since Open-source LLMs are being used the network/system will be locked down in such a way that students can not update nor change the sources.
- The Open-source LLMs will be able to run on the computer selected and that it will be enough bandwidth to serve the students as the current plan is to set up a computer and allow students to connect.

## Data Strategy

The data collected will be validated for accuracy and copyright infringement possibilities.  The data will be cleaned prior to being loaded into the system for student use ensuring that bad data is removed.  Students will also be given the option to 'flag' data they feel is incorrect or inappropriate for review.  We will ensure that data comes from different sources to ensure a variety of learning for the students.  Certain data for students will be collected as this will help us enhance their learning experience but only the data required for learning language will be collected.  Access to social media sites and access sites will be blocked for security purposes.

## Integration and Deployment

We are going to use a cloud based solution (AWS) to host this environment along with containers.  Students will connect to the portal and 'check out' one of the containers containing the application. The container will restrict access to the greater Internet and allow for us to easily patch and update to newer versions.

## Monitoring and Optimization

Using containers will allow us to easily monitor what students are doing.  Errors in the program or container will generate an error report that can be reviewed.  15-30-60 and 90 day check points will occur along with student survey's asking for their experience using the platform so far.

## Governance and Security

Students will be required to take a training course prior to using the platform explaining appropriate use.  All sessions will be monitored and logged for review when needed.  Words that have been deemed offensive have been flagged and will not work on the program.  Students who violate policies will be removed from the program and no longer allowed to learn on the platform.  Routine review of industry standards and regulations will occur on a monthly basis and adjustments will occur to our internal policies as needed.

## Scalability and Future-Proofing

Containers will be used due to their ease of updating and flexibility.  We will operate on an n-1 policy with version updates to ensure that we stay up to date but not on the bleeding edge. This will allow us to properly vette new versions and review changelogs to ensure we aren't introducing unecessary risk.  Future plans include setting up a classroom setting where students can come and learn in person on devices provided.

## Considerations

IBM Granite is currently the top candidate for this effort.  It is a true open-source model that comes with training data that is traceable so the possibility of copyright issues is minimal.

https://huggingface.co/ibm-granite