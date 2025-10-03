# UI Test Template README

UI test suite for the `[service-name]`

<details>
<summary>External Documentation</summary>

- [Link to test data or journey documentation](#)
- [Any other relevant external docs](#)
</details>

<details>
<summary>Running the tests</summary>

1. **Start required services**
```sh
  sm2 --start [SERVICE_PROFILE] --wait [SECONDS]
```

Or use the provided script:
```sh
  ./startup.sh Example
```
To run all standard journey tests:
```sh
  ./run-tests.sh Example
```
To run smoke tests against a specific environment:
```sh 
  ./run-smoke.sh Example
```
</details>

<details>
<summary>Journeys Covered</summary>

The following journeys are covered by this test suite: (Team to decide on the level of detail required here)
* Feature("A user goes through the Unincorporated Association Flow")
* TrustE2ESpecNoMatch.scala
* [Link to Journey on github ?? ](https://github.com/hmrc/minor-entity-identification-ui-journey-tests/blob/12f4d4e9ad5d4251893374f258360e02d8f449a3/src/test/scala/uk/gov/hmrc/test/ui/specs/UnincorporatedAssociation/UaE2ESpec.scala)
* Example....
* 
</details>

<details>
<summary>Jenkins</summary>

The Jenkins job for these tests are located at:

> https://build.tax.service.gov.uk/job/SIS/identity-verification-ui-tests example

And has been integrated into the build pipelines:

> https://build.tax.service.gov.uk/job/SIS/job/identity-verification-stub-pipeline/ example

</details>

<details>
<summary>Troubleshooting</summary>  

To access the journey in staging, go to:

> https://www.staging.tax.service.gov.uk/example-page

Information on running the journey in staging.
</details>