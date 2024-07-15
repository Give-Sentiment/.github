<h1 align="center">Welcome to Sentiment's GitHub Organization</h1>

<div id="header" align="start">
  <div align="center">
  <img src="https://sentiment-survey-logos.s3.us-east-2.amazonaws.com/8aa0c65f-2232-49c8-a647-29b039d9f5c1.jpeg" width="150"/><br>
  </div>
    <br>
    <br>

## Our Software
We want to build tools that aid in data collection and data valuation. It's that simple. Our software will include bits and integrations with the following:

- Survey Service
- Biometric Authentication APIs
- Dor Hardware Devices
- Blockchain
- Langchain Functions
- etc.

## Reach out for help
We are a team -- please reach out to any team member if you need help for any convoluted or non-complicated reason. We are here to help each other.

- **Kory Ryan** - Software Engineer
- **Evan Wang** - Software Engineer
- **Austin Margarone** - Software Engineer
- **Mike McMahon** - CTO & Technical Co-Founder
- **Ryan Paglione** - COO & Technical Co-Founder

## Security Practices
We require all of our team to be onboarded through SOC 2 II compliant practices, security awareness, and certifications prior to touching code.

- Regularly review OWASP guidelines, OpenAPI, and integrate security checks (e.g., Snyk).
- Follow best practices for securing environment variables using Vault.
- Ensure all PII (Personal Identifiable Information) data is private or encrypted.

- [OWASP guidelines](https://owasp.org/www-project-secure-coding-practices-quick-reference-guide/stable-en/02-checklist/05-checklist)
- [OpenAPI Reference](https://swagger.io/specification/)
- [PII Practices](https://www.virtru.com/blog/compliance/hipaa/pii-encryption-best-practices#:~:text=It%20requires%20encryption%20in%20transit,or%20damage%20to%20your%20reputation.)

## Branch Naming Strategies
These are branching strategies, in which we will keep in short and sweet -- decide whether you are working on a feature, a bugfix, or doing an experiment -- please pre-pend your branch with this followed by the ticket 'chapter', with a very short description of what you are working on. **Keep everything lowecase except the ticekt chapter, ie SNT-001**

1. **Feature**: `feature/<ticket-number>-<short-description>`
   - Example: `feature/SNT-001-add-login-page`
   
2. **Bugfix**: `bugfix/<ticket-number>-<short-description>`
   - Example: `bugfix/SNT-001-fix-login-issue`
   
3. **Experiment**: `experiment/<short-description>` * as these are not tickets so there is no ticket 'chapter', but feel free to experiment.
   - Example: `experiment/new-login-cache-strategy`

## Commit Related Changes
A commit should be a wrapper for related changes. For example, fixing two different bugs should produce two separate commits. Small commits make it easier for other developers to understand the changes and roll them back if something went wrong.

  **CLI Commits**
  - Use your CLI to `git add .`
  - Then `git commit -m "SNT-001` <- Notice how I did not add an 'end quote'
  - Press 'enter', in which you cli should show `dquote>` or some equivelant. This is how we can produce multiple lines.
  - On these following lines you may enter a brief description of the work `dquote> addded the login feature`
  - You may press enter and repeat for as many lines as you need, but please keep it to a reasonable amount.
  - When you are done with your commit you may now add the final quote in your cli `"` in which this will close the commit message
  - Finally `git push` to your branch, in which this will automatically trigger our CI/CD pipeline.

1. **Commit Often**
Committing often keeps your commits small and, again, helps you commit only related changes. Moreover, it allows you to share your code more frequently with others. That way it‘s easier for everyone to integrate changes regularly and avoid having merge conflicts. Having large commits and sharing them infrequently, in contrast, makes it hard to solve conflicts.

2. **Don't Commit Half-Done Work**
You should only commit code when a logical component is completed. Split a feature‘s implementation into logical chunks that can be completed quickly so that you can commit often. If you‘re tempted to commit just because you need a clean working copy (to check out a branch, pull in changes, etc.) consider using Git‘s «Stash» feature instead.

3. **Test Your Code Before You Commit**
Resist the temptation to commit something that you «think» is completed. Test it thoroughly to make sure it really is completed and has no side effects (as far as one can tell). While committing half-baked things in your local repository only requires you to forgive yourself, having your code tested is even more important when it comes to pushing/sharing your code with others.

4. **Write Good Commit Messages**
We will use an interesting strategy for commit messages, please reach out if you need alignment on doing this. Previous to committing, review the files you are changing in the source control extension in your IDE (typically on the left side bar in VSCode). Then navigate to your cli and follow these steps: 

## Workflow

1. **We Will Communicate as a Team and Assign Tickets and Tasks**:
   - Find alignment with Mike or Ryan, ensure you understand the task and an approach on how to tackle the task. Reach out for help.

2. **Pull Main**:
   - Use your CLI to `git fetch --all`
   - Use your CLI to `git pull`
   - Ensure your branch is up-to-date with main

3. **Create Branch**:
   - Use your CLI to `git checkout -b <branch-type>/<ticket-number>-<short-description>`
   - Example: `git checkout -b feature/SNT-001-add-login-page`

4. **Make Atomic Commits**:
   - Commit single logical changes with clear, concise messages.
   - Use your cli to `git add .`
   - Then `git commit -m "SNT-001`
   - `dquote> fixed auth and added correct login timeout`
   - `"`
   - Finally `git push` in which it may prompt you to set up stream for the first commit.
   - Utilize **CLI Commits** (from the above 'Commit Related Changes' section above) after your branch is upstream.

5. **Push Branch**:
   - Push your branch to the remote repository.
   - Example: `git push origin feature/SNT-001-add-login-page` 

6. **Create Pull Request (PR)**:
   - Navigate to the repository on GitHub.
   - Create a pull request for your branch, ensuring it targets the `main` branch.
   - Provide a clear description of the changes and request a review.

7. **Code Review**:
   - Participate in code reviews, providing constructive feedback.
   - Address any comments or requested changes on your PR.

8. **Merge Pull Request**:
   - Once approved, merge your pull request into the `main` branch.
   - Use the "Squash and merge" option to keep the commit history clean.

9. **Pull Main Again**:
   - Ensure your local `main` branch is up-to-date.
   - Use your CLI to `git fetch --all`
   - Use your CLI to `git pull`

## Welcome!
We are excited to have you, and are happy to find that you align with us in working on some really cool technologies! Always reach out for any help, as we are a team.
