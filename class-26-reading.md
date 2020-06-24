### *Hooks API*

#### What does a component’s lifecycle refer to?
Each component in React has a lifecycle which you can monitor and manipulate during its three main phases. The three phases are: Mounting, Updating, and Unmounting.

#### Why are functional components preferred over class components?
Developers tended to favor functional components for their ease of implementation, and so Hooks were added as a way to enable that further.

#### What is wrong with the following code?

Hook should not be used within the for loop.

```JS
import React, {useState, useEffect} from 'react'; 
   
function MyComponent(props) {
  const [count, setCount] = useState(0); 
     
  function changeCount(e) {
    setCount(e.target.value); 
  }
     
  let renderedItems = []
     
  for (let i = 0; i < count; i++) {
    useEffect( () => {
      console.log('component mount/update'); 
    }, [count]); 
       
    renderedItems.push(<div key={i}>Item</div>); 
  }
     
  return (<div>
    	<input type='number' value={count} onChange={changeCount}/>
      {renderedItems}
    </div>);
}
```


