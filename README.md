# psclientsidereactroute4

## 3.Dynamic Routing
### 3 Demo: Dynamic Routes
HashRouter will be deprecated.
```
import { BrowserRouter as Router, Route } from 'react-router-dom';
const App=()=>{
  return (
    <Router>
      <Route path='/' component={Home} />
    </Router>
  )
}
```


## 4. Client and Server Routing

Pro | Con
--- | ---
Routing is generally faster |
Smooth transitions are easy to implement |
It's simple to render client-side views |
Can render only part of a page without a full page refresh |
No refund trip to the server for the entire UI |


## 7. Nesting Routes
### 3 Demo: Multiple Route Parameters
```
const SmartColorSwatch = ({match})=>{
  let style={backgroundColor: match.params.color
};
return(
  <div style={style}>
    <h2>{match.params.text}</h2>
  </div>
  );
);
```
