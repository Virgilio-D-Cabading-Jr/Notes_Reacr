# Using React Router on Front End

1. Create a React Project
```
nx create-react-app PROJECT-NAME
```

2. Then navigate to inside the project fold

3. Inside the project fold, Install React Router dependencies
```
npm install react-router-dom@5
```

4. In App.js, Import Browser Router and Link
```
import { BrowserRouter, Link } from "react-router-dom";
```

5. In App.js, Wrap Browser Router Arund Everything:
```
function App() {
  return (
    <BrowserRouter>
      <h1>React Routing Demonstration</h1>
      <p>
        <Link to="/">Home</Link>
        &nbsp;|&nbsp;
        <Link to="/about">About</Link>   
      </p>
    </BrowserRouter>
  );
}
    
export default App;
```

6. Links:
```
<Link to="/">Home</Link>
<Link to="/about">About</Link>
```

7. Import Switch and Route into App.js
```
import { Switch, Route } from "react-router-dom";
```

7. How to add a Non-Breaking-Space
```
&nbsp;
```

8. How to add a Break Line
```
<br>
```

9. How to add a line
```
<hr>
```