# Repository Name

<details>
<summary>Summary</summary>

!!!Brief description of what this service does and its purpose within the system. This should be sourced from Confluence, the existing README.md and your own knowledge of the repository.!!!
https://confluence.tools.tax.service.gov.uk/display/DDCW/Catfish+Projects
</details>

<details>
<summary>Feature Flags</summary>
!!!These can be found in `application.conf` typically under a set called `feature` or a similar name!!!
!!!Information for the description can be found by analysing their usage under `/app` in the main project files!!!
!!!This should follow the format below!!!

| Feature Flags         | Description                 |
|-----------------------|-----------------------------|
| feature-flag-name     | Description of feature flag |
| another-feature-flag  | Description of feature flag |
</details>

<details>
<summary>Running Service</summary>

!!!This should follow the format below!!!

Steps to run the service locally:
1. You will need SM2 as well as a mongo/docker set up. Detailed instructions can be found in the [Developer Handbook](https://docs.tax.service.gov.uk/mdtp-handbook/documentation/developer-set-up/index.html)
2. Start up the SM2 profile `sm2 --start <PROFILE_NAME>`
3. Stop the current service (if you want to test your changes) `sm2 --stop <SERVICE_NAME>`
4. View the exact journey information found at [<Service_Acceptance_Tests_Journey>](link-to-acceptance-tests-journey)
</details>

<details>
<summary>Testing</summary>

!!!This should follow the format below!!!

### Manual Testing
- Steps for manual testing. Refer to running the service

### Local Testing
1. You will need SM2 as well as a mongo/docker set up. Detailed instructions can be found in the [Developer Handbook](https://docs.tax.service.gov.uk/mdtp-handbook/documentation/developer-set-up/index.html)
2. Start up the SM2 profile `sm2 --start <PROFILE_NAME>`
3. Stop the current service (if you want to test your changes) `sm2 --stop <SERVICE_NAME>`. Then run the service with !!!This can vary depending on service. Sometimes a simple `sbt run` will work. Sometimes a dedicated script or command is required. Check the current README.md for context!!!
- Run the script `./test.sh` which will run the command `sbt coverage test it/test coverageReport dependencyUpdates`. This will check coverage meets the standard. Run the integration and unit tests. Produce a coverage report and finally inform you of any dependencies behind on versions.

### Test Repositories
Links to related test repositories:
- [Acceptance Tests](link-to-repo)
- [Performance Tests](link-to-repo)

### Jenkins Testing
- A list of all SIS builds can be found at [SIS - Jenkins](https://build.tax.service.gov.uk/job/SIS/)
- Acceptance tests can be triggered by picking the relevant service, clicking `Build with Parameters` then clicking `Build`. If you wish to run against a specific branch of the UI/Acceptance tests then enter the branch name under the `BRANCH` field
- [Perfomance Tests](https://performance.tools.staging.tax.service.gov.uk/job/VERIFICATION/) Similarly to acceptance are triggered under `Build with Parameters` however you have additional options for adjusting load and running smoke tests.
</details>

<details>
<summary>API's</summary>
</details>

<details>
<summary>Endpoints</summary>

!!!You can generate the list of endpoints using `.route` files typically found under `/conf`!!!
!!!This should follow the format below!!!

Base URL:
- `/base-url`

List of available API endpoints:
- `GET /endpoint1` - Description
- `POST /endpoint2` - Description
- `PUT /endpoint3` - Description
</details>

<details>
<summary>Example Requests/Responses</summary>

!!!This should follow the format below!!!

### Sample Request 1
```json
{
  "example": "request body"
}
```

### Sample Response 1
```json
{
  "example": "response body"
}
```
</details>

<details>
<summary>cURL/Bruno</summary>
!!!If there are any relevant cURL or Bruno collections, provide links to them here!!!
!!!cURL commands for testing this service!!!
</details>
