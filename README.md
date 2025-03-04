In this project, let's fix the **IPL Dashboard** by applying the concepts we have learned till now.

### Refer to the image below:

<br/>
<div style="text-align: center;">
    <img src="https://assets.ccbp.in/frontend/content/react-js/ipl-dashboard-output-v2.gif" alt="ipl dashboard output" style="max-width:70%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12)">
</div>
<br/>

### Set Up Instructions

<details>
<summary>Click to view</summary>

- Download dependencies by running `npm install`
- Start up the app using `npm start`
</details>

### Completion Instructions

<details>
<summary>Functionality to be fixed</summary>
<br/>

Fix the given code to have the following functionality

- When the app is opened, Home Route should be displayed
- When the Home Route is opened,
  - Make HTTP GET request to the **teamsApiUrl**
  - **_loader_** should be displayed while fetching the data
  - After fetching the data, the list of teams should be displayed
- When a team card in Home Route is clicked,
  - Page should be navigated to the Team Matches Route with the URL `/team-matches/:id`
- When the Team Matches Route is opened,
  - Make HTTP GET request to the **teamMatchesApiUrl** with the team id to get the recent matches data of the team
    - Example: `https://apis.ccbp.in/ipl/KKR`
  - **_loader_** should be displayed while fetching the data
  - After fetching the data, the team banner, latest match, and list of recent matches should be displayed

</details>

<details>

<summary>API Requests & Responses</summary>
<br/>





### Quick Tips

<details>
<summary>Click to view</summary>
<br>

- There are `13` bugs to be fixed to achieve the functionality and the UI that is expected

</details>

### Important Note

<details>
<summary>Click to view</summary>

<br/>

**The following instructions are required for the tests to pass**

- Wrap the `Loader` component with an HTML container element and add the `data-testid` attribute value as `loader` to it as shown below

  ```jsx
  <div data-testid="loader">
    <Loader type="Oval" color="#ffffff" height={50} width={50} />
  </div>
  ```

</details>

> ### _Things to Keep in Mind_
>
> - All components you implement should go in the `src/components` directory.
> - Don't change the component folder names as those are the files being imported into the tests.
> - **Do not remove the pre-filled code**
> - Want to quickly review some of the concepts you’ve been learning? Take a look at the Cheat Sheets.
