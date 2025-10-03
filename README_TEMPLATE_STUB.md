# Stub Service Template README

<details>
<summary>Overview</summary>
- **How to run tests locally:**  
  _Describe prerequisites, setup steps, and commands._

</details>

<details>
<summary>How to Run</summary>

Instructions for running locally and in CI:
- `sbt run` (or relevant command)
- Default port: `xxxx`
- Any required environment variables or configuration

</details>

<details>
<summary>Endpoints</summary>

| Method | Path     | Purpose                   | Notes                          |
|--------|----------|---------------------------|--------------------------------|
| GET    | /example | Returns a static response | Used for ...                   |
| POST   | /example | Accepts ...               | Special cases documented below |

_**Note:** Standard stub endpoints do not require detailed explanation here. Only document endpoints with non-obvious or special-case behaviors below._

</details>

<details>
<summary>Example Requests & Responses</summary>

Show example requests and responses for key scenarios, especially those with non-standard behavior.

**Example:**

Request:
```http
POST /example
Content-Type: application/json

{
  "example": "abc"
}
```

</details>

<details>
<summary>Test Data</summary>

Document **specific request patterns** or test data that trigger special responses.
- **/example endpoint**
    - Request with body `{ "example": "error" }` returns 500 Internal Server Error.
    - Request with missing `Authorization` header returns 401 Unauthorized.
    - Request with query parameter `type=notfound` returns 404 Not Found.

</details>
