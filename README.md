# StalkHub

* Platform to stalk and view different github profiles in a easy way .

* You can view their most starred , forked  and most popular repos , 
* also according to different languages in the form of 3d and 2d graphs and charts. 
* The platform is well authenticated by using Oauth 2 . It makes use of GithubApi and FusionCharts .

* Just login and Stalk your favourite Developer. 


# Setup

## Tech Stack
- ReactJs 
- React Router Dom
- React Icons
- Styled Components
- Fusion Charts
- Auth0
- Github API
- Netlify

## ScreenShots
* Login/SignUp
  <img width="1424" alt="Screenshot 2023-09-14 at 12 07 48 PM" src="https://github.com/PARASnagpal99/StalkHub/assets/86076130/0fd9807d-4ca7-4f77-8d3d-348b703564fa">
  <img width="419" alt="Screenshot 2023-09-14 at 12 08 40 PM" src="https://github.com/PARASnagpal99/StalkHub/assets/86076130/870a33f8-45d9-41d7-a2dd-89158bdb5ab5">
  
* DashBoard , SearchBar , Searched Persons's Profile and its Followers
  <img width="1432" alt="Screenshot 2023-09-14 at 12 09 37 PM" src="https://github.com/PARASnagpal99/StalkHub/assets/86076130/82a87c75-e671-4eec-a246-21ed51703ef3">
  
* Most Used Languages , Most Popular Repos , Stars per Language , and Most Forked Repos visualized in form of charts and Graphs .
  <img width="1201" alt="Screenshot 2023-09-14 at 12 10 20 PM" src="https://github.com/PARASnagpal99/StalkHub/assets/86076130/918b50ac-920a-4f10-b671-d3be8e6f5c8c">




## Styled Components

[Styled-Components - Main Docs](https://styled-components.com/)

```jsx
import styled from "styled-components";

const ReactComponent = () => {
 // logic here
 return <Wrapper>
 {some content}
 </Wrapper>
}


const Wrapper = styled.htmlElement`
write your styles here
`
export default ReactComponent
```

## React Icons

[React Icons - Main Docs](https://react-icons.github.io/react-icons/)

```jsx
import { FiUsers, FiUserPlus } from 'react-icons/fi';
<FiUsers className='nameOfTheClass'> </FiUsers>;
```

## React Router Dom
[React Router](https://reactrouter.com/en/main)

- version 6.4 brought significant changes (loader and action)
- pages as independent entities
- less need for global state
- more pages

#### Setup Router Command
```
npm i react-router-dom@6.10.0
```

## Github API

- [Root Endpoint](https://api.github.com)
- [Get User](https://api.github.com/users/hkirat)
- [Repos](https://api.github.com/users/hkirat/repos?per_page=100)
- [Followers](https://api.github.com/users/hkirat/followers)
- [Rate Limit](https://api.github.com/rate_limit)

  For unauthenticated requests, the rate limit allows for up to 60 requests per hour. Unauthenticated requests are associated with the originating IP address, and not the user making requests.

## Fusion Charts

- [Fusion Charts - Main Docs](https://www.fusioncharts.com/)
- [First React Chart](https://www.fusioncharts.com/dev/getting-started/react/your-first-chart-using-react)
- [List Of Charts](https://www.fusioncharts.com/dev/chart-guide/list-of-charts)
- [Themes](https://www.fusioncharts.com/dev/themes/introduction-to-themes)

## Auth0

- [Auth0 - Main Docs](https://auth0.com/)

- Create Application
- Choose : Single Page Web Applications
- Choose : React
- Go to Settings Tab
- Copy/Paste Domain, ClientID - can be public (or use .env)
- Add Domain -
  for now http://localhost:3000 (DON'T COPY PASTE FROM URL BAR)

  - Allowed Callback URLs
  - Allowed Logout URLs
  - Allowed Web Origins
  - SAVE CHANGES!!!!!!!!!!!!!!!

- Connections
  email,social

- [React SDK Docs](https://auth0.com/docs/libraries/auth0-react)
- [REACT SDK API Docs](https://auth0.github.io/auth0-react/)

## Deployment

[Netlify](https://www.netlify.com/)

## Additional Info

#### Redirects with react-router-dom

In order for routing to work on netlify, redirects was added to the public folder

- \_redirects file in public

```

/*    /index.html   200

```

[Redirects Blog Post](https://dev.to/dance2die/page-not-found-on-netlify-with-react-router-58mc)

#### Warnings and create-react-app

package.json

```js
"build": "CI= react-scripts build",
```

[create-react-app Warning Fix Blog Post](https://community.netlify.com/t/how-to-fix-build-failures-with-create-react-app-in-production/17752)
