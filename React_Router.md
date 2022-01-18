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

8. Add Component
```
const Home = (props) => {
  return (
    <h1 style={{color: "red"}}>Home Component</h1>
  );
}
    
const About = (props) => {
  return (
    <h1 style={{color: "blue"}}>About Component</h1>
  );
}
```

9. In App.js, Add Switch Around Each Component
```
    <BrowserRouter>
      <Switch>
          <Home />
          <About />
      </Switch>
    </BrowserRouter>
```

10. Wrap each component with the Route that specifies that Component
```
    <BrowserRouter>
      <Switch>
        <Route path="/about">
          <About />
        </Route>
        <Route path="/">
          <Home />
        </Route>
      </Switch>
    </BrowserRouter>
```

11. Use "exact keyword in Route to make sure only that route will fire that component
```
    <BrowserRouter>
      <Switch>
        <Route exact path="/">
          <Home />
        </Route>
        <Route path="/about">
          <About />
        </Route>
      </Switch>
    </BrowserRouter>
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